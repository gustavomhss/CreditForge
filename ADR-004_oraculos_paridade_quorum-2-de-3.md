# ADR-004 — Oráculos de Paridade CE$ (quórum 2/3)

**Status:** proposed  
**Data:** 2025-08-18  
**Owner:** Token Specialist (com PO)  
**Escopo:** Token | Dados | Segurança

## Contexto
Manter **paridade 1:1** do CE$ com reservas (fiat/cripto) via oráculos. [BK:/token#paridade]

## Decisão
- **Quórum 2/3**: ao menos 2 de 3 oráculos concordantes para atualizar paridade.
- Janelas de atualização: **24h cripto / 7d fiat** (alinhado ao monitor de colateral).
- Liveness: alerta se ≥ 26h (cripto) ou ≥ 8d (fiat) sem atualização.
- Auditoria: registrar `OracleUpdate { ts_utc, providers, median, proof }`.

## Racional
Resiliência a falhas/parciais e trilha auditável.

## Impactos
Módulo de agregação; alertas; dashboards; playbook de contingência.

## Implementação
Agregador com mediana; validade por tipo de ativo; storage com assinatura.

## Compatibilidade
Formaliza o comportamento descrito no Product Brief v6.0.