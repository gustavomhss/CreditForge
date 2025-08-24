# Arquitetura (v0.1) — Visão de alto nível
Módulos on-chain: CreditEngineToken, AuctionManager, LoanVault, RiskRegistry, PaymentRouter.
Módulos off-chain: Risk Adapter (ratings); Bank Adapter (webhooks + reconciliação); Orchestrator (event sourcing).

Fluxo resumido do leilão:
1) Tomador publica pedido (valor, max_rate_bps, tenor_days, risk_hash).
2) Credores ofertam (valor, rate_bps). Ordenação por taxa asc e timestamp.
3) Clear: taxa de clearing definida; cria LoanVault; credores alocados recebem taxa_exec = clearing.
4) Drawdown: PaymentRouter sinaliza transferência fiat via parceiro; on-chain registra estado.
5) Repagamento: parcelas roteadas ao LoanVault; distribuição pro-rata; mora se atraso.

Segurança: timelocks, pausas, ReentrancyGuard, oráculos redundantes, provas de reserva, logs completos.
