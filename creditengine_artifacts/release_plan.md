# release_plan.md — MVP → R1

## Premissas
- Gate A concluído (2025-08-18): Product Brief v6.0 aprovado.
- ADR-001/002 vigentes; ADR-003/004/005 em proposta (parametrizáveis via config).

## Sprints (exemplo; ajuste datas conforme calendário)
- **Sprint 1 (2 semanas)** — Protocolo básico + UX 3 telas + logs base.
  - BL-001, BL-002, BL-007, BL-009.
- **Sprint 2 (2 semanas)** — Anti-manipulação + Banking + KYC/AML.
  - BL-003, BL-005, BL-006.
- **Sprint 3 (2 semanas)** — Pré-pagamento + Monitor de colateral + métricas.
  - BL-004, BL-008, instrumentação dos KPIs de `success_metrics.md`.
- **Sprint 4 (hardening)** — Observabilidade, segurança, testes E2E e go-live controlado.

## Gates de qualidade (saída de sprint)
- Critérios de aceite por história cumpridos e revisados por Security quando aplicável.
- KPIs mínimos instrumentados (Funding ≤24h, Pool ≥65%).

## Riscos & mitigação
- Oráculos atrasados → usar fonte temporária interna com auditoria (flag) até ADR-004.
- Gateway fiat intermitente → fallback `RequestOnHold` + mensagens.

## Go/No-Go
- PO decide com base em `acceptance_criteria.md` + KPIs atingíveis.