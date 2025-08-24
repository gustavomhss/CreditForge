# Reconciliação (v0.1)
- Event sourcing: toda mudança no ledger off-chain é um evento imutável.
- Janelas: recon diária às 02:00 BRT (America/Bahia).
- Passos: importar extrato → normalizar → casar por `tx_ref`/valor/data → gerar diferenças → reprocessar com idempotência.
- Divergências críticas pausam `PaymentRouter` até resolução.
