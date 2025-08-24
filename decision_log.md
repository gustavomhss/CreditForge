# decision_log.md — CreditEngine$

> Hierarquia: Master KB > docs anteriores até ADR. Logs em **UTC**; exibição em timezone do usuário (America/Bahia).

## Resumo (humano)
- **2025-08-18** — Gate A: *Product Brief (MVP) v6.0 — “Perfeita”* **aprovado** pelo PO.
- **2025-08-18** — ADR-001 (**SLA default ≤6h**) — **approved** (vigente).
- **2025-08-18** — ADR-002 (**Taxa mínima 0,50%**) — **approved** (vigente).
- **2025-08-18** — ADR-003 (**Pré-pagamento**) — **proposed** (aguarda aprovação PO).
- **2025-08-18** — ADR-004 (**Oráculos & quórum 2/3**) — **proposed**.
- **2025-08-18** — ADR-005 (**Antimanipulação & faixas cripto**) — **proposed**.
- **2025-08-18** — Distribuição do Brief + ADRs para **11 agentes** na KB (banner de precedência fixado).

## Log auditável (NDJSON)
{"id":"DL-2025-08-18-01","ts_utc":"2025-08-18T00:00:00Z","ts_local_tz":"2025-08-18T00:00:00-03:00 America/Bahia","actor":"Product Owner","type":"GateAApproved","subject":"Product Brief (MVP) v6.0 — \"Perfeita\"","status":"approved","basis":["Master KB (Sanity Check v2)","ADR-001","ADR-002"],"links":["/KB/product_brief_v6.0.md"],"checksum_sha256":"<to-be-generated>","signature":"<platform>"}
{"id":"DL-2025-08-18-02","ts_utc":"2025-08-18T00:00:00Z","ts_local_tz":"2025-08-18T00:00:00-03:00 America/Bahia","actor":"Product Owner","type":"ADR","subject":"ADR-001 — SLA default ≤6h","status":"approved","links":["/KB/ADRs/ADR-001_SLA_default_le6h.md"],"checksum_sha256":"<to-be-generated>","signature":"<platform>"}
{"id":"DL-2025-08-18-03","ts_utc":"2025-08-18T00:00:00Z","ts_local_tz":"2025-08-18T00:00:00-03:00 America/Bahia","actor":"Product Owner","type":"ADR","subject":"ADR-002 — Taxa mínima de serviço 0,50%","status":"approved","links":["/KB/ADRs/ADR-002_taxa_servico_min_0p50.md"],"checksum_sha256":"<to-be-generated>","signature":"<platform>"}
{"id":"DL-2025-08-18-04","ts_utc":"2025-08-18T00:00:00Z","ts_local_tz":"2025-08-18T00:00:00-03:00 America/Bahia","actor":"Product Owner","type":"ADR","subject":"ADR-003 — Política de Pré-Pagamento (MVP)","status":"proposed","links":["/KB/ADRs/ADR-003_politica_prepagamento_mvp.md"],"checksum_sha256":"<to-be-generated>","signature":"<platform>"}
{"id":"DL-2025-08-18-05","ts_utc":"2025-08-18T00:00:00Z","ts_local_tz":"2025-08-18T00:00:00-03:00 America/Bahia","actor":"Product Owner","type":"ADR","subject":"ADR-004 — Oráculos de Paridade CE$ (quórum 2/3)","status":"proposed","links":["/KB/ADRs/ADR-004_oraculos_paridade_quorum-2-de-3.md"],"checksum_sha256":"<to-be-generated>","signature":"<platform>"}
{"id":"DL-2025-08-18-06","ts_utc":"2025-08-18T00:00:00Z","ts_local_tz":"2025-08-18T00:00:00-03:00 America/Bahia","actor":"Product Owner","type":"ADR","subject":"ADR-005 — Parâmetros Anti-Manipulação & Faixas de Colateral Cripto","status":"proposed","links":["/KB/ADRs/ADR-005_parametros_antimanipulacao_e_faixas_cripto.md"],"checksum_sha256":"<to-be-generated>","signature":"<platform>"}
{"id":"DL-2025-08-18-07","ts_utc":"2025-08-18T00:00:00Z","ts_local_tz":"2025-08-18T00:00:00-03:00 America/Bahia","actor":"Product Owner","type":"KBUpdate","subject":"Distribuição do Product Brief v6.0 + ADRs 001/002/003/004/005 para os 11 agentes","status":"completed","details":{"banner":"[HIERARQUIA] Master KB > docs anteriores até ADR. [STATUS] Brief v6.0 APROVADO (Gate A, 2025-08-18). [OBRIGATÓRIO] ADR-001 • ADR-002."},"links":["/KB/master/SanityCheck_v2.md","/KB/product_brief_v6.0.md","/KB/ADRs/"],"checksum_sha256":"<to-be-generated>","signature":"<platform>"}




{"id": "DL-2025-08-20-S1-START", "ts_utc": "2025-08-20T05:09:56Z", "ts_local_tz": "2025-08-20T02:09:56-0300 -03", "actor": "Orchestrator", "type": "SprintStarted", "subject": "Sprint 1 aberta (Kanban, sem datas)", "status": "ongoing", "details": {"stories": ["BL-001", "BL-002", "BL-007", "BL-009"], "labels": ["S1"], "wip_policy": "2 por pessoa"}}
