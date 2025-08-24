# ADR-001 — SLA default ≤6h (notificação/execução)

**Status:** approved  
**Data:** 2025-08-18  
**Owner:** Product Owner  
**Escopo:** Produto | Operações

## Contexto
Padronizar prazos de ações assíncronas (notificações, reprocessos, callbacks) no MVP. [BK:/governance#adr-001]

## Decisão
- **SLA default ≤ 6h** para tarefas operacionais do MVP (notificação/execução).
- Exceções: incidentes seguem Security (§12): **SEV-1 ≤1h**, **SEV-2 ≤4h**, **SEV-3 ≤24h**.
- Medir em UTC (logs) e exibir em timezone do usuário.

## Racional
Evita ambiguidade entre times, simplifica expectativas com parceiros e auditoria.

## Impactos
Ferramentas de fila/agendador; dashboards de SLA; alertas quando >80% do prazo.

## Implementação
Timers por job; métricas por evento; retries com backoff; auditoria em JSON + hash.

## Compatibilidade
Base do MVP; não substitui ADR anterior.
