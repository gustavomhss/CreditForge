# ADR-003 — Política de Pré-Pagamento (MVP)

**Status:** proposed  
**Data:** 2025-08-18  
**Owner:** Product Owner  
**Escopo:** Protocolo | Produto

## Contexto
Formalizar §7.4 do Product Brief. [BK:/protocol#prepayment]

## Decisão
- Pré-pagamento permitido **a qualquer tempo**, **sem multa**.
- Cobrança de **juros pró-rata die** até a data da liquidação.
- **Taxa de serviço 0,50%**: aplicada no desembolso e **não reembolsável**.
- Evento: `LoanPrepaid { principal_pago, juros_pro_rata, saldo }`.

## Racional
Simplicidade do MVP e previsibilidade ao tomador.

## Impactos
Cálculo pró-rata; mensagens UX; conciliação; testes de arredondamento.

## Implementação
Atualizar serviço de liquidação; testes de centavos; logs JSON + hash.

## Compatibilidade
Complementa Product Brief v6.0 §7.4; relaciona-se a ADR-002.