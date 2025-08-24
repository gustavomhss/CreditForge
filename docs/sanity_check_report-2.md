# 🏛️ Master Knowledge Base — CreditEngine$ (Sanity Check Consolidado e Detalhado)

> **Hierarquia:** Este documento é promovido a nível **Master KB**, sobrepondo detalhes à BK v0.1 quando houver divergência. Sempre prevalecem as instruções aqui registradas até que haja nova decisão do PO ou ADR formal.

## Contexto
Consolidação do **Sanity Report v0.1 (complementado)** em formato de **base de conhecimento hierárquica** para todos os agentes (Protocol, Token, Risk, Banking, UX, Orchestrator, Security). Inclui SLAs, reavaliação de colaterais, reputação, acessibilidade e governança consultiva. 

---

## 📌 Pilares Confirmados
- **Leilão reverso (uniform-price adaptado)**: tomador acessa ofertas e escolhe composição final; credores competem por taxa.  
- **LoanVault**: garante liquidação até o valor colateralizado.  
- **Token CreditEngine$**: sempre lastreado (100% fiat, 130% cripto pequena, 105% cripto grande).  
- **Integrações externas**: score + fiat via parceiros.  
- **Operação 100% navegador (ChatGPT)**: UX unificada.  

---

## 🔧 Protocol & Mecânica
- **Default do leilão**: tomador pode estender, cancelar ou aceitar parcial.  
- **Liquidação parcial**: LoanVault cobre até o colateral.  
- **Inadimplência**: protocolo identifica atraso → credores decidem entre abandono, transferência direta (>R$2k), renegociação, judicialização conjunta (com *Report* gerado), ou venda secundária da dívida.  
  - **Observação**: SLA de notificação deve ser definido (horas até aviso aos credores). Relatórios jurídicos padronizados.  
- **Mercado secundário**: dívidas negociáveis em frações, formato “quanto pagar por cada R$1”.  

---

## 💰 Token & Economia
- **Supercolateralização escalável**: 130% (valores pequenos), 105% (valores grandes), 100% fiat.  
- **Reavaliação periódica**: cripto (24h), fiat/tokenizado (7 dias).  
- **Incentivos**: sem rewards extras. Credores decidem risco × retorno.  
- **Juros**: mínimo 6% a.a.; sem teto máximo; governança pode ajustar.  
- **Observação**: considerar taxa de serviço mínima para sustentabilidade.  

---

## ⚖️ Risco & Compliance
- **Scores alternativos**:  
  - MVP Brasil: Serasa, Bacen Registrato, Open Banking.  
  - Médio prazo: utilidades, telecom, pagamentos digitais.  
  - Longo prazo: bureaus globais, reputação on-chain.  
- **KYC/AML & Anti-fraude**:
  - **PF**: gateway fiat → coleta CPF, valida Receita. Protocolo cripto → coleta CPF, checa wallets/listas de sanção.  
  - **PJ**: gateway fiat → CNPJ + representante legal. Protocolo cripto → CNPJ + representante legal, reforço em operações >R$50k.  
- **Anti-fraude (detalhes)**: validação de CPF/CNPJ ativo, checagem de contas bancárias vinculadas, monitoramento de transações atípicas (>R$50k/dia), listas PEP e Chainalysis para cripto.  
- **Observação**: logs seguros devem ser armazenados para auditoria. Definir formato padrão de input (JSON/KYC schema) para simplificar integrações.  

---

## 🖥️ UX & Governança
- **Experiência do tomador**:
  - Ofertas listadas como marketplace (“prateleira de capital”).  
  - Sistema calcula taxa média ponderada automaticamente.  
  - Exemplo: 3k×10% + 5k×12% + 2k×14% ÷ 10k = **11,8% a.a.**  
- **UX em 3 telas**:  
  1. Pedido (valor, prazo, publicar).  
  2. Ofertas (lista + cálculo taxa média em tempo real).  
  3. Customização (colateral, anexos, taxa final).  
- **Extras**: reputação/badges para tomadores recorrentes; acessibilidade mobile-first; comunicação simples; ícones claros; suporte multilíngue.  
- **Governança**:
  - Fase 0: centralizada (mínimo 6%).  
  - Fase 1: tokenholders definem parâmetros.  
  - Extra: comitê de risco consultivo inicial até descentralização plena.  
  - **Regra de hierarquia**: sempre prevalece a versão mais recente do documento promovida a **Master KB**. Todos os agentes devem consultar este documento como referência máxima, até que o PO ou um ADR formal defina alteração.  

---

## 🔄 Fallback UX
- **Quando usar**: falha de score, antifraude ou gateway fiat. Evita travar capital.  
- **Estados**:  
  - RequestOnHold (aguarda serviço externo).  
  - RequestFilled (100% pool, aguardando validação).  
  - RequestAutoCancelled (não normalizou em SLA de 2h).  
- **Notificações (prontas para uso)**:  
  - Tomador: pedido em espera até 2h, sem ação necessária.  
  - Credores: capital não travado até normalização.  
  - Auto-cancelamento: pedido cancelado sem custos, pode republicar.  
- **Regras**:  
  - ON_HOLD aceita novas ofertas mas não confirma.  
  - Capital só bloqueado em LoanConfirmed.  
  - Ao retomar, recalcula pool e expirações.  
  - SLA inicial sugerido = 2h; revisável por ADR de governança.  

---

## ✅ Validação & Auto-check
- Pilares respeitam BK.  
- Fluxos detalhados, sem contradições.  
- Lacunas originais resolvidas em processos claros.  
- Detalhes adicionais incorporados: SLA, reavaliação de colaterais, reputação, acessibilidade, logs seguros.  
- Documento elevado a **Master KB**: prevalece sobre entradas anteriores em caso de conflito.  

---

## 📌 Próximos Passos
- Orchestrator transformar tópicos em **next_actions por agente**.  
- ADRs para SLA, formatos de colateral, parâmetros de governança inicial.  
- Security revisar logs/auditoria KYC e fallback.  

