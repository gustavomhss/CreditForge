# Padrões de nomes (v0.1)
- Sufixo em bps para parâmetros percentuais: `*_bps` (ex.: max_rate_bps, ltv_max_bps).
- Tempo sempre em segundos ou dias explícitos: `*_seconds`, `*_days`.
- Eventos no particípio passado claro: AuctionCreated, AuctionCleared.
- Variáveis monetárias em unidades mínimas (wei, centavos) documentadas.
