# ADR-002 — Taxa mínima de serviço 0,50% sobre valor financiado

**Status:** approved  
**Data:** 2025-08-18  
**Owner:** Product Owner  
**Escopo:** Produto | Token | Financeiro

## Contexto
Garantir receita mínima por operação e cobertura de custos. [BK:/token#fees]

## Decisão
- **Taxa mínima 0,50%** sobre **valor financiado**, aplicada **uma única vez** no desembolso.
- **Não reembolsável** em pré-pagamento (ver ADR-003).
- Arredondamento em **centavos (off-chain)** conforme normas CE$.

## Racional
Sustentação do MVP e previsibilidade de unit economics.

## Impactos
Cálculo no desembolso; exposição em UX e recibos; conciliação financeira.

## Implementação
Aplicar no pipeline de **LoanConfirmed**; registrar no evento e nos recibos.

## Compatibilidade
Complementa o Product Brief v6.0; referência cruzada com ADR-003.