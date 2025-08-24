# CreditEngine\$ — Product Brief (MVP) \[v6.0 — “Perfeita”]

> **Hierarquia documental:** prevalece sempre a versão mais recente promovida a **Master KB** até ADR formal. Master KB atual: **Sanity Check Consolidado v2** \[BK:/masterkb#hierarquia].
>
> **ADRs confirmados e obrigatórios:**
>
> * **ADR‑001** — SLA **default ≤6h** (notificação/execução). \[BK:/governance#adr-001]
> * **ADR‑002** — **Taxa mínima de serviço 0,50%** sobre valor financiado. \[BK:/token#fees]
>
> **Normas CE\$ (unidades, relógio, arredondamento)**
>
> * Taxas: **\_bps**; prazos: **\_days/\_seconds**; valores: **centavos (off‑chain)** / **wei (on‑chain)**. \[BK:/convenções#unidades]
> * Arredondamento: **centavos off‑chain** e **wei on‑chain**; **ordem de operações** definida em §7.1.4.
> * Timestamps: **UTC** nos logs/eventos; exibição em timezone do usuário; auditorias em UTC.
> * Datas financeiras: **APR** como taxa nominal anual base **365 dias**; comparação com CDI em base **252 dias** (ver §10.1 para conversão).

---

## 1. Visão do Produto

Marketplace P2P de crédito com **leilão reverso uniform‑price adaptado CE\$**, **LoanVault** (liquidez até colateral) e **liquidação via CE\$**. Objetivos: **reduzir custo**, **ampliar acesso**, **padronizar risco**. \[BK:/protocol#auction]

---

## 2. Problema

Tomadores: custo efetivo alto, imprevisibilidade, exclusão. Credores: originação despadronizada, risco sem garantias mínimas, difícil judicialização coletiva.

---

## 3. Solução (MVP)

* **Leilão reverso uniform‑price adaptado**: taxa final = **média ponderada** das ofertas aceitas (APR).
* **LoanVault**: liquidação parcial até colateral; recalcula pool e expirações em retomadas. \[BK:/protocol#loanvault]
* **Token CE\$**: lastreado (fiat/cripto), **paridade 1:1** por oráculos; emissão auditada; queima na liquidação. \[BK:/token#paridade]
* **UX 3 telas** + **fallback**: Pedido → Ofertas → Customização (aceite parcial/final); estados `RequestOnHold`/`RequestFilled`/`RequestAutoCancelled` com **SLA ≤2h**. \[BK:/ux#3telas] \[BK:/fallback#fluxo]

---

## 4. Perfis

Tomador PF/PJ; Credor PF/Institucional; Parceiros (score, bancos, antifraude); **Comitê de risco consultivo inicial** (sem poder decisório até descentralização). \[BK:/governance#fase0]

---

## 5. Jornada do Usuário

Publica pedido → credores ofertam → sistema calcula **média ponderada** → tomador aceita parcial/final → LoanVault liquida → (se default) **credores decidem**: abandono, transferência >R\$2k, renegociação, judicialização conjunta (relatório padronizado), venda secundária. \[BK:/protocol#default]

---

## 6. Escopo MVP

Leilão reverso; LoanVault; CE\$; UX 3 telas + fallback; logs imutáveis (hash, JSON/KYC schema); integrações mínimas (score, gateway fiat); Governança Fase 0.

---

## 7. Protocol — Especificação Operacional (Perfeita)

### 7.1 Algoritmo CE\$ (uniform‑price adaptado)

1. **Ordenação** por menor APR; **tie‑breakers**: (i) maior volume, (ii) timestamp mais antigo, (iii) hash do lance.
2. **Aceitação** até 100% do pedido.
3. **Oversubscription** na margem: distribuição **pró‑rata por valor** entre ofertas empatadas/cortadas.
4. **Taxa final (APR\_bps)** = `sum(amount_i_cent * apr_i_bps) / sum(amount_i_cent)` (precisão em centavos).
5. **Eventos** (ver §7.3) registrados com hash.
6. **Transparência**: publicar composição final + `apr_weighted_bps` + `hash_calc` no `LoanConfirmed`.

#### 7.1.1 Anti‑manipulação (parâmetros de governança)

* **Step mínimo de taxa**: **5 \_bps** (parametrizável).
* **Máx. ofertas ativas por credor/auction**: **3**.
* **Cooldown cancelamento**: **60 \_seconds** entre `OfferCancelled`→`OfferPlaced`.
* **Extensão anti‑sniping**: ofertas nos **últimos 120 \_seconds** estendem o fim em **+120 \_seconds** (máx. +600 \_seconds).
* **Proibição de taxa negativa**; **mínimo ≥ 6% a.a.** (Fase 0).
* **Detecção de Sybil** (sinais): KYC/contas bancárias vinculadas, correlação de IP/dispositivo (somente sinal; decisão manual do comitê de risco).

#### 7.1.2 Validade & Reserva

* **TTL** da oferta: **24 \_hours**; expira silenciosamente.
* Reserva de capital: **apenas em `LoanConfirmed`**.
* **Offer updates**: `OfferUpdated` preserva o mesmo `offer_id` com novo hash; aplica cooldown.

#### 7.1.3 Fallback UX

* Estados `RequestOnHold`/`RequestFilled`/`RequestAutoCancelled`; **SLA ≤2h**.
* **Capital não trava**; ao retomar: **recalcular** pool e expirações.
* Mensagens‑modelo (§15‑F).

#### 7.1.4 Ordem de operações & arredondamento

1. Calcular **pró‑rata** em **centavos**.
2. Somar `amount_i_cent` aceitos = **valor do pedido em centavos** (ajuste final ≤1 centavo na última linha).
3. Calcular `apr_weighted_bps` com os valores **após** pró‑rata.
4. Persistir `hash_calc` do array de ofertas aceitas (ordem determinística).
5. Em on‑chain, converter montantes para **wei** (precisão total).

### 7.2 Mercado Secundário

* **Frações**; formato de lance: “**preço por R\$1 de face**”.
* **Passo mínimo**: **R\$0,01** (off‑chain) / **1 wei** (on‑chain).
* Eventos: `DebtAuctionStarted`, `DebtTraded`, `DebtAuctionClosed`.
* **Invariantes**: (i) soma das frações ≤ 100%; (ii) preço ≥ 0; (iii) logs com hash.

### 7.3 Eventos (state machine)

`AuctionCreated` → (`OfferPlaced`|`OfferUpdated`|`OfferCancelled`)\* → `RequestFilled` (opcional) → `LoanPartiallyFilled` (opcional) → `LoanConfirmed` → (`LoanPrepaid`|`LoanDefaulted`|`LoanClosed`).
Fallback: `RequestOnHold`/`RequestAutoCancelled` podem ocorrer em paralelo ao book (sem travar capital).
**Eventos adicionais**: `RepresentationEngaged` (judicialização conjunta).

### 7.4 Política de pré‑pagamento (MVP‑safe)

* **Permitido** a qualquer tempo; **sem multa**.
* Cobrança de **juros pro‑rata die** até a data de liquidação.
* **Taxa de serviço (0,50%)**: aplicada **uma única vez** no desembolso, **não reembolsável**.
* Evento: `LoanPrepaid { principal_pago, juros_pro_rata, saldo }`.

> **Nota**: Mantém simplicidade do MVP e previsibilidade ao tomador (ADR recomendável para formalizar).

---

## 8. Tokenomics — Especificação

* **Colateral**: **130%** cripto pequena; **105%** cripto grande; **100%** fiat. Reavaliação: **24h cripto / 7d fiat**. \[BK:/token#collateral]
* **Paridade 1:1** via **oráculos** (quorum **2/3**; parametrizável).
* **Mint/Burn**: mint no funding (reserva lastro) e **burn** na liquidação/prepagamento.
* **Sem incentivos** (rewards).
* **Monitor de colateral**: alerta se razão < **102%** do alvo (sem *margin call* no MVP — apenas alerta e dashboard).

---

## 9. Risk & Compliance — Especificação

* **PF**: CPF, Receita, listas de sanção; **PEP**; contas bancárias vinculadas.
* **PJ**: CNPJ, representante legal; reforço > R\$50k.
* **Transações atípicas**: limiar inicial **> R\$50k/dia** agregado (CPFs/CNPJs relacionados).
* **Chainalysis** para cripto.
* **Logs KYC/AML**: JSON/KYC schema + hash; **retenção sugerida: 5 anos**; acesso segregado (RBAC); auditoria de leitura.

---

## 10. Métricas & OKRs — Definições e Cálculos

### 10.1 Convenções

* **APR (anual)**: nominal base **365 dias**.
* **CDI (252)**: converter APR→base 252 para comparação: `APR_252 = (1+APR)^(252/365) - 1` (aprox. simples permitido no dashboard).
* **Yield ≥ CDI + 150 \_bps**: `APR_média_confirmada – taxa_serviço` comparada a **CDI\_252**.

### 10.2 KPIs

* **Funding ≤24h**: `AuctionCreated`→`LoanConfirmed`.
* **Pool ≥65%**: aceito/solicitado **antes do aceite do tomador**.
* **NPL30 ≤3%**: principal com atraso >30 \_days / carteira vigente.
* **Ativação lenders D7 ≥40%**; **Retenção D30 ≥60%**.
* **Qualidade do leilão (novos)**: (i) taxa de cancelamento < **15%** por credor/auction; (ii) % de leilões com anti‑sniping < **25%**; (iii) HHI de concentração de funding (meta ≤ 0,35 no MVP).

---

## 11. UX & Acessibilidade

* **3 telas** (Pedido/Ofertas/Customização) + **fallback**; cálculo em tempo real e aceite parcial.
* **Mobile‑first**, EN/PT, ícones claros.
* **Mensagens‑modelo** (Apêndice F).
* **Acessibilidade**: foco visível, contraste AA, navegação por teclado, labels ARIA básicos.

---

## 12. Security & Observabilidade

* Logs/eventos: **JSON** com **SHA‑256 hash** e **assinatura** da plataforma; versionamento de schema (semver).
* **Criptografia em trânsito** (TLS 1.3) e **em repouso** (AES‑256).
* **RBAC**; auditoria de leitura em logs KYC.
* **Backups** diários com verificação de integridade; retenção ≥ 30 \_days.
* **Incidentes**: classificação (SEV‑1..3); SLA de resposta: **SEV‑1 ≤1h**, **SEV‑2 ≤4h**, **SEV‑3 ≤24h**.

---

## 13. Governança & Roadmap

* **Fase 0**: centralizada, **mínimo 6%** juros; **comitê de risco consultivo** (sem poder decisório).
* **Fase 1**: tokenholders definem parâmetros.
* **Fase 2**: comitê tokenizado parcial.
* **Fase 3**: descentralizada.
* **Hierarquia**: Master KB > docs anteriores até ADR novo.

---

## 14. Restrições MVP

SLA fallback ≤2h; SLA default ≤6h (ADR‑001); taxa mínima 0,50% (ADR‑002); sem incentivos; Governança Fase 0.

---

## 15. Tabelas, Simulações, Schemas

### 15‑A Exemplo de taxa média ponderada

3k×10% + 5k×12% + 2k×14% ÷ 10k = **11,8% a.a.** (APR média ponderada). Registrar `hash_calc`.

### 15‑B Pró‑rata na margem

Pedido 10k; ofertas: 6k\@10%, 3k\@11%, 4k\@12% → aceita 6k + 3k + **1k pró‑rata** do último; APR = média ponderada.

### 15‑C Ordem e ajustes de centavos

Distribuir centavos e corrigir **±1** na última linha para fechar o total; persistir composição final.

### 15‑D Schemas JSON mínimos (resumo)

```json
{"AuctionEvent":{"id":"uuid","ts":"utc_iso","type":"string","payload_hash":"hex"}}
```

```json
{"Offer":{"offer_id":"uuid","auction_id":"uuid","lender_id":"uuid","amount_centavos":0,"apr_bps":0,"ts":"utc_iso","status":"PLACED|UPDATED|CANCELLED|EXPIRED"}}
```

```json
{"LoanConfirmed":{"auction_id":"uuid","composition":[{"offer_id":"uuid","amount_centavos":0,"apr_bps":0}],"apr_weighted_bps":0,"hash_calc":"hex"}}
```

```json
{"KYCLog":{"subject_id":"uuid","type":"PF|PJ","checks":["SERASA","PEP","SANCTIONS"],"result":"PASS|REVIEW|FAIL","reviewer":"id","ts":"utc_iso"}}
```

### 15‑E Casos de borda

* TTL expira durante cálculo → remover e recomputar.
* Gateway fiat off → `RequestOnHold` + mensagens.
* Volatilidade cripto → alerta de colateral; permitir editar/cancelar antes do aceite.
* Empates em cadeia → aplicar tie‑breakers em ordem, depois hash.

### 15‑F Mensagens‑modelo (fallback)

* **Tomador**: “Seu pedido está em espera (até 2h) enquanto validamos integrações. Você não precisa agir agora.”
* **Credor**: “Seu capital **não foi travado**; confirmaremos ao final da validação do pedido.”
* **Auto‑cancel**: “Pedido cancelado sem custos. Você pode republicar a qualquer momento.”

---

## 16. Critérios de Aceite (Gate A)

* Algoritmo, anti‑manipulação, TTL e tie‑breakers **implementáveis** e descritos.
* **Logs** e **schemas** publicados; hash/assinatura ativos.
* **UX 3 telas** + fallback com mensagens‑modelo.
* **KPIs** com fórmulas e bases (365/252) definidas.
* **Taxa mínima 0,50%** aplicada e **juros mínimo 6%**; **capital só trava** em `LoanConfirmed`.
* **Governança Fase 0** e hierarquia Master KB respeitadas.

---

## 17. Decisões/Parâmetros (ADR recomendados)

* **Oráculos & quorum** (sug. 2/3; provedores).
* **Faixas cripto pequena/grande** por ticket (sug. ≤ R\$25k = pequena).
* **Step mínimo 5 \_bps**, máx. ofertas=3, cooldown=60s, anti‑sniping=120s (+600s).
* **Retenção de logs** (sug. 5 anos) e RBAC.
* **Limiar de transações atípicas** e agregação por relacionamentos.
* **Conversões APR↔252** fixadas no data‑layer.

---

## 18. Glossário

CE\$, LoanVault, NPL30 (>30 \_days), ADR, uniform‑price adaptado CE\$ (média ponderada), APR (365), CDI (252), HHI.

---

> **Status**: **v6.0 — “Perfeita”**. Documento coeso, auditável e integralmente alinhado à Master KB; pronto para **Gate A** e parametrização via ADR onde indicado.
