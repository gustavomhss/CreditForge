# acceptance_criteria.md — MVP

## Protocolo
- Ordenação por menor APR; tie-breakers: (i) maior volume, (ii) timestamp mais antigo, (iii) hash do lance.
- Pró-rata na margem em centavos; ajuste final ≤ 1 centavo na última linha.
- Clearing: **APR_média_ponderada** com `apr_weighted_bps = sum(amount_cent * apr_bps)/sum(amount_cent)`.
- Anti-manipulação (parametrizável): step 5 _bps; máx. 3 ofertas/credor; cooldown 60s; anti-sniping 120s (teto +600s); juros mínimo 6% a.a.
- Estados de fallback ON_HOLD/AUTO_CANCELLED; capital só trava em **LoanConfirmed**.

## Tokenomics
- Colateral: 130% cripto pequena (≤ R$25k); 105% cripto grande; 100% fiat.
- Oráculos de paridade com quórum 2/3 (em aprovação); logs `OracleUpdate` auditáveis.

## Risk & Compliance
- KYC PF/PJ; listas de sanção; PEP; contas bancárias vinculadas; Chainalysis.
- Logs KYC/AML: JSON + hash; RBAC; auditoria de leitura; retenção sugerida 5 anos.

## Banking
- Cobrança **0,50%** no desembolso; recibos e conciliação diária.

## UX & Acessibilidade
- 3 telas (Pedido/Ofertas/Customização) com cálculo em tempo real; aceite parcial.
- Mobile-first; EN/PT; contraste AA; foco visível; labels ARIA.

## Observabilidade & Segurança
- Logs/eventos JSON com SHA-256 + assinatura; schemas versionados (semver).
- TLS 1.3; AES-256 em repouso; backups diários com verificação; RBAC.

## KPIs mínimos instrumentados
- Funding ≤24h; Pool ≥65%; NPL30 ≤3%; Yield ≥ CDI + 150 _bps.