# success_metrics.md — CreditEngine$

## Convenções
- **APR anual**: base **365 dias**.
- **CDI**: base **252 dias**.
- Conversão: `APR_252 = (1+APR)^(252/365) - 1` (pode usar aproximação no dashboard).
- Unidades: **_bps**, **_days/_seconds**, **centavos (off-chain)**, **wei (on-chain)**.

## KPIs (definições e fórmulas)
1. **Funding ≤24h**: `t(LoanConfirmed) − t(AuctionCreated)` ≤ 24h (P95) — alvo: ≥ 90% dos casos.
2. **Pool ≥65% antes do aceite**: `sum(accepted_amount_before_borrower_accept)/requested_amount` ≥ 0,65.
3. **NPL30 ≤3%**: `principal_atrasado_>30d / carteira_vigente` ≤ 0,03.
4. **Ativação lenders D7 ≥40%**: `lenders_com_≥1_oferta_aceita_em_D7 / lenders_novos` ≥ 0,40.
5. **Retenção D30 ≥60%**: `lenders_ativos_D30 / lenders_ativos_D7` ≥ 0,60.
6. **Yield ≥ CDI + 150 _bps**: `APR_media_confirmada_252 – taxa_servico` ≥ `CDI_252 + 150 _bps`.
7. **Qualidade do leilão**:
   - (i) taxa de cancelamento < 15% por credor/auction;
   - (ii) % de leilões com anti-sniping < 25%;
   - (iii) **HHI** de concentração de funding ≤ 0,35.

## Instrumentação mínima
- Eventos estruturados (`AuctionCreated`, `OfferPlaced/Updated/Cancelled`, `LoanConfirmed`, `LoanPrepaid`, `LoanDefaulted`, `LoanClosed`).
- Campos: `id`, `ts_utc`, `payload_hash`, valores em centavos/wei, APR em _bps.