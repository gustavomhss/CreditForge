# Roadmap — CreditEngine\$ (MVP → R1/R2/R3) — vA3.1.11 (CANÔNICO — impecável+)

> **Hierarquia:** Master KB > docs anteriores até ADR. Atualizações devem ser registradas em `decision_log.md`.
>
> **\[CANÔNICO]** `<<<PREENCHER_URL_CANONICA_DA_MASTER_KB_ANTES_DO_GATE_M0>>>` *(preencher e validar HTTP 200 antes do Gate M0; registrar hash SHA‑256 e timestamp no `decision_log.md`)*
>
> **Precondição M0:** esta URL deve estar preenchida e acessível (**HTTP 200**) antes do Gate M0.
>
> **Unidades:** `_bps` • `_days/_seconds` • **centavos** (off‑chain) • **wei** (on‑chain).  **Bases:** **APR = 365**; **CDI = 252**; **day\_count = ACT/365F**.
>
> **ADRs base:** ADR‑001 (**SLA ≤ `21600 _seconds`**) • ADR‑002 (taxa 0,50%) • ADR‑003/004/005 (em evolução).
>
> **Nota de versão (vA3.1.11)** — *patches de impecabilidade*
>
> 1. **Banking/Inbounds clarificado**: `Content-Digest` **opcional para webhooks inbound** (provedor→CE); **obrigatório nos outbound** (CE→parceiro). Inbound **requer** `X-Signature: sha256=<hex>` (**HMAC‑SHA256**) por `provider_id`.
> 2. **Status CANCELLED** incluído no mapeamento provider→interno (Banking).
> 3. **Telemetria unificada**: parâmetro **canônico** `telemetry_window_seconds = [120, 300]` referenciado uma única vez (evita redundância).
> 4. **Semântica Offer.UPDATED** reforçada em **Invariantes** (R2+: **apenas reduções**; monotonicidade para baixo).
> 5. **Expiração de leilão**: regra explícita `expiry_ts ≤ ts_utc(AuctionCreated) + auction_ttl_seconds` (MVP) e consistência com anti‑sniping (máx `+600s`).
> 6. **Tabelas e enums**: normalização de nomes/casos; remoção de repetições; exemplos com **round half‑up** (APR) preservados.

---

## 🎯 Visão Macro

* **MVP (Fase 0)**: marketplace P2P com leilão reverso (uniform‑price adaptado; **clearing = média ponderada por centavos**; `apr_weighted_bps` **inteiro (round half‑up)**), LoanVault (cobre até o valor colateralizado), token CE\$ lastreado, integrações mínimas (score fiat, KYC/AML PF), **UX 3 telas + fallback (SLA `7200 _seconds` — override do ADR‑001; registrar no `decision_log.md`)**.
* **R1**: reforço de protocolo e observabilidade (**anti‑manipulação `observe_only`**), banking, KYC/AML PJ, logs/eventos **assinados** com RBAC completo.
* **R2**: expansão de integrações (scores alternativos, **reputação/badges on‑chain**, novos colaterais, **governança inicial de parâmetros**), início do **enforcement anti‑manipulação e mínimos por oferta**.
* **R3**: consolidação global (bureaus internacionais, **multimoeda** com FX oracle e livros segregados, **governança plena**, **secundário líquido** — “quanto pagar por cada R\$ 1”).

---

## 🟢 MVP (Sprint 0–2)

**Guardas & Defaults (MVP)**

* **Juros mínimo**: `min_apr_365_bps = 600` (≥ 6% a.a., base 365).
* **Juros máximo**: `max_apr_365_bps = 5000` (≤ 50% a.a., base 365).
* **Mínimo por oferta**: `min_offer_amount_cent = 100` *(R\$ 1,00 — **R1: observe\_only**; **R2+: enforcement rejeita ofertas < mínimo**).*
* **TTLs**: `offer_ttl_seconds = 300`, `auction_ttl_seconds = 3600`.
* **Expiração do leilão**: exigir `expiry_ts ≤ ts_utc(AuctionCreated) + auction_ttl_seconds`. Extensões por anti‑sniping **não** alteram esse limite além de `+600s` (ver BL‑003 e Invariantes #3).
* **Heartbeats (MVP = telemetria interna)**: `oracle_liveness_crypto_seconds = 93600`, `oracle_liveness_fiat_seconds = 691200` *(eventos a partir de R1).*
* **Widget APR média (bps)**: **exclusivamente** `LoanConfirmed.apr_weighted_bps` (ponderada por **centavos**; **round half‑up**; **base 365 (APR)**). **Fórmula APR→252** e **day\_count=ACT/365F** no Apêndice.

**Sprint 0**: foundation → Product Brief v6.0, ADR‑001/002 aprovados, backlog + critérios + métricas.

**Sprint 1**: protocolo básico

* **BL‑001 Ordenação** — **Algoritmo determinístico**: ordenar ofertas por **(1)** `apr_365_bps` **asc** → **(2)** `amount_cent` **desc** → **(3)** `ts_utc` **asc** → **(4)** `offer_id_hash` **asc** *(sha‑256 hex)*.
* **BL‑002 Pró‑rata** — Método dos **maiores restos** em centavos; distribuir resíduos de 1 centavo por **maior fração** e, em empate, por **ordem determinística de lender** (lexicográfica). Soma final **==** `total_amount_cent`.
* **BL‑007 UX 3 telas + fallback**
* **BL‑009 Logs imutáveis**
* **〽️ KPIs (observado)**: **Funding P95 ≤ `86400 _seconds`**, **Pool ≥ 65%**, **Yield\_gap\_net\_bps ≥ 150\`**.

**Sprint 2 (planejada)**

* **BL‑003 Anti‑sniping** (**observe\_only** em MVP/R1; **enforcement** a partir de **R2/BL‑003**):
  Regra inequívoca (MVP): *apenas **uma extensão total** por auction* — **feature‑flag** `anti_sniping.single_extension=true`.
  `new_expiry = min(original_expiry + 120s, last_valid_bid_ts + 120s, original_expiry + 600s)`; registrar `extended_by_seconds` (0 ou >0).
  *(Mais restritiva que ADR‑005; registrar desvio no `decision_log.md`; manter feature‑flag para rollback.)*
* **BL‑005 Banking**: taxa **0,50%** no desembolso + conciliação.
* **BL‑006 KYC/AML PF** + Chainalysis + **RBAC** + auditoria de leitura.

**Fallback UX — regras explícitas**

* `RequestOnHold` **não trava capital**; aceita novas ofertas mas **não confirma**.
* Capital **só é bloqueado** em `LoanConfirmed`.
* Ao retomar, **recalcula pool e expirações**.
* **SLA `7200 _seconds`** com `RequestAutoCancelled` (**override ADR‑001; logar no `decision_log.md`**).
* **Medição de SLA em UTC; exibição no timezone do usuário** (ADR‑001).

---

## 🟡 Release 1 (R1)

### Protocolo & Produto

* **Anti‑manipulação (telemetria): `observe_only`** — Parâmetros canônicos: `min_delta_bps: 5`, `min_change_interval_seconds: 30`, `telemetry_window_seconds: [120, 300]`, `rate_limit_offers_per_lender_per_minute: 6` (**escopo global por lender**). *Sem bloqueio/reject em R1; apenas telemetria e alertas.*
* **Semântica `Offer.UPDATED`** — **R1 (observe\_only)**: aceitar **reduções ou aumentos** de APR; registrar `delta_bps` (telemetria). **R2 (enforcement)**: aplicar `min_step_bps=5` e **permitir apenas reduções** de APR (monotonicidade para baixo). Parâmetro votável em R2+: `offers_updated_allow_increase=false`.
* **Pré‑pagamento (ADR‑003)**: sem multa; **juros pró‑rata die**; **taxa 0,50% não reembolsável** (ADR‑002).

### Banking

* **Conciliação multi‑gateway** com **idempotência por** `idempotency_key = sha256(provider_id + payment_id)` **(hex lowercase)** e reconciliação **D+0 (`0 _days`)**.
* **Callbacks financeiros (INBOUND)**: SLA ≤ `21600 _seconds` (ADR‑001); **autenticidade obrigatória** via `X-Signature: sha256=<hex>` (**HMAC‑SHA256** com segredo por `provider_id`). `Content-Digest` **opcional** inbound: se ausente, **computar e logar** internamente.
* **Webhooks CE→parceiro (OUTBOUND)**: **exigir** `Content-Digest: sha-256=:<base64(SHA-256(payload))>:`.
* **Espelhamento de idempotência no canal**: preferir header externo **`Idempotency-Key`**; se ausente, usar **`CE-Idempotency-Key`** = `payload.idempotency_key` (mesmo valor; hex lowercase). Logar qual foi aceito; se ambos presentes, **priorizar `Idempotency-Key`** e espelhar no outro.
* **Retenção de idempotência**: armazenar `idempotency_key` por **≥ `3 _days`**; replays **200** com corpo **idêntico** e header **`X-CE-Dedup-Hit: true`**.
* **HTTP backoff** (5xx/timeouts): **exponencial com jitter** `initial=2s`, `factor=2`, `jitter=±20%`, `max_interval=60s`, `cutoff=21600 _seconds`.
* **Mapeamento de status (provider → interno)**

  | Provider Status   | Interno     | Observações                |
  | ----------------- | ----------- | -------------------------- |
  | `PIX_SETTLED`     | `CONFIRMED` | liquidação instantânea     |
  | `PIX_PENDING`     | `PENDING`   | aguarda confirmação        |
  | `CARD_AUTH_ONLY`  | `PENDING`   | risco de reversão          |
  | `CARD_SETTLED`    | `CONFIRMED` | D+0/D+1 conforme arranjo   |
  | `CARD_CHARGEBACK` | `FAILED`    | falha/estorno              |
  | `BANK_RETURNED`   | `FAILED`    | devolução bancária         |
  | `CANCELLED`       | `CANCELLED` | cancelamento pelo provedor |

### Segurança & Observabilidade

* Logs/eventos **assinados** (KMS em prod); RBAC completo (viewer, kyc\_reader, kyc\_admin, banking\_admin, protocol\_admin, security\_auditor).
* **Tempo & IDs**: NTP obrigatório; **`clock_drift_max_seconds ≤ 2`**; **UUIDv7** com monotonicidade local.
* **Ingestão de eventos (aceitação):** `max_event_age_seconds = 86400`, `max_event_future_skew_seconds = 5`, **`max_event_size_bytes = 65536`**; fora dos limites → **HTTP 422** (age/skew) ou **HTTP 413** (size); não retentar 4xx.
* **Retenção de eventos**: **30 \_days (quente)** + **12 \_months (frio)** com compressão **gzip** (NDJSON) e ciclo de vida; forense ≥ 12 meses.
* **Semântica de HTTP (webhooks/eventos)**: **2xx = ack**; **4xx = erro permanente**; **5xx = erro transitório**.
* **DLQ & reentrega** — **Eventos internos**: DLQ `ttl_days=3`, máx tentativas **20**. **Webhooks externos**: DLQ `ttl_days=7`, alerta após **3** falhas.
* **Incidentes (SEV/RTO/RPO)**:

  * **SEV‑1**: **RTO `14400 _seconds` / RPO `900 _seconds`**
  * **SEV‑2**: **RTO `28800 _seconds` / RPO `1800 _seconds`**
  * **SEV‑3**: **RTO `86400 _seconds` / RPO `86400 _seconds`**
* **Guardrails de protocolo**: R1→`Pausable` (manual), R2→`Timelock`, R3→`DAO`.
* **Janelas de telemetria (canônicas)**: `telemetry_window_seconds = [120, 300]` (caps de reemissão; máx **6/h** por `oracle_id`).
* **Heartbeats (eventos a partir de R1)**:

  * `OracleHeartbeatWarned{oracle_id, threshold_seconds, last_beat_ts}` ao cruzar `elapsed ≥ floor(0.8 * liveness_seconds)`;
  * `OracleHeartbeatMissed{oracle_id, threshold_seconds, last_beat_ts}` ao cruzar `elapsed ≥ liveness_seconds`.

### UX

* Internacionalização **EN/PT**.
* **Acessibilidade AA (WCAG 2.1)** — DoD: foco visível, **contraste ≥ 4.5:1**, navegação por teclado, rótulos ARIA, **mensagens de erro associadas** aos campos e **`role=alert`** por campo em erros.

---

## 🟠 Release 2 (R2)

#### Faixas de Colateral (R2)

* **Parâmetro de corte**: `collateral_small_crypto_threshold_cent = 2500000` (R\$ 25.000,00).
* Se `collateral_value_cent ≤ collateral_small_crypto_threshold_cent` → **130%**; caso contrário → **105%**.
* **Fiat → 100%**.
* Reforçar reavaliações: **`1 _days` (cripto) / `7 _days` (fiat)** e **política reativa** (alerta ≥ 1 janela → liquidação parcial/bloqueio de saques até recomposição).

### Token & Colateral

* **Oráculos CE\$ (ADR‑004)**: quórum **2/3**, **agregador = mediana**, **liveness: `93600 _seconds` (cripto) / `691200 _seconds` (fiat)**, **peg\_unit: 'BRL'**.
  Evento `OracleUpdate{ts_utc, providers[], median, deviation_bps, liveness_seconds, twap_window_seconds, peg_unit, chain_id, network, twap_unavailable, proof, signatures[], aggregator_sig}` *(cada item em `signatures[]` = `{provider, key_id, signature}`)*.
  **Fórmula `deviation_bps`**: `round_half_up( abs(median/peg_par_value - 1) * 10000 )`; `peg_par_value = 1.0` quando `peg_unit` coincide com a moeda de paridade.
  **Staleness**: se `now - last_update > liveness_seconds` → **Pausable** para **saques/devoluções CE\$ e criação de loans** lastreados; alertar Security/Orchestrator.
  **Depeg (observe\_only)**: `warn_if deviation_bps ≥ 50` por ≥ **`10 _seconds`**; `pause_if deviation_bps ≥ 100` por ≥ **`60 _seconds`**.
  **TWAP**: `twap_window_seconds ∈ {300, 1800}`; se `median` fora do **IQR** das fontes → `outlier=true` e `outlier_score` em telemetria.
  **FX quando `currency != peg_unit`**: exigir `fx_oracle_id` e política de fallback.

* **Reavaliação periódica** conforme acima; **política reativa**: alerta ≥ 1 janela → **liquidação parcial** e/ou **bloqueio de novos saques** até recomposição.

* **Novos colaterais**: cripto grande/pequena; stablecoins adicionais.

### Risco & Score

* Integrações: **Open Banking**, **utilities**, **telecom**.
* **Reputação on‑chain**: 3 badges mínimos (pagador pontual, recorrente, volume); **`badge_ttl_days = 365 _days`**; **grace** ±`1 _days`; eventos `BadgeGranted` / `BadgeExpired` com `proof`.

### Governança

* Comitê de risco **consultivo** inicial.
* **Parâmetros votáveis**: `min_apr_365_bps`, `offer_ttl_seconds`, `max_offers_per_lender_per_auction`, `min_step_bps` (**casar com ADR‑005**).
* **Votáveis (risco/oráculos)**: `depeg_warn_bps=50`, `depeg_pause_bps=100`, `twap_window_seconds=1800`, `oracle_liveness_crypto_seconds=93600`, `oracle_liveness_fiat_seconds=691200`, `max_oracle_skew_bps=75`.
* **Timelock**: `param_change_timelock_seconds = 86400` *(exceção **hotfix** sujeita a veto de Security; `hotfix_max_duration_seconds = 3600`)*.

### UX & Painéis

* Painéis avançados: **Funding Velocity (R\$/h)**; **APR\_252\_bps vs CDI\_252\_bps (Δ\_bps)** — horas com **2 casas decimais**.
* Mobile‑first refinado.

---

## 🔵 Release 3 (R3)

### Expansão Global & Multimoeda

* **Livros segregados por moeda** (BRL, USD, EUR, stablecoins globais) e **oráculo FX dedicado**.
* **Política de arredondamento por moeda** (minor units) e **`currency` obrigatório** em **todos os eventos/fluxos financeiros** com valores.

### Scores Internacionais

* Bureaus globais e **reputação cross‑chain**.

### Governança

* **DAO** plena para parâmetros críticos; módulo de propostas e votação on‑chain.

### Mercado Secundário

* Negociação de dívidas fracionadas; **eventos** `DebtListed` e `DebtTraded`.
* Liquidez contínua (modelo “quanto pagar por cada R\$ 1”).

### Segurança Avançada

* **Zero‑trust**: mTLS entre serviços; rotação de secrets; KMS para assinatura/storage; least‑privilege com revisão trimestral.
* **SLA ≤ `21600 _seconds`** para **notificações de inadimplência** e evento **`DefaultNotified{loan_id, dpd_days, amount_minor, currency, minor_unit_dp}`**.

---

## 📡 Eventos mínimos por Release (NDJSON, Envelope A)

> **Envelope A (canônico)**: `{ type, ts_utc, payload, payload_hash, signature, event_id, schema_version }`
> **Canonicalização/Hash/Assinatura**: **JCS (RFC 8785)** → **SHA‑256(JCS(payload)) (hex lowercase)** → **ECDSA\_P256\_SHA256 (signature base64 DER)**.
> **Entrega fora de ordem & replays**: **tolerar** chegada fora de ordem e replays; aplicar **LWW** com `ts_utc` e `event_id` (UUIDv7). Em replays **idênticos**, responder com **o mesmo corpo** e header **`X-CE-Dedup-Hit: true`**.
> **Restrição de schema**: Schemas 1.0.0 definem `additionalProperties=false` para `payload`.
> **Campos adicionais obrigatórios**: `event_id` (**UUIDv7**), `schema_version` (ex.: `1.0.0`), `day_count` (**ACT/365F** quando aplicável), `currency` quando houver valores.

* **MVP**: `AuctionCreated`, `Offer{status∈[PLACED|UPDATED|CANCELLED]}`, `LoanConfirmed`, `AuctionExtended{auction_id, prev_expiry_ts, new_expiry_ts, extended_by_seconds, reason}`.
* **R1**: + `FiatCallback{payment_id, provider_id, idempotency_key, status, amount_cent, currency}` (**assinado; idempotência `sha256(provider_id + payment_id)` — hex lowercase; header aceito: `Idempotency-Key` ou `CE-Idempotency-Key`**), `KYCReadAudit{who, subject_id, purpose}`, `LoanPrepaid{principal_pago_cent, juros_pro_rata_cent, saldo_cent, currency, apr_365_bps, day_count}`, `OracleHeartbeatWarned{oracle_id, threshold_seconds, last_beat_ts}`, `OracleHeartbeatMissed{oracle_id, threshold_seconds, last_beat_ts}`.
* **R2**: + `OracleUpdate{...}`, `OracleStale{oracle_id,last_update,liveness_seconds}`, `OracleSkewDetected{deviation_bps}`, `CollateralRevalued`, `BadgeGranted{address,badge,issued_at,expires_at,proof}`, `BadgeExpired{address,badge,expires_at,proof}`, `OfferExpired{offer_id, auction_id, lender_id, expired_at_ts}`.
* **R1+ (opcional PROD, assinado)**: `KYCDataDeleted{subject_id, deleted_at_ts, basis}`.

---

## ✅ Critérios de decisão por Release (gates)

* **Definição formal — Funding P95**: P95 de `(t1 − t0)` com **`t0 = ts(AuctionCreated)`** e **`t1 = ts(LoanConfirmed)`**; **excluir** pedidos `AUTO_CANCELLED`; **janela móvel: `30 _days`**. *Ambiente novo*: **burn‑in 3 \_days**.

* **Definição formal — Pool (canônica)**: `Pool = Σ(notional_i * funded_flag_i) / Σ(notional_i)` na **janela móvel de `30 _days`** (métrica em UTC).

* **Definição formal — Yield (gross vs net)**:
  `APR_252 = (1+APR)^(252/365) − 1`
  `Yield_gap_gross_bps = APR_252 − CDI_252`
  **`Yield_gap_net_bps = (APR_252 − 50_bps) − CDI_252`** *(taxa ADR‑002)*

* **MVP (Gate M0)** — **Funcional**: BL‑001/002/007/009; anti‑sniping `observe_only`; fallback `ON_HOLD/AUTO_CANCELLED`.
  **KPIs**: **Funding P95 ≤ `86400 _seconds`**; **Pool ≥ 65%**; **Yield\_gap\_net\_bps ≥ 150**.
  **Segurança**: tamper test; assinatura **ECDSA\_P256**; RBAC básico.

* **R1 (Gate R1)** — **Funcional**: Banking (conciliação + callbacks ≤ `21600 _seconds`), KYC PJ, logs KMS.
  **KPIs**: **Funding P95 ≤ `64800 _seconds`**; **Pool ≥ 70%**; **0 SEV‑1**.
  **Segurança**: RBAC completo; auditoria de leitura; **backup + restore** ok.

* **R2 (Gate R2)** — **Funcional**: Oráculos 2/3 (mediana) **com telemetria de depeg/skew e pausa por staleness**, reavaliação com **política reativa**; reputação on‑chain (3 badges + eventos); governança de parâmetros; **enforcement anti‑manipulação e mínimos por oferta**.
  **KPIs**: **Funding P95 ≤ `43200 _seconds`**; **Pool ≥ 75%**; **0 SEV‑1/2**.
  **Segurança**: alertas de liveness; rotação de chaves KMS.

* **R3 (Gate R3)** — **Funcional**: **multimoeda** (livros + FX), **secundário** (DebtListed/Traded), **DAO**.
  **KPIs**: **Funding P95 ≤ `28800 _seconds`**; **Pool ≥ 80%**; **Liquidez secundária ≥ 30%** do estoque/mês = `(sum(TradedNotionalMonth) / OutstandingPrincipalStartOfMonth)` **excluindo primário e wash trades**.
  **Segurança**: zero‑trust; PEP/sanções globais.

---

## ✅ Critérios de validação (geral)

Cada Sprint/Release encerra com:

* Testes unitários + integração + E2E (DoD por módulo).
* **Eventos com hash + assinatura** (Envelope A) publicados no feed imutável. **Webhooks OUTBOUND** incluem `Content-Digest`; **INBOUND** validam **HMAC** e registram digest internamente se ausente.
* **KPIs atingidos** na janela de medição do Release (**`30 _days`**).
* **Registro no `decision_log.md`** (`SprintClosed` / `ReleaseClosed`).
* **Widget APR média (bps)** único a partir de `LoanConfirmed.apr_weighted_bps` (**APR base 365**) com conversão **APR→252** validada.

---

## 📌 Notas

* Roadmap sujeito a ajustes por ADRs e decisões do PO.
* Creative Process pode propor alternativas; Orchestrator consolida.
* Security tem poder de veto em caso de risco crítico.
* **Compat ADR‑005 (anti‑sniping)**: MVP adota **uma extensão total por leilão**; desvio registrado no `decision_log.md` e **feature‑flag** para rollback/A‑B em DEV.
* **Compat de Envelope (DEV)**: aceitar eventos **sem `event_id`/`schema_version`** somente em **DEV**, com header **`CE-Unsafe-Envelope: true`** e *warning*; deprecar até *code‑freeze* de R1.
* **SemVer & deprecação**: **MAJOR** quebra; **MINOR** campos opcionais; **PATCH** correção. **Janela de deprecação ≥ 60 \_days** após anúncio no feed canônico.

---

## 📐 Invariantes normativas & edge‑cases (MVP→R3)

1. **Pró‑rata (BL‑002)**: método dos maiores restos; soma final **==** `total_amount_cent`.
2. **Faixa de APR**: `min_apr_365_bps ≤ apr_365_bps ≤ max_apr_365_bps`; **R2+**: rejeitar fora da faixa. **R1**: logar telemetria.
3. **Extensão de leilão**: `new_expiry ≤ original_expiry + 600s`; sempre emitir `AuctionExtended{...}` quando `extended_by_seconds>0`.
4. **TTLs**: estender `auction_expiry` **não altera** `offer_ttl_seconds` já emitidos; novas ofertas **herdam** `auction_expiry` vigente.
5. **Widget APR**: única fonte `LoanConfirmed.apr_weighted_bps` (ponderado por centavos; **round half‑up**; **APR base 365**). **Proibidas** outras médias na UI.
6. **Composition hash**: `composition` = array ordenado por `(lender_id ASC, apr_365_bps ASC, amount_cent DESC)` com itens `{lender_id, amount_cent, apr_365_bps}`; `composition_hash_hex = sha256(JCS(composition))` **hex lowercase**; deve **bater** com o payload em `LoanConfirmed`. `lender_id` **único** por composição.
7. **UUIDv7 & tempos**: UUIDv7 com monotonicidade local; `ts_utc` ISO‑8601 UTC (**sufixo Z**); assinatura sobre **JCS(payload)**; **`clock_drift_max_seconds ≤ 2`** com NTP obrigatório.
8. **Funding Velocity (R\$/h)**: `sum(confirmed_amount_cent)/100 / horas_decorridas_no_dia` (métrica em UTC; exibir no fuso do usuário). Arredondar horas com **2 casas decimais**.
9. **CDI\_252**: **dev/test** usar `mock_cdi_252_bps`; **prod** usar feed `oracles.cdi` com `liveness_seconds = 93600` e fallback manual com timelock.
10. **Secundário (R3)**: `price_pct_bps` inteiro em **bps**; ex.: **9500 = 95,00%**.
11. **Staleness de oráculo**: `now - last_update ≤ liveness_seconds`; violado → **Pausable** e `OracleStale{...}`.
12. **Skew primário×TWAP**: `|median - twap| ≤ max_oracle_skew_bps` **SHOULD**; excedido → `OracleSkewDetected{deviation_bps}` e **freeze** de avaliações não críticas até confirmação (R2) ou auto‑pause (R3).
13. **Assinaturas (`OracleUpdate`)**: cada `signatures[]` com `{provider, key_id, signature}` + **`aggregator_sig`**.
14. **Dedup por `event_id`**: produtores **MUST** não reutilizar; consumidores **MUST** deduplicar por `event_id` em **`30 _days`**, retornando mesmo corpo para replays idênticos **+ `X-CE-Dedup-Hit: true`**.
15. **Minor units (R3)**: definir `minor_unit_dp` por moeda; eventos multimoeda: usar `*_minor` + `minor_unit_dp`. BRL: campos `*_cent`; on‑chain: `*_wei`.
16. **Clearing**: somente com ofertas **não expiradas** no instante do `LoanConfirmed`.
17. **Ranges secundário**: `1 ≤ price_pct_bps ≤ 20000` (1%–200%); rejeitar fora (R3+).
18. **Conversão APR→252 — referência**: `apr252_bps = floor( ((1+APR)^(252/365) - 1) * 10000 + 0.5 )`.
19. **Enums canônicos**: `AuctionExtended.reason ∈ {AUTO_SNIPING, MANUAL_OPERATOR, SYSTEM_HEALTH}`; se `MANUAL_OPERATOR`, registrar `operator_id` no log interno.
20. **Offer.UPDATED (R2+)**: **apenas reduções** de `apr_365_bps`; aumentos **rejeitados** (salvo feature‑flag emergencial).
21. **Max offers por lender/auction (R2+)**: `max_offers_per_lender_per_auction = 3` (enforcement; rejeitar a 4ª+).

---

## 🔧 Feature flags (canônico)

| Flag                                                 | Default MVP | R1    | R2+ (enforcement)  | Observações                                                 |
| ---------------------------------------------------- | ----------- | ----- | ------------------ | ----------------------------------------------------------- |
| anti\_sniping.single\_extension                      | true        | true  | true/patch ADR‑005 | Única extensão total por leilão                             |
| protocol.observe\_only                               | true        | true  | false              | Telemetria sem bloqueio                                     |
| risk.min\_step\_bps\_enforce                         | false       | false | true               | `min_step_bps=5`                                            |
| risk.max\_offers\_per\_lender\_per\_auction\_enforce | false       | false | true               | máx. **3** por lender/auction                               |
| risk.cooldown\_cancel\_enforce                       | false       | false | true               | `cooldown_cancel_seconds=60`                                |
| risk.max\_cancels\_per\_5min\_per\_lender\_enforce   | false       | false | true               | `max_cancels_per_5min_per_lender=1`                         |
| banking.idempotency\_header\_mirror                  | true        | true  | true               | Aceitar `Idempotency-Key`; espelhar em `CE-Idempotency-Key` |
| offers.updated\_allow\_increase                      | true        | true  | false              | R2+: **apenas reduções** de APR                             |

---

## 📎 Apêndice (referências rápidas)

* **Parâmetros `observe_only` (R1)**: `min_delta_bps=5`, `min_change_interval_seconds=30`, `telemetry_window_seconds=[120,300]`, `rate_limit_offers_per_lender_per_minute=6`.
* **Enforcement (R2/BL‑003)**: `min_step_bps=5`, `max_offers_per_lender_per_auction=3`, `cooldown_cancel_seconds=60`, `max_cancels_per_5min_per_lender=1`, anti‑sniping **uma** extensão total.
* **Badges (R2)**: `badge_ttl_days = 365 _days` (+ **grace ±`1 _days`**); eventos `BadgeGranted`/`BadgeExpired`.
* **Multimoeda (R3)**: `currency` obrigatório (ISO‑4217 ou ticker on‑chain), **minor\_unit\_dp** por moeda e arredondamento por minor units.
* **Fórmulas**: `APR_252 = (1+APR)^(252/365) − 1`; `Yield_gap_gross_bps = APR_252 − CDI_252`; **`Yield_gap_net_bps = (APR_252 − 50_bps) − CDI_252`**.
* **Day count**: `ACT/365F`.
* **FX (R3+)**: quando houver conversão, registrar `fx_rate_source` e `fx_ts_utc` no evento afetado.
* **Arredondamento (APR média)**: **round half‑up** (*0,5 sobe*). `round_half_up(x_bps) = floor(x_bps + 0.5)`.

---

### C) Schemas — mínimos do MVP (1.0.0)

> Mantidos e **especificados**: AuctionCreated (com `apr_min_365_bps`), Offer, LoanConfirmed, AuctionExtended; todos com `event_id`, `schema_version`, `payload_hash` (hex lowercase) e assinatura ECDSA\_P256. `additionalProperties=false` em `payload`.

#### 1) `schemas/AuctionCreated/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/AuctionCreated/1.0.0/schema.json",
  "title":"AuctionCreated/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"AuctionCreated"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["auction_id","notional_cent","currency","apr_min_365_bps","expiry_ts"],
      "properties":{
        "auction_id":{"type":"string"},
        "notional_cent":{"type":"integer","minimum":1},
        "currency":{"type":"string"},
        "apr_min_365_bps":{"type":"integer"},
        "expiry_ts":{"type":"string","format":"date-time"}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 2) `schemas/Offer/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/Offer/1.0.0/schema.json",
  "title":"Offer/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"Offer"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["offer_id","auction_id","lender_id","amount_cent","apr_365_bps","status"],
      "properties":{
        "offer_id":{"type":"string"},
        "auction_id":{"type":"string"},
        "lender_id":{"type":"string"},
        "amount_cent":{"type":"integer","minimum":1},
        "apr_365_bps":{"type":"integer"},
        "status":{"type":"string","enum":["PLACED","UPDATED","CANCELLED"]}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 3) `schemas/LoanConfirmed/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/LoanConfirmed/1.0.0/schema.json",
  "title":"LoanConfirmed/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"LoanConfirmed"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["loan_id","auction_id","amount_cent","currency","apr_weighted_bps","composition_hash_hex","composition","day_count"],
      "properties":{
        "loan_id":{"type":"string"},
        "auction_id":{"type":"string"},
        "amount_cent":{"type":"integer","minimum":1},
        "currency":{"type":"string"},
        "apr_weighted_bps":{"type":"integer"},
        "composition_hash_hex":{"type":"string","pattern":"^[a-f0-9]{64}$"},
        "composition":{
          "type":"array",
          "minItems":1,
          "items":{
            "type":"object",
            "required":["lender_id","amount_cent","apr_365_bps"],
            "properties":{
              "lender_id":{"type":"string"},
              "amount_cent":{"type":"integer","minimum":1},
              "apr_365_bps":{"type":"integer"}
            },
            "additionalProperties":false
          }
        },
        "day_count":{"type":"string","const":"ACT/365F"}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 4) `schemas/AuctionExtended/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/AuctionExtended/1.0.0/schema.json",
  "title":"AuctionExtended/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"AuctionExtended"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["auction_id","prev_expiry_ts","new_expiry_ts","extended_by_seconds","reason"],
      "properties":{
        "auction_id":{"type":"string"},
        "prev_expiry_ts":{"type":"string","format":"date-time"},
        "new_expiry_ts":{"type":"string","format":"date-time"},
        "extended_by_seconds":{"type":"integer","minimum":1},
        "reason":{"type":"string","enum":["AUTO_SNIPING","MANUAL_OPERATOR","SYSTEM_HEALTH"]}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

---

### D) Schemas adicionais (1.0.0) — LoanPrepaid, Oracles, Badges, Secondary, Default, Callbacks/Audit, **KYCDataDeleted**

> Mesmo Envelope A dos demais (`type`, `ts_utc`, `payload`, `payload_hash`, `signature`, `event_id`, `schema_version`). Todos com `additionalProperties=false`.

#### 1) `schemas/LoanPrepaid/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/LoanPrepaid/1.0.0/schema.json",
  "title":"LoanPrepaid/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"LoanPrepaid"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["loan_id","principal_pago_cent","juros_pro_rata_cent","saldo_cent","currency","apr_365_bps","day_count"],
      "properties":{
        "loan_id":{"type":"string"},
        "principal_pago_cent":{"type":"integer","minimum":0},
        "juros_pro_rata_cent":{"type":"integer","minimum":0},
        "saldo_cent":{"type":"integer","minimum":0},
        "currency":{"type":"string"},
        "apr_365_bps":{"type":"integer"},
        "day_count":{"type":"string","const":"ACT/365F"}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 2) `schemas/OracleUpdate/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/OracleUpdate/1.0.0/schema.json",
  "title":"OracleUpdate/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"OracleUpdate"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["providers","median","deviation_bps","liveness_seconds","twap_window_seconds","peg_unit","chain_id","network","twap_unavailable","signatures","aggregator_sig"],
      "properties":{
        "providers":{"type":"array","items":{"type":"string"},"minItems":2},
        "median":{"type":"number"},
        "deviation_bps":{"type":"integer","minimum":0},
        "liveness_seconds":{"type":"integer","minimum":1},
        "twap_window_seconds":{"type":"integer","enum":[300,1800]},
        "peg_unit":{"type":"string"},
        "chain_id":{"type":"integer","minimum":1},
        "network":{"type":"string"},
        "twap_unavailable":{"type":"boolean"},
        "proof":{"type":"string"},
        "signatures":{"type":"array","minItems":2,"items":{"type":"object","required":["provider","key_id","signature"],"properties":{"provider":{"type":"string"},"key_id":{"type":"string"},"signature":{"type":"string"}},"additionalProperties":false}},
        "aggregator_sig":{"type":"string"}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 3) `schemas/OracleStale/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/OracleStale/1.0.0/schema.json",
  "title":"OracleStale/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"OracleStale"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["oracle_id","last_update","liveness_seconds"],
      "properties":{
        "oracle_id":{"type":"string"},
        "last_update":{"type":"string","format":"date-time"},
        "liveness_seconds":{"type":"integer","minimum":1}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 4) `schemas/OracleSkewDetected/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/OracleSkewDetected/1.0.0/schema.json",
  "title":"OracleSkewDetected/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"OracleSkewDetected"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["deviation_bps"],
      "properties":{"deviation_bps":{"type":"integer","minimum":0}},
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 5) `schemas/OracleHeartbeatWarned/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/OracleHeartbeatWarned/1.0.0/schema.json",
  "title":"OracleHeartbeatWarned/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"OracleHeartbeatWarned"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["oracle_id","threshold_seconds","last_beat_ts"],
      "properties":{
        "oracle_id":{"type":"string"},
        "threshold_seconds":{"type":"integer","minimum":1},
        "last_beat_ts":{"type":"string","format":"date-time"}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 6) `schemas/OracleHeartbeatMissed/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/OracleHeartbeatMissed/1.0.0/schema.json",
  "title":"OracleHeartbeatMissed/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"OracleHeartbeatMissed"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["oracle_id","threshold_seconds","last_beat_ts"],
      "properties":{
        "oracle_id":{"type":"string"},
        "threshold_seconds":{"type":"integer","minimum":1},
        "last_beat_ts":{"type":"string","format":"date-time"}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 7) `schemas/BadgeGranted/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/BadgeGranted/1.0.0/schema.json",
  "title":"BadgeGranted/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"BadgeGranted"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["address","badge","issued_at","expires_at","proof"],
      "properties":{
        "address":{"type":"string"},
        "badge":{"type":"string","enum":["ON_TIME_PAYER","RECURRENT_BORROWER","VOLUME_TIER"]},
        "issued_at":{"type":"string","format":"date-time"},
        "expires_at":{"type":"string","format":"date-time"},
        "proof":{"type":"string"}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 8) `schemas/BadgeExpired/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/BadgeExpired/1.0.0/schema.json",
  "title":"BadgeExpired/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"BadgeExpired"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["address","badge","expires_at","proof"],
      "properties":{
        "address":{"type":"string"},
        "badge":{"type":"string","enum":["ON_TIME_PAYER","RECURRENT_BORROWER","VOLUME_TIER"]},
        "expires_at":{"type":"string","format":"date-time"},
        "proof":{"type":"string"}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 9) `schemas/DebtListed/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/DebtListed/1.0.0/schema.json",
  "title":"DebtListed/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"DebtListed"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["listing_id","amount_minor","price_pct_bps","currency","minor_unit_dp"],
      "properties":{
        "listing_id":{"type":"string"},
        "amount_minor":{"type":"integer","minimum":1},
        "price_pct_bps":{"type":"integer","minimum":1},
        "currency":{"type":"string"},
        "minor_unit_dp":{"type":"integer","minimum":0}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 10) `schemas/DebtTraded/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/DebtTraded/1.0.0/schema.json",
  "title":"DebtTraded/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"DebtTraded"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["trade_id","listing_id","amount_minor","price_pct_bps","currency","minor_unit_dp"],
      "properties":{
        "trade_id":{"type":"string"},
        "listing_id":{"type":"string"},
        "amount_minor":{"type":"integer","minimum":1},
        "price_pct_bps":{"type":"integer","minimum":1},
        "currency":{"type":"string"},
        "minor_unit_dp":{"type":"integer","minimum":0}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 11) `schemas/DefaultNotified/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/DefaultNotified/1.0.0/schema.json",
  "title":"DefaultNotified/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"DefaultNotified"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["loan_id","dpd_days","amount_minor","currency","minor_unit_dp"],
      "properties":{
        "loan_id":{"type":"string"},
        "dpd_days":{"type":"integer","minimum":0},
        "amount_minor":{"type":"integer","minimum":1},
        "currency":{"type":"string"},
        "minor_unit_dp":{"type":"integer","minimum":0}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 12) `schemas/FiatCallback/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/FiatCallback/1.0.0/schema.json",
  "title":"FiatCallback/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"FiatCallback"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["payment_id","provider_id","idempotency_key","status","amount_cent","currency"],
      "properties":{
        "payment_id":{"type":"string"},
        "provider_id":{"type":"string"},
        "idempotency_key":{"type":"string","pattern":"^[a-f0-9]{64}$"},
        "status":{"type":"string","enum":["PENDING","CONFIRMED","FAILED","CANCELLED"]},
        "amount_cent":{"type":"integer","minimum":0},
        "currency":{"type":"string"}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 13) `schemas/KYCReadAudit/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/KYCReadAudit/1.0.0/schema.json",
  "title":"KYCReadAudit/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"KYCReadAudit"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["who","subject_id","purpose"],
      "properties":{
        "who":{"type":"string"},
        "subject_id":{"type":"string"},
        "purpose":{"type":"string","enum":["FRAUD_REVIEW","CUSTOMER_SUPPORT","LEGAL_REQUEST","AUDIT","OTHER"]}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 14) `schemas/OfferExpired/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/OfferExpired/1.0.0/schema.json",
  "title":"OfferExpired/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"OfferExpired"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["offer_id","auction_id","lender_id","expired_at_ts"],
      "properties":{
        "offer_id":{"type":"string"},
        "auction_id":{"type":"string"},
        "lender_id":{"type":"string"},
        "expired_at_ts":{"type":"string","format":"date-time"}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```

#### 15) `schemas/KYCDataDeleted/1.0.0/schema.json`

```json
{
  "$schema":"https://json-schema.org/draft/2020-12/schema",
  "$id":"https://creditengine/schemas/KYCDataDeleted/1.0.0/schema.json",
  "title":"KYCDataDeleted/1.0.0",
  "type":"object",
  "required":["type","ts_utc","payload","payload_hash","signature","event_id","schema_version"],
  "properties":{
    "type":{"const":"KYCDataDeleted"},
    "ts_utc":{"type":"string","format":"date-time"},
    "event_id":{"type":"string","description":"UUIDv7"},
    "schema_version":{"type":"string","const":"1.0.0"},
    "payload_hash":{"type":"string","pattern":"^[a-f0-9]{64}$"},
    "signature":{"type":"string"},
    "payload":{
      "type":"object",
      "required":["subject_id","deleted_at_ts","basis"],
      "properties":{
        "subject_id":{"type":"string"},
        "deleted_at_ts":{"type":"string","format":"date-time"},
        "basis":{"type":"string","enum":["RETENTION_POLICY","DATA_SUBJECT_REQUEST","LEGAL_REQUIREMENT","OTHER"]}
      },
      "additionalProperties":false
    }
  },
  "additionalProperties":false
}
```
