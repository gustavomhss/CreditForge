# Webhooks do parceiro bancário (v0.1)
Eventos:
- CREDIT_CONFIRMED: crédito recebido (depósito do usuário).
- DEBIT_SETTLED: pagamento liquidado (saída para tomador/credor).
- REVERSAL: estorno/chargeback.

Campos mínimos (todos os eventos):
- event_type, event_id, occurred_at, idempotency_key, signature
- account_ref, currency, amount, narrative
- metadata: { tx_ref, customer_id, bank_code, ... }

Assinatura: HMAC-SHA256 sobre corpo canonicalizado; header `X-Signature`.
Retry: backoff exponencial (5 tentativas). Idempotência via `idempotency_key`.
