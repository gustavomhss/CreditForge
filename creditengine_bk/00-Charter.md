# CreditEngine$ — Charter (v0.1)

Propósito: marketplace P2P de crédito com leilão reverso (uniform-price), liquidação via LoanVault e token CreditEngine$ lastreado por reservas (fiat/cripto), sem assumir risco de crédito na plataforma.

Objetivos MVP (4 sprints):
1) Núcleo on-chain (AuctionManager, LoanVault, CreditEngineToken) e esqueleto off-chain (Risk/Bank adapters).
2) Integração fiat (webhooks + reconciliação) e risco externo (hash ancorado on-chain).
3) Cofre cripto com LTV e liquidação automática; oráculos redundantes (Chainlink + TWAP) com circuit breakers.
4) Segurança (timelocks, pausas, testes básicos) e UX mínima.

Não-objetivos (MVP): bancos múltiplos, multicollateral avançado, derivativos, stablecoin própria.

Princípios: simplicidade, auditabilidade, minimização de privilégios, transparência de taxas, isolamento de risco.
