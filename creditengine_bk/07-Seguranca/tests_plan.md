# Plano de Testes (v0.1)
- Unitários: leilão, accrual, distribuição pro-rata, pausas.
- Fuzz: lances aleatórios, gaps de liquidação, atrasos.
- Invariants: saldo do Vault = soma de posições; não cunhar sem lastro; sem drawdown sem clear.
- Testes de integração: simular webhooks e reconciliação com casos de erro.
