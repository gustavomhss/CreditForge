# stakeholder_alignment.md — CreditEngine$

## Status
- **Product Brief (MVP) v6.0 — “Perfeita”**: **Aprovado (Gate A)** em 2025-08-18.
- **ADRs**: 001/002 **approved**; 003/004/005 **proposed** (aguardam aprovação PO).

## Stakeholders & papéis (RACI simplificado)
- **PO** — R/A por escopo, prioridades, aceite.
- **Professor** — R por didática/prompts; C em planejamento.
- **Orchestrator** — R/A por coerência técnica e integração; C para PO.
- **Especialistas** — R por entregas (Protocol, Token, Risk, Banking, UX).
- **Security** — R/A por riscos críticos.
- **Troubleshooter** — R por diagnóstico; sem A.
- **Creative** — R por alternativas/experimentos; C para PO.

## Acordos e trade-offs confirmados
- **Clearing do leilão = média ponderada (APR)** (não menor lance). Simplicidade e previsibilidade ao tomador.
- **Capital só trava em `LoanConfirmed`**. Reduz atrito durante o book.
- **Pré-pagamento sem multa** (proposto em ADR-003) — foco em UX e MVP-safe.
- **Juros mínimo 6% a.a. (Fase 0)** e **taxa de serviço mínima 0,50%** — unit economics do MVP.
- **Monitor de colateral** com reavaliação 24h (cripto)/7d (fiat); sem margin call no MVP — apenas alerta.

## Aprovações registradas
- PO: Product Brief v6.0 — **aprovado**.
- Security: requisitos de logs/cripto/auditoria — **de acordo** com MVP; revisão contínua na implementação.
- Orchestrator: sequência de execução (Professor → Especialistas → Security) — **validada**.

## Pendências para ADR (não bloqueantes para Gate A)
- ADR-003 (Pré-pagamento) — aprovar.
- ADR-004 (Oráculos/quórum 2/3) — aprovar e indicar provedores.
- ADR-005 (Parâmetros anti-manipulação & faixas cripto) — aprovar.