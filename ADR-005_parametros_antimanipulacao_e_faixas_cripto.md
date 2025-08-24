# ADR-005 — Parâmetros Anti-Manipulação & Faixas de Colateral Cripto

**Status:** proposed  
**Data:** 2025-08-18  
**Owner:** Protocol Specialist (com PO)  
**Escopo:** Protocolo | Token | Risco

## Contexto
Consolidar §7.1.1 (anti-manipulação) e faixas de colateral. [BK:/protocol#auction] [BK:/token#collateral]

## Decisão
- **Step mínimo de taxa:** **5 _bps**.
- **Máx. ofertas ativas por credor/auction:** **3**.
- **Cooldown cancelamento:** **60 _seconds**.
- **Anti-sniping:** lances nos **últimos 120 _seconds** estendem o fim em **+120 _seconds** (teto **+600 _seconds**).
- **Juros mínimo (Fase 0):** **≥ 6% a.a.** (APR, base 365).
- **Faixas de colateral:** **Cripto pequena ≤ R$25k → 130%**; **Cripto grande > R$25k → 105%**; **Fiat → 100%**.
- **Detecção de Sybil:** sinais via KYC/banco/IP/dispositivo (sinal; decisão manual do comitê).

## Racional
Evitar gaming do leilão e calibrar risco por ticket.

## Impactos
Validador de ofertas; UI (regras claras); monitor de colateral e alertas.

## Implementação
Parâmetros em config de governança; testes de borda; logs de eventos com hash.

## Compatibilidade
Detalha e fixa parâmetros do Product Brief v6.0 §§7.1.1 e 8.