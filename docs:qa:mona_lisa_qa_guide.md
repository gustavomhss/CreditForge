# KB Master Audit & Enhancement Plan — “Mona Lisa” Edition

Este documento é o Guia de QA da KB. Ele define os padrões de qualidade e critérios de aceite globais que todos os artefatos desta base (catálogo, features, roadmap, top100, etc.) devem obedecer.

> **Objetivo:** Fazer um deepdive extremo em todo o material (Product Map v5.8 + Feature Index + Roadmap vNext + Top100 template + IID feature), identificar **lacunas**, **riscos**, **inconsistências** e **oportunidades de perfeição**, e entregar **patches cirúrgicos** prontos para aplicar. Este arquivo é o *guia de curadoria final* — alto padrão, critérios de aceite e convenções canônicas.  
> **Regra de ouro:** nada entra sem rastreabilidade (FEAT‑ID), critério de aceite testável e contrato de dados explícito.

---

## 0) Sumário executivo (estado atual → alvo)
- **Cobertura**: Feature Index agora cobre 100+ features (001→100); Roadmap vNext define 7 fases com gates; IID especificada; Top100 pronto.
- **Alvo**: padronizar **contratos**, **eventos**, **métricas**, **NFRs**, **convenções** e **fórmulas financeiras**; fechar buracos de compliance; introduzir invariantes e *runbooks* operacionais.

**Top 10 patches (alta prioridade):**
1. **Contratos de dados canônicos (JSON Schema) por domínio.**
2. **Invariantes financeiras** (rounding, day count, ordem de cálculo, timezone) para fees/waterfall.
3. **Catálogo de eventos** (dicionário + versionamento) com IDs, semântica, e *idempotency rules*.
4. **Benchmark & HWM** — metodologia, frequência, fontes e fórmulas fechadas.
5. **Suitability & Guardrails** — matriz de bloqueio por perfil/risco por classe de ativo.
6. **Política de reconciliação** (aceitável = 0, exceções e runbook) + *reversal mirrors*.
7. **Segurança transversal**: RBAC granular, segredo HMAC com *rotation cadence*, *proof of delivery* dos webhooks.
8. **NFRs por domínio** com SLOs + *error budgets* + playbooks.
9. **Tax/Withholding (base)** — regras, fontes, relatórios, calendários de mercado.
10. **Governança**: estrutura de ADR + Decision Log com *templates* e exigência de link FEAT.

---

## 1) Modelo de dados canônico (CDM) — mínimo viável
> **Propósito**: definir entidades e chaves *cross‑feature* para evitar divergência semântica.

**Núcleo (Finance/Core)**
- `Party(id, type[PF|PJ], kyc_status, risk_profile)`
- `Account(id, party_id, kind[bank|virtual|custody|margin], currency, status)`
- `Instrument(id, class[FI|FUND|ETF|FX|DERIV|COE|INS], is_tradable)`
- `Position(id, party_id, instrument_id, qty, nav_px, ts)`
- `CashMovement(id, account_id, direction[in|out], amount_minor, currency, ts, ref)`
- `LedgerEntry(id, debit_account, credit_account, amount_minor, currency, ts, ref, memo)`

**Wealth/IID**
- `StrategyDesk(id, owner_party_id, status)`
- `TermsVersion(id, strategy_id, v, fees, benchmarks, liquidity, whitelist_assets, effective_from)`
- `ShareClass(id, terms_id, code)`
- `InvestorPosition(id, strategy_id, party_id, share_class_id, shares, nav, ts)`
- `FeeRule(id, terms_id, type[perf|mgmt|platform], base[pnl|pnl_above_hwm|interest], rate_bps)`
- `FeeAccrual(id, position_id, period, base_amount_minor, fee_amount_minor, ts)`
- `PayoutBatch(id, n_items, amount_total_minor, currency, status, hash)`

**Payments/Banking**
- `VirtualAccount(id, party_id, label)`
- `SplitRule(id, strategy_id, basis[shares|fixed], precision_mode)`
- `SplitEntry(id, batch_id, party_id, amount_minor)`
- `BankStatement(id, account_id, provider, period, hash)`
- `Reconciliation(id, statement_id, status, diff_minor)`

**Compliance/Security**
- `KycCase(id, party_id, status, risk)`
- `AmlFlag(id, party_id, reason)`
- `AuditLog(id, actor, action, resource, ts, ip, sig)`
- `IdempotencyKey(id, scope, status, first_ts, last_ts)`

**Metadados**: `tenant_id`, `env`, `created_at`, `updated_at`, `version` em todas as entidades persistentes.

---

## 2) Convenções e invariantes (obrigatórias)
**Moeda & precisões**
- Valores monetários em **centavos** (inteiro). **Taxas** em **bps** (inteiro). Proibição de `float` em contabilidade.
- **Rounding**: *bankers rounding* (ou HALF_UP) — **fixar um** e declarar globalmente.

**Datas & contagem de dias**
- Timezone do sistema: **UTC**. *Cutoffs* operacionais: **America/Bahia**.
- Contagem de dias: **BUS/252** para CDI; **ACT/365** para juros simples; declarar por *terms*.

**Ordem de cálculo (waterfall)**
1. Determinar `principal` e `interest` do período.
2. Calcular `fee_perf` (sobre base declarada) → `fee_mgmt` → `fee_platform`.
3. Aplicar **custos operacionais** do período.
4. **Amortizar principal**.
5. Distribuir **juros líquidos** pro‑rata.

**HWM/Benchmark**
- `HWM_i(t) = max(HWM_i(t-1), NAV_i(t))` por investidor.
- `PerfBase = max(0, NAV_i(t) − HWM_i(t-1))` (ou `Retorno − Benchmark` quando aplicável).
- Frequência e defasagem do benchmark documentadas (D‑1, D‑2).

**Idempotência & assinatura**
- Todo endpoint mutável requer `Idempotency-Key` (uuidv7) + `X-Signature: HMAC(v=1, algo=SHA256)`.
- Replays retornam 200 com recurso **imutável** (sem efeitos colaterais).

---

## 3) Catálogo de eventos (canônico)
> **Formato** JSON‑Lines; cada evento contém: `event_id`, `event_type`, `occurred_at`, `tenant_id`, `actor`, `entity`, `idempotency_key`, `hash`, `schema_version`.

**Eventos essenciais**
- `cash_in.created`, `cash_in.reconciled`  
- `split.applied`, `payout.batch_sent`, `payout.item_settled`  
- `fee.accrued`, `fee.paid`  
- `ledger.entry_created` (espelho débito/crédito)  
- `terms.version_applied`, `share_class.issued`  
- `risk.limit_breached`, `risk.limit_cleared`  
- `kyc.status_changed`, `aml.flagged`  
- `webhook.delivery_attempted`, `webhook.delivery_confirmed`

**Versionamento**: `event_type@major.minor` (ex.: `fee.accrued@1.0`). *Breaking changes* sobem **major**.

---

## 4) Padrões de API (REST) — contratos mínimos
**Headers obrigatórios**: `X-Idempotency-Key`, `X-Signature`, `X-Tenant`, `X-Client-Version`.

**Exemplos**
- `POST /desks/{deskId}/close_period` → fecha período e emite `fee_accrued`, `payout_batch_sent`.
- `POST /payouts/batch` → cria lote de pagamentos.  
Body (esqueleto):
```json
{
  "currency":"BRL",
  "items":[{"party_id":"...","amount_minor":970000,"reason":"interest_net","ref":"period:2025-08"}],
  "metadata":{"terms_version":"v1.2.0","desk_id":"..."}
}
```
- `POST /fees/accrue` → `{ position_id, base_minor, rate_bps, period }` retorna `fee_amount_minor` e evento.
- `POST /splits/apply` → `{ batch_id, basis:"shares", precision:"floor|round|bankers" }`.

**Códigos**: 2xx sucesso idempotente; 422 *semantic errors*; 409 conflito de idempotência.

---

## 5) Métricas & NFRs — versão consolidada (alvo inicial)
| Domínio | Disponibilidade | Latência p95 | Throughput base | Observabilidade |
|---|---:|---:|---:|---|
| **Payments** (033/034/005/006) | 99.95% | ≤ 500ms | 200 TPS | tracing + métricas por provedor |
| **Ledger** (017) | 99.99% | ≤ 50ms append | 5k writes/s | auditoria + hash chain |
| **Webhooks** (091/018) | 99.9% | ≤ 3s entrega | 10k ev/min | retries + DLQ + assinatura |
| **Reporting** (013) | 99.9% | ≤ 30s | n/a | jobs observáveis + export logs |
| **Brokerage** (009) | 99.9% | ≤ 200ms ordem | 50 ord/s | slippage monitorado |

**SLO & Error Budgets**: definir por serviço; *burn alerts* automáticos.

---

## 6) Compliance & Regulatórios — mapa mínimo
- **KYC/KYB** (PF/PJ gestores, merchants, investidores) — fonte canônica, periodicidade de revisão.
- **AML/Sanctions/PEP** — política de *hits* e *false positives*.
- **LGPD** — base legal por tratamento, retenção, anonimização, DSAR.
- **CVM/B3/SUSEP/BACEN** — por módulo (Wealth/Insurance/Payments).
- **Contratos** — e‑sign, *terms versioning*, *mandate* discricionário (IID/DPM).
- **Regulatórios** — *reporting cadence* e evidências arquivadas (hash + storage).

**Critérios de aceite (compliance)**
- Checklists por feature **bloqueiam go‑live** sem owner, base legal, DPA/operador e *runbook* de incidentes.

---

## 7) Reconciliação & Contabilidade — invariantes
- Diferença diária aceitável = **R$ 0,00** (exceto ajuste de centavos justificados por *precision mode*).
- **Reversões em espelho**: todo estorno gera `ledger.reverse_of=<id>`.
- **Extratos CNAB/EDI**: *hash* por arquivo + amarração de cada linha a `CashMovement`.

**Testes obrigatórios**
- *Golden datasets* por provedor bancário.  
- Fuzz de idempotência (replays concorrentes).  
- Simulação de *partial payments* e *prepayments*.

---

## 8) Fees & Benchmarks — fórmulas canônicas
**Performance (sem HWM)**: `fee = max(0, base_minor) * rate_bps / 10000`.

**Com HWM (por investidor)**:
```
NAV_t = NAV_{t-1} + cashflows_t + pnl_t
excesso = max(0, NAV_t - HWM_{t-1})
fee = excesso * rate_bps / 10000
HWM_t = max(HWM_{t-1}, NAV_t)
```
**Benchmark (ex.: CDI)**: `ret_bench = exp(taxa_diaria * dias) - 1` (ou linear se definido nos termos).
**Cristalização**: `D+X` após *close*; *accruals* zeradas ao pagar; *events*: `fee.accrued` → `fee.paid`.

---

## 9) Segurança & Acesso
- **RBAC** por *resource + action*; *segregation of duties* em Admin.
- **Secrets**: KMS + rotação trimestral; *dual control* para chaves HMAC.
- **PII**: mascaramento nos logs; *data minimization* por contrato.
- **SSO/MFA** obrigatório para internos; *step‑up auth* para ações sensíveis.

---

## 10) Roadmap vNext — ajustes finos (sem mudar fases)
- Acrescentar *gates de dados*: `JSON Schemas publicados`, `event catalog v1`, `data contracts versionados` nas fases 0–2.
- Fase 3 (IID): *pilot playbook*, *whitelist managers*, *kill‑switch* de estratégias.
- Fase 4 (Brokerage): *best‑execution evidences* + teste de *slippage tolerance*.
- Fase 5 (PSP/Cards): *PCI scope definition* e *3DS metrics* obrigatórias.

---

## 11) Top100 — ajustes metodológicos
- **Double‑blind scoring** (dois avaliadores; divergência >1 ponto → mediação).
- **Gates de parceiro**: sem *letter of intent* → penalidade automática (‑1 no peso de parceiro).
- **Explainability**: cada Top item traz *nota executiva* (<= 240 caracteres) com a razão objetiva do ranking.

---

## 12) UX & Acessibilidade — padrões mínimos
- **WCAG 2.1 AA** para Marketplace/Investor/Manager.
- **Terminologia consistente** com catálogo; *tooltips* e *info icons* para termos técnicos.
- **Comprovantes** exportáveis com hash/ID legível.

---

## 13) Operações — Runbooks & BCDR
- **Runbooks** por domínio (Payments, Ledger, IID, Brokerage), contendo: *detect → diagnose → mitigate → communicate*.
- **BCDR**: RTO/RPO formais; *chaos days* trimestrais.

---

## 14) Governança & Qualidade
- **ADRs** para escolhas irreversíveis; *template* com contexto → forças → decisão → consequências → links para FEAT/decision_log.
- **Definition of Done** (por feature): contratos publicados, eventos gerados, testes, NFRs, compliance, runbook, métricas plugadas.

---

## 15) Patches prontos (aplicar nos arquivos)
- **Feature Index**:
  - adicionar link para **JSON Schemas** por domínio (placeholder `schemas/`),
  - campo `precision_mode` nas features de split/payout,
  - coluna `data_contracts`.
- **Roadmap vNext**: inserir *gates de dados* nas fases 0–2; adicionar *kill‑switch* em IID (fase 3).
- **IID Feature**: seção “**Invariantes e Fórmulas**” (deste doc §2 e §8) + “**Kill‑switch**”.
- **Top100**: adicionar regra de *double‑blind scoring* + campo `justificativa_exec`.

---

## 16) Critérios de aceite (nível KB) — passar = perfeito
1. **Rastreabilidade**: 100% dos artefatos com `FEAT‑ID` e links (Index ↔ Roadmap ↔ Docs).
2. **Contratos**: JSON Schema publicado para todos os payloads críticos (payments, ledger, fees, splits, events).
3. **Eventos**: dicionário v1 com versionamento e idempotência testada.
4. **Fórmulas**: invariantes financeiras codificadas e testadas.
5. **Compliance**: checklists por módulo; bases legais/retention definidas.
6. **NFRs**: SLOs mensuráveis e monitorados.
7. **Runbooks**: publicados e testados (DR, incidentes, reconciliação).
8. **Governança**: ADRs e decision_log atualizados por mudança relevante.

---

## 17) Anexos (exemplos de JSON Schema — esqueleto)
**Evento fee.accrued@1.0**
```json
{
  "$id":"schemas/events/fee.accrued.1.0.json",
  "type":"object",
  "required":["event_id","event_type","occurred_at","tenant_id","position_id","base_minor","rate_bps","fee_amount_minor","schema_version"],
  "properties":{
    "event_id":{"type":"string"},
    "event_type":{"const":"fee.accrued@1.0"},
    "occurred_at":{"type":"string","format":"date-time"},
    "tenant_id":{"type":"string"},
    "position_id":{"type":"string"},
    "base_minor":{"type":"integer"},
    "rate_bps":{"type":"integer"},
    "fee_amount_minor":{"type":"integer"},
    "metadata":{"type":"object"},
    "schema_version":{"type":"string"}
  }
}
```

**Payload /payouts/batch (v1)**
```json
{
  "$id":"schemas/api/payouts.batch.v1.json",
  "type":"object",
  "required":["currency","items"],
  "properties":{
    "currency":{"type":"string"},
    "items":{"type":"array","items":{
      "type":"object","required":["party_id","amount_minor"],
      "properties":{
        "party_id":{"type":"string"},
        "amount_minor":{"type":"integer"},
        "reason":{"type":"string"},
        "ref":{"type":"string"}
      }
    }},
    "metadata":{"type":"object"}
  }
}
```

---

**FIM — Master Audit. Aplicando estes patches, sua KB atinge padrão “PhD” em clareza, governança e precisão.**

