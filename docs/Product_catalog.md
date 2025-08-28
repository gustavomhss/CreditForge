# \# Product Map — CreditEngine$

# 

# \#\# Finalidade

# Este documento instrui os agentes sobre como interpretar e utilizar o \*\*Catálogo Único v5.8\*\*.  

# Ele deve ser entendido como um \*\*mapa de visão de longo prazo\*\* — não um backlog imediato.  

# 

# \#\# Como usar

# 1\. \*\*Referência principal\*\*: use sempre o catálogo para consultar nomes, descrições, tickets médios, taxas, prazos e economia ao tomador.  

# 2\. \*\*Horizonte de entrega\*\*:

#    \- \*\*MVP (2025)\*\*: Contas digitais básicas, PIX, TED, boleto, cartão de débito, crédito pessoal simples (PF).  

#    \- \*\*R1 (2026)\*\*: Crédito PJ (capital de giro, antecipação de recebíveis), adquirência, gateways, split de pagamentos.  

#    \- \*\*R2 (2027)\*\*: Investimentos (Tesouro, CDB, fundos), seguros básicos (vida, residencial, auto simples), wealth simples.  

#    \- \*\*R3+ (longo prazo)\*\*: Trade finance, project finance, previdência, family office, produtos estruturados/complexos.  

# 3\. \*\*Agentes devem sempre\*\*:  

#    \- Manter consistência de nomes/unidades conforme BK.  

#    \- Evitar feature drift: se um produto não estiver no catálogo, consulte PO.  

#    \- Usar este arquivo para orientar \*\*escopo e sprints futuros\*\*.

# 

# \#\# Catálogo de Produtos (v5.8)

# \*(O conteúdo abaixo é o catálogo integral, sem alterações. Incluído aqui para manter contexto completo.)\*

# 

# \---

# 

# 

# 

# CATÁLOGO v5.8 — Versão Completa com Tabelas (HTML → DOCX)

# **CATÁLOGO v5.8 — Pacote Integrado para Google Docs**

Modo: Export consolidado — inclui o conteúdo original (se disponível) e o patch não‑destrutivo (v5.8p) num único documento para importação direta no Google Docs.

# **Original v5.8 — Conteúdo extraído do DOCX**

Catálogo Único — VERSÃO FINAL (v5.8) — CONSOLIDADO LIMPO

Fechado em 26/08/2025 02:33 (horário local).

Sanity check completo aplicado (regras de preço, consistências e faixas). QA detalhado no Excel v14.

# **Resumo e sanidade**

***Métrica; Valor***  
***Produtos totais; 350***  
***Descrições XL (≥300 chars); 350***  
***Viol. regra 'mais barato que banco'; 0***  
***Inconsistências (juros/custo/economia); 0***  
***Taxas fora 0%–50% a.m.; 0***  
***Volumes inválidos (\<0); 0***  
***Duplicatas por nome; 6***

# **Tabela-mestra consolidada**

***Domínio; Familia; Categoria/Subfamília; Produto; Ticket padrão (R$); Banco\_taxa\_am; Sua\_taxa\_am; Prazo (dias); Banco\_juros\_R$; Tomador\_custo\_voce\_R$; Tomador\_economia\_R$; Volume de mercado (snapshot)***  
***Tradicional; Accounts & Deposits; Contas; Conta Corrente PF; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Accounts & Deposits; Contas; Conta Corrente PJ; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Accounts & Deposits; Contas; Conta Salário; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Accounts & Deposits; Contas; Conta Universitária; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Accounts & Deposits; Contas; Conta MEI; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Accounts & Deposits; Depósitos; Poupança; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Accounts & Deposits; Depósitos a prazo; CDB Pós‑CDI; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Accounts & Deposits; Depósitos a prazo; CDB Prefixado; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Accounts & Deposits; Depósitos a prazo; CDB Escalonado; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Accounts & Deposits; Depósitos a prazo; LCI; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Accounts & Deposits; Depósitos a prazo; LCA; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Accounts & Deposits; Depósitos a prazo; LC (Letra de Câmbio); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Accounts & Deposits; Depósitos a prazo; LF (Letra Financeira); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Accounts & Deposits; Contas; Conta Pagamento (Carteira Digital); R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Tradicional; Payments & Transfers; PIX; PIX Transferência; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; PIX; PIX Cobrança (QR Dinâmico); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; PIX; PIX Saque; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Payments & Transfers; PIX; PIX Troco; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Payments & Transfers; Transferências; TED; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; Transferências; SWIFT Internacional; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; Cobrança; Boleto – Emissão; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; Cobrança; Boleto – Cobrança Registrada; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; Pagamentos; Débito Automático; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; Pagamentos; DDA (Débito Direto Autorizado); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; Pagamentos; Agendamento de Pagamentos; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; Pagamentos; Pagamento de Tributos; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; Pagamentos; Tokenização Carteiras (Apple/Google Pay); R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Payments & Transfers; Cobrança; Link de Pagamento; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; Cobrança; Split de Pagamentos; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; Cobrança; QR Code Estático Loja; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; PSP/Acquiring; Gateway de Pagamentos; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; Cobrança; Assinaturas/Recorrência; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; Pagamentos; Pagamento por Aproximação (NFC); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Payments & Transfers; Cobrança; Portal de Cobranças PJ; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cards; Débito; Cartão de Débito; R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Tradicional; Cards; Crédito; Cartão de Crédito Internacional; R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Crédito; Cartão Gold; R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Crédito; Cartão Platinum; R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Crédito; Cartão Black/Infinite; R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Crédito; Cartão Empresarial (Business); R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Tradicional; Cards; Crédito; Cartão Corporate (T\&E); R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Tradicional; Cards; Pré‑pago; Cartão Pré‑pago; R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Tradicional; Cards; Crédito; Cartão Co‑branded/Private Label; R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Crédito; Cartão Consignado; R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Crédito; Cartão com Garantia (Secured); R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Crédito; Cartão Adicional; R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Crédito/Débito; Cartão Virtual; R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Tradicional; Cards; Pré‑pago; Cartão Multimoeda (Travel); R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Serviços ao Cartão; Parcelamento de Fatura; R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Serviços ao Cartão; Rotativo Gerenciado; R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Serviços ao Cartão; Programa de Pontos/Milhas; R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Serviços ao Cartão; Cashback; R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Serviços ao Cartão; Proteção de Compra/Preço; R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Cards; Crédito; Limite Garantido por CDB; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Loans \- Retail; Crédito PF; Empréstimo Pessoal; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Crédito PF; Consignado INSS; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Crédito PF; Consignado Privado; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Crédito PF; Cheque Especial (Overdraft); R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Crédito PF; Parcelamento do Cheque Especial; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Crédito PF; Antecipação 13º Salário; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Crédito PF; Antecipação Restituição IR; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Crédito PF; Home Equity (Garantia de Imóvel); R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Crédito PF; Crédito com Garantia de Veículo; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Crédito PF; Crédito com Garantia de Investimento; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Financiamentos; Financiamento de Veículos (CDC); R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Financiamentos; Financiamento Imobiliário SFH; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Financiamentos; Financiamento Imobiliário SFI; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Financiamentos; Portabilidade de Crédito Imobiliário; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Financiamentos; Refinanciamento de Veículo; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Financiamentos; Crediário/BNPL via Banco; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Financiamentos; Crédito Educacional; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- Retail; Microcrédito; Microcrédito PF; R$ 8.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 2.418,08; R$ 1.763,00; R$ 655,08; —***  
***Tradicional; Loans \- SME/Corp; Crédito PJ; Capital de Giro; R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Crédito PJ; Cheque Especial PJ; R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Crédito PJ; Conta Garantida; R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Crédito PJ; Giro com Trava de Recebíveis; R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Crédito PJ; Desconto de Duplicatas; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Loans \- SME/Corp; Crédito PJ; Antecipação de Recebíveis de Cartão; R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Tradicional; Loans \- SME/Corp; Crédito PJ; NCE/CCE; R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Crédito PJ; BNDES FINAME (repasse); R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Crédito PJ; BNDES Automático; R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Trade/Crédito PJ; ACC (Adiantamento Contrato de Câmbio); R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Trade/Crédito PJ; ACE (Adiantamento Cambiais Entregues); R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Financiamentos; Financiamento Máquinas/Equipamentos; R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Financiamentos; Financiamento de Veículos PJ; R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Financiamentos; Crédito para Construção/Real Estate Corp; R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Estruturado; Project Finance; R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Estruturado; Empréstimo Sindicalizado; R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Crédito PJ; Linha Revolving (Standby); R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Loans \- SME/Corp; Microcrédito; Microcrédito Produtivo Orientado; R$ 5.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 1.511,30; R$ 1.101,87; R$ 409,43; —***  
***Tradicional; Trade Finance & Guarantees; LCs; Carta de Crédito – Importação; R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Tradicional; Trade Finance & Guarantees; LCs; Carta de Crédito – Exportação; R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Tradicional; Trade Finance & Guarantees; Collections; Cobrança Documentária; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Trade Finance & Guarantees; Collections; Remessas Diretas (Clean); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Trade Finance & Guarantees; Recebíveis; Forfaiting; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Trade Finance & Guarantees; SCF; Confirming (Reverse Factoring); R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Tradicional; Trade Finance & Guarantees; SCF; Supply Chain Finance (SCF); R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Tradicional; Trade Finance & Guarantees; Recebíveis; Invoice Discounting Internacional; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Trade Finance & Guarantees; Garantias; Garantia – Bid Bond; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Trade Finance & Guarantees; Garantias; Garantia – Performance Bond; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Trade Finance & Guarantees; Garantias; Garantia – Advance Payment; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Trade Finance & Guarantees; Garantias; Garantia – Maintenance; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Trade Finance & Guarantees; Garantias; Standby Letter of Credit (SBLC); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Trade Finance & Guarantees; Garantias; Aval em Títulos; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Trade Finance & Guarantees; Garantias; Seguro Garantia (via banco); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Trade Finance & Guarantees; Trade Loans; Trade Loans (Pós‑Shipment); R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Cash Management & Merchant; Cash Mgmt; Folha de Pagamento (Payroll); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Cash Mgmt; Gestão de Contas a Pagar (AP); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Cash Mgmt; Gestão de Contas a Receber (AR); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Cash Mgmt; Conciliação Bancária Automática; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Cash Mgmt; Extratos CNAB/EDI; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Cash Mgmt; Lockbox; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Cash Mgmt; Varredura (Sweeping) de Contas; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Cash Mgmt; Pooling de Caixa (Notional/Physical); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Cash Mgmt; Pagamentos Massivos (Lotes); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Acquiring; Split de Recebíveis Marketplace; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Acquiring; Subadquirência (White‑label); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Acquiring; POS – Aluguel/Comodato; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Acquiring; Gateway de Pagamento Enterprise; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Acquiring; Antifraude Transacional; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; APIs; API Banking (Contas/Pagamentos); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Cash Management & Merchant; Cash Mgmt; Contas Virtuais (Virtual Accounts); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Fixed Income; Government Bonds; Tesouro Selic; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Investments \- Fixed Income; Government Bonds; Tesouro Prefixado; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Investments \- Fixed Income; Government Bonds; Tesouro IPCA+; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Investments \- Fixed Income; Bank Bonds; CDB Pós‑CDI; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Fixed Income; Bank Bonds; CDB Prefixado; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Fixed Income; Bank Bonds; CDB Escalonado; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Fixed Income; Bank Bonds; LCI; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Investments \- Fixed Income; Bank Bonds; LCA; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Investments \- Fixed Income; Finance Companies; LC (Letra de Câmbio); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Fixed Income; Corporate Bonds; Debêntures Simples; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Fixed Income; Corporate Bonds; Debêntures Incentivadas (Infra); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Fixed Income; Securitização; CRA; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Fixed Income; Securitização; CRI; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Fixed Income; Bank Bonds; Letras Financeiras (LF); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Fixed Income; Bank Bonds; DPGE; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Investments \- Fixed Income; Corporate Bonds; Nota Promissória Comercial; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Fundos RF; Fundo DI; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Fundos RF; Fundo RF Crédito Privado; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Multimercados; Fundo Multimercado Macro; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Multimercados; Fundo Long & Short Neutro; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Cambiais; Fundo Cambial Dólar; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Ações; Fundo de Ações Ibovespa Ativo; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Ações; Fundo de Ações Dividendos; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Ações; Fundo Small Caps; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Ações; Fundo Setorial (Infra/Utilidades); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Multimercados; Fundo Quantitativo; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Ações/MM; Fundo ESG; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Ações; Fundo Internacional Global Equity; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Multimercados; Fundo Multimercado com Proteção; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; ETFs; ETF Ibovespa (ex. BOVA11); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; ETFs; ETF S\&P 500 (ex. IVVB11); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; ETFs; ETF de Renda Fixa; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; ETFs; ETF Setorial/Temático; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Imobiliários; FII – Tijolo; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Imobiliários; FII – Papel; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Crédito Estruturado; FIDC; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Investments \- Funds/ETFs/COE; COE; COE – Autocallable; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Investments \- Funds/ETFs/COE; COE; COE – Twin Win; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Investments \- Funds/ETFs/COE; COE; COE – Capital Protegido (Moeda); R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Investments \- Funds/ETFs/COE; Previdência em fundos; Fundo Previdenciário (Estrutura Master‑Feeder); R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Brokerage/Wealth; Brokerage; Conta de Corretora / Home Broker; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Brokerage/Wealth; Brokerage; Custódia de Ativos; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Brokerage/Wealth; Brokerage; Aluguel de Ações (SLB); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Brokerage/Wealth; Brokerage; Margem para Operações; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Brokerage/Wealth; Brokerage; Negociação de Opções; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Brokerage/Wealth; Brokerage; Acesso a Futuros (BM\&F); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Brokerage/Wealth; Wealth; Mesa de Operações Estruturadas; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Brokerage/Wealth; Wealth; Carteira Administrada (DPM); R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Tradicional; Brokerage/Wealth; Wealth; Advisory de Investimentos; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Brokerage/Wealth; Wealth; Family Office; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Brokerage/Wealth; Wealth; Acesso Offshore; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Brokerage/Wealth; Wealth; Planejamento Sucessório; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Vida; Seguro de Vida Temporário; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Insurance & Protection; Vida; Seguro de Vida Resgatável; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Insurance & Protection; Vida; Seguro Doenças Graves; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Insurance & Protection; Vida; Acidentes Pessoais; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Insurance & Protection; Vida/Crédito; Seguro Prestamista (Credit Life); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Vida/Crédito; Proteção Financeira/Perda de Renda; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Insurance & Protection; Ramos Elementares; Seguro Residencial; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Insurance & Protection; Ramos Elementares; Seguro Condomínio; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Ramos Elementares; Seguro Empresarial (Multirrisco); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Auto; Seguro Automóvel; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Insurance & Protection; Auto; Seguro Frotas; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Viagem; Seguro Viagem; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Afinidades; Seguro Cartão (Compra Protegida); R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; Insurance & Protection; Afinidades; Garantia Estendida; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Insurance & Protection; Afinidades; Seguro Celular/Portáteis; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Insurance & Protection; Riscos Especiais; Seguro Cibernético PME; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Responsabilidade; D\&O (Directors & Officers); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Responsabilidade; E\&O (Responsabilidade Profissional); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Garantias; Seguro Garantia (Surety); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Riscos Especiais; Seguro Rural/Agrícola; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Saúde/Odont; Saúde Coletivo (parceria); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Saúde/Odont; Dental Coletivo; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Ramos Elementares; Seguro Transporte (Carga); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Insurance & Protection; Afinidades; Seguro Pet; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; FX & Hedging; FX Retail; Câmbio Turismo (Espécie); R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; FX & Hedging; FX Retail; Cartão Viagem Multimoeda; R$ 8.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 301,87; R$ 195,79; R$ 106,08; —***  
***Tradicional; FX & Hedging; Remittances; Remessa Internacional PF (Envio); R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; FX & Hedging; Remittances; Remessa Internacional PJ (Envio); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; FX & Hedging; Remittances; Recebimento do Exterior (Wire In); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; FX & Hedging; FX Wholesale; Contrato de Câmbio Pronto; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; FX & Hedging; Derivativos; NDF (Câmbio Futuro); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; FX & Hedging; Derivativos; Swap Cambial; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; FX & Hedging; Derivativos; Opções de Moeda (Vanilla); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; FX & Hedging; Remittances; Pagamentos Globais Massivos; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; FX & Hedging; FX Wholesale; Hedge de Importação; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; FX & Hedging; FX Wholesale; Hedge de Exportação; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Consórcios; Consórcios; Consórcio Imobiliário; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Consórcios; Consórcios; Consórcio Automóvel; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Consórcios; Consórcios; Consórcio Motos; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Consórcios; Consórcios; Consórcio Caminhões/Máquinas; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Consórcios; Consórcios; Consórcio Serviços; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Consórcios; Consórcios; Consórcio Náutico; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Pensions & Previdência; Previdência; PGBL – Renda Fixa; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Pensions & Previdência; Previdência; PGBL – Multimercado; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Pensions & Previdência; Previdência; PGBL – Ações; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Pensions & Previdência; Previdência; VGBL – Renda Fixa; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Pensions & Previdência; Previdência; VGBL – Multimercado; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Pensions & Previdência; Previdência; VGBL – Ações; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Pensions & Previdência; Previdência; Previdência Empresarial (Patrocinada); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Pensions & Previdência; Previdência; Previdência sob Medida (Fundo Exclusivo); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Corporate & Investment Banking; IB Services; M\&A Advisory; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Corporate & Investment Banking; IB Services; Underwriting – Debêntures (DCM); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Corporate & Investment Banking; IB Services; Underwriting – Ações/Follow‑on (ECM); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Corporate & Investment Banking; IB Services; Coordenação de IPO; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Corporate & Investment Banking; IB Services; Securitização (CRI/CRA/FIDC); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Corporate & Investment Banking; IB Services; Project Finance (Estruturação); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Corporate & Investment Banking; IB Services; Syndicated Loans (Coordenação); R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Tradicional; Corporate & Investment Banking; IB Services; Private Placements; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Corporate & Investment Banking; IB Services; Emissão de Letras Financeiras p/ Clientes; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Corporate & Investment Banking; Markets; Derivativos de Taxa de Juros (IRS); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Corporate & Investment Banking; Markets; Hedge de Commodities; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Corporate & Investment Banking; Markets; Structured Notes Corporativas; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Digital/Open Finance/Services; Pacotes; Cesta de Serviços Essencial PF; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Digital/Open Finance/Services; Pacotes; Cesta de Serviços Especial PF; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Digital/Open Finance/Services; Pacotes; Cesta de Serviços PJ; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Digital/Open Finance/Services; Serviços Digitais; Alertas e Notificações (SMS/App); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Digital/Open Finance/Services; Serviços Digitais; Gerenciador Financeiro Pessoal (PFM); R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Digital/Open Finance/Services; Serviços Cartões; Disputa/Chargeback Cartões; R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Tradicional; Digital/Open Finance/Services; Segurança; Token Físico (Chave de Segurança); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Digital/Open Finance/Services; Serviços Digitais; Cofre Digital de Documentos; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Digital/Open Finance/Services; Open Finance; Portal Open Finance – Consentimentos; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Digital/Open Finance/Services; Open Finance/APIs; API Pix para PJ; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Digital/Open Finance/Services; Open Finance/APIs; API de Dados de Conta/Transações; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Digital/Open Finance/Services; Segurança; Onboarding Digital KYC/KYB; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Tradicional; Digital/Open Finance/Services; Serviços Digitais; Educação/Score Financeiro; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Tradicional; Digital/Open Finance/Services; Serviços; Atendimento Priority/Concierge; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Custody; ; Custódia Fria Segregada (PF/Wealth); R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Crypto; Custody; ; Custódia Fria Segregada (Institucional); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Custody; ; Custódia MPC (Multi‑Party Computation); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Custody; ; Custódia com Staking (ETH/SOL); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Custody; ; Custódia com Seguro (Crime/Specie); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Custody; ; Custódia Off‑Exchange (Tri‑party); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Custody; ; Custódia de Stablecoins; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Custody; ; Custódia de Deposit Tokens; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Custody; ; Custódia de Tokens de T‑bills; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Custody; ; Escrow On‑chain; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Brokerage & Distribution; ; On‑ramp bancário (spot); R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Crypto; Brokerage & Distribution; ; Distribuição ETFs BTC (EUA); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Brokerage & Distribution; ; Distribuição ETFs ETH (EUA); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Brokerage & Distribution; ; Distribuição ETPs (Europa); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Brokerage & Distribution; ; Fundos de Fundos Cripto; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Brokerage & Distribution; ; Índices/Baskets (BTC+ETH); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Brokerage & Distribution; ; ETFs de Miners/Infra; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Crypto; Brokerage & Distribution; ; Notas Privadas 144A/Reg S; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Brokerage & Distribution; ; Advisory & Research; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Brokerage & Distribution; ; Tax/Lot & Consolidação; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Brokerage & Distribution; ; DCA Programado; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Crypto; Brokerage & Distribution; ; OTC Spot (Mesa); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Credit & Financing; ; Lombard vs BTC; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Credit & Financing; ; Lombard vs ETH; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Credit & Financing; ; Lombard vs Staked ETH; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Credit & Financing; ; Lombard vs SOL/XRP; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Credit & Financing; ; Microcrédito Colateralizado; R$ 8.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 869,74; R$ 602,52; R$ 267,22; —***  
***Crypto; Credit & Financing; ; Overdraft Garantido (Cripto); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Credit & Financing; ; Financiamento com Recebíveis Tokenizados; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Credit & Financing; ; Repo vs BTC/ETFs BTC; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Credit & Financing; ; Trade Finance c/ Colateral Cripto; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Credit & Financing; ; SBL vs ETFs BTC/ETH; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Credit & Financing; ; Inventário p/ Market‑Making; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Credit & Financing; ; Syndicated Loan c/ Colateral Cripto; R$ 100.000,00; 4.50% a.m.; 3.38% a.m.; 180; R$ 30.226,01; R$ 22.037,45; R$ 8.188,56; —***  
***Crypto; Derivatives & Hedging; ; Futuros BTC (CME); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Opções BTC (CME); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Futuros ETH (CME); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Opções ETH (CME); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Futuros SOL (CME); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Futuros XRP (CME); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; NDF BTC (OTC); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; TRS BTC; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; TRS ETH/Basket; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Swap de Volatilidade; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; IRS Staking Yield (ETH); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Opções OTC Exóticas; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Hedge Basis (BTIC); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Swaps USD‑Stablecoin; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Forwards On‑chain; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Opções Semanais (BTC/ETH); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Calendar/Diagonal Spreads; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Protective Puts; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Covered Calls; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Derivatives & Hedging; ; Quanto Swaps (BTC‑USD/BRL); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; Capital Protegido BTC (Bond+Call); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; Capital Protegido ETH; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; Autocallable BTC (Phoenix); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; Autocallable ETH; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; Barrier Reverse Convertible BTC; R$ 200.000,00; 2.50% a.m.; 1.62% a.m.; 45; R$ 7.546,68; R$ 4.894,75; R$ 2.651,93; —***  
***Crypto; Structured Notes & COEs; ; Dual Currency BTC/USDC; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; Dual Currency ETH/USDC; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; Range Accrual BTC; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; Twin‑Win BTC; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; COE Multi‑Ativos (BTC+ETH+Ouro); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; Structured Note Tokenizada (ETH); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; CLN Miners/Exchanges; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; Proteção Parcial (95%); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; Indexadas à Vol (BTC); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; Basket c/ Rebalance; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Structured Notes & COEs; ; Cupom de Staking (ETH); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; Conta PJ em Stablecoin; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; Cross‑border em Stablecoin; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; Cash Sweep p/ Stablecoin; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; Deposit Tokens (JPMD/Citi); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; Escrow Supply Chain; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; Folha/Provisões em Stablecoin; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; Settlement Merchant em Stablecoin; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; FX on‑chain (USD–BRL); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; Open Finance \+ Cripto; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; NF/Comprovantes on‑chain; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; Citi Token Services (Cash); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; Stablecoin Bancária (EURCV/USDCV); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; Pagamentos com Deposit Token \+ FX; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Treasury & Payments; ; Treasury Dashboard On‑chain; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Prime & Institutional Services; ; Prime Brokerage Cripto; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Prime & Institutional Services; ; Liquidez Multi‑Venue; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Prime & Institutional Services; ; Tri‑party Collateral Mgmt; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Prime & Institutional Services; ; Risco & Travel Rule; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Prime & Institutional Services; ; Settlement DVP on‑chain; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Prime & Institutional Services; ; Controle de Rehipoteca; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Prime & Institutional Services; ; Proof‑of‑Reserves (PoR); R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Prime & Institutional Services; ; Lend/Borrow de Ativos; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Tokenization & RWAs; ; Distribuição de T‑Bills Tokenizados; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Tokenization & RWAs; ; Securitização de Recebíveis; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Tokenization & RWAs; ; Tokenização de Dívida Corp.; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Tokenization & RWAs; ; Equity Privado Tokenizado; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Tokenization & RWAs; ; Fundos Tokenizados; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Tokenization & RWAs; ; Imobiliário Tokenizado; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Tokenization & RWAs; ; Notas Estruturadas Tokenizadas; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***  
***Crypto; Tokenization & RWAs; ; Programa de Stablecoin Bancária; R$ 160.000,00; 3.50% a.m.; 2.45% a.m.; 90; R$ 17.394,86; R$ 12.050,47; R$ 5.344,39; —***

# **Fichas XL — por produto (conteúdo limpo)**

## **Conta Corrente PF**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Contas  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Conta Corrente PF integra a família Accounts & Deposits, subfamília Contas. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Conta Corrente PJ**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Contas  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Conta Corrente PJ integra a família Accounts & Deposits, subfamília Contas. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Conta Salário**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Contas  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Conta Salário integra a família Accounts & Deposits, subfamília Contas. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Conta Universitária**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Contas  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Conta Universitária integra a família Accounts & Deposits, subfamília Contas. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Conta MEI**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Contas  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Conta MEI integra a família Accounts & Deposits, subfamília Contas. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Poupança**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Depósitos  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Poupança integra a família Accounts & Deposits, subfamília Depósitos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **CDB Pós‑CDI**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Depósitos a prazo  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): CDB Pós‑CDI integra a família Accounts & Deposits, subfamília Depósitos a prazo. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **CDB Prefixado**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Depósitos a prazo  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): CDB Prefixado integra a família Accounts & Deposits, subfamília Depósitos a prazo. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **CDB Escalonado**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Depósitos a prazo  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): CDB Escalonado integra a família Accounts & Deposits, subfamília Depósitos a prazo. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **LCI**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Depósitos a prazo  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): LCI integra a família Accounts & Deposits, subfamília Depósitos a prazo. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **LCA**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Depósitos a prazo  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): LCA integra a família Accounts & Deposits, subfamília Depósitos a prazo. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **LC (Letra de Câmbio)**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Depósitos a prazo  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): LC (Letra de Câmbio) integra a família Accounts & Deposits, subfamília Depósitos a prazo. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **LF (Letra Financeira)**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Depósitos a prazo  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): LF (Letra Financeira) integra a família Accounts & Deposits, subfamília Depósitos a prazo. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Conta Pagamento (Carteira Digital)**

Domínio: Tradicional  
Família / Subfamília: Accounts & Deposits / Contas  
Persona: Ambos  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Conta Pagamento (Carteira Digital) integra a família Accounts & Deposits, subfamília Contas. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **PIX Transferência**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / PIX  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): PIX Transferência integra a família Payments & Transfers, subfamília PIX. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **PIX Cobrança (QR Dinâmico)**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / PIX  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): PIX Cobrança (QR Dinâmico) integra a família Payments & Transfers, subfamília PIX. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **PIX Saque**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / PIX  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): PIX Saque integra a família Payments & Transfers, subfamília PIX. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **PIX Troco**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / PIX  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): PIX Troco integra a família Payments & Transfers, subfamília PIX. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **TED**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Transferências  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): TED integra a família Payments & Transfers, subfamília Transferências. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **SWIFT Internacional**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Transferências  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): SWIFT Internacional integra a família Payments & Transfers, subfamília Transferências. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Boleto – Emissão**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Cobrança  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Boleto – Emissão integra a família Payments & Transfers, subfamília Cobrança. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Boleto – Cobrança Registrada**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Cobrança  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Boleto – Cobrança Registrada integra a família Payments & Transfers, subfamília Cobrança. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Débito Automático**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Pagamentos  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Débito Automático integra a família Payments & Transfers, subfamília Pagamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **DDA (Débito Direto Autorizado)**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Pagamentos  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): DDA (Débito Direto Autorizado) integra a família Payments & Transfers, subfamília Pagamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Agendamento de Pagamentos**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Pagamentos  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Agendamento de Pagamentos integra a família Payments & Transfers, subfamília Pagamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Pagamento de Tributos**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Pagamentos  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Pagamento de Tributos integra a família Payments & Transfers, subfamília Pagamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Tokenização Carteiras (Apple/Google Pay)**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Pagamentos  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Tokenização Carteiras (Apple/Google Pay) integra a família Payments & Transfers, subfamília Pagamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Link de Pagamento**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Cobrança  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Link de Pagamento integra a família Payments & Transfers, subfamília Cobrança. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Split de Pagamentos**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Cobrança  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Split de Pagamentos integra a família Payments & Transfers, subfamília Cobrança. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Marketplace  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **QR Code Estático Loja**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Cobrança  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): QR Code Estático Loja integra a família Payments & Transfers, subfamília Cobrança. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Gateway de Pagamentos**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / PSP/Acquiring  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Gateway de Pagamentos integra a família Payments & Transfers, subfamília PSP/Acquiring. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Assinaturas/Recorrência**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Cobrança  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Assinaturas/Recorrência integra a família Payments & Transfers, subfamília Cobrança. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Pagamento por Aproximação (NFC)**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Pagamentos  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Pagamento por Aproximação (NFC) integra a família Payments & Transfers, subfamília Pagamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Portal de Cobranças PJ**

Domínio: Tradicional  
Família / Subfamília: Payments & Transfers / Cobrança  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Portal de Cobranças PJ integra a família Payments & Transfers, subfamília Cobrança. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Cartão de Débito**

Domínio: Tradicional  
Família / Subfamília: Cards / Débito  
Persona: Ambos  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Cartão de Débito integra a família Cards, subfamília Débito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **Cartão de Crédito Internacional**

Domínio: Tradicional  
Família / Subfamília: Cards / Crédito  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cartão de Crédito Internacional integra a família Cards, subfamília Crédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Cartão Gold**

Domínio: Tradicional  
Família / Subfamília: Cards / Crédito  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cartão Gold integra a família Cards, subfamília Crédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Cartão Platinum**

Domínio: Tradicional  
Família / Subfamília: Cards / Crédito  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cartão Platinum integra a família Cards, subfamília Crédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Cartão Black/Infinite**

Domínio: Tradicional  
Família / Subfamília: Cards / Crédito  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cartão Black/Infinite integra a família Cards, subfamília Crédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Cartão Empresarial (Business)**

Domínio: Tradicional  
Família / Subfamília: Cards / Crédito  
Persona: PJ  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Cartão Empresarial (Business) integra a família Cards, subfamília Crédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **Cartão Corporate (T\&E)**

Domínio: Tradicional  
Família / Subfamília: Cards / Crédito  
Persona: EPP  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Cartão Corporate (T\&E) integra a família Cards, subfamília Crédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **Cartão Pré‑pago**

Domínio: Tradicional  
Família / Subfamília: Cards / Pré‑pago  
Persona: Ambos  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Cartão Pré‑pago integra a família Cards, subfamília Pré‑pago. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **Cartão Co‑branded/Private Label**

Domínio: Tradicional  
Família / Subfamília: Cards / Crédito  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cartão Co‑branded/Private Label integra a família Cards, subfamília Crédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Cartão Consignado**

Domínio: Tradicional  
Família / Subfamília: Cards / Crédito  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cartão Consignado integra a família Cards, subfamília Crédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Cartão com Garantia (Secured)**

Domínio: Tradicional  
Família / Subfamília: Cards / Crédito  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cartão com Garantia (Secured) integra a família Cards, subfamília Crédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Cartão Adicional**

Domínio: Tradicional  
Família / Subfamília: Cards / Crédito  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cartão Adicional integra a família Cards, subfamília Crédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Cartão Virtual**

Domínio: Tradicional  
Família / Subfamília: Cards / Crédito/Débito  
Persona: Ambos  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Cartão Virtual integra a família Cards, subfamília Crédito/Débito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **Cartão Multimoeda (Travel)**

Domínio: Tradicional  
Família / Subfamília: Cards / Pré‑pago  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cartão Multimoeda (Travel) integra a família Cards, subfamília Pré‑pago. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Parcelamento de Fatura**

Domínio: Tradicional  
Família / Subfamília: Cards / Serviços ao Cartão  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Parcelamento de Fatura integra a família Cards, subfamília Serviços ao Cartão. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Rotativo Gerenciado**

Domínio: Tradicional  
Família / Subfamília: Cards / Serviços ao Cartão  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Rotativo Gerenciado integra a família Cards, subfamília Serviços ao Cartão. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Programa de Pontos/Milhas**

Domínio: Tradicional  
Família / Subfamília: Cards / Serviços ao Cartão  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Programa de Pontos/Milhas integra a família Cards, subfamília Serviços ao Cartão. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Cashback**

Domínio: Tradicional  
Família / Subfamília: Cards / Serviços ao Cartão  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cashback integra a família Cards, subfamília Serviços ao Cartão. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Proteção de Compra/Preço**

Domínio: Tradicional  
Família / Subfamília: Cards / Serviços ao Cartão  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Proteção de Compra/Preço integra a família Cards, subfamília Serviços ao Cartão. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Limite Garantido por CDB**

Domínio: Tradicional  
Família / Subfamília: Cards / Crédito  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Limite Garantido por CDB integra a família Cards, subfamília Crédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Empréstimo Pessoal**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Crédito PF  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Empréstimo Pessoal integra a família Loans \- Retail, subfamília Crédito PF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Consignado INSS**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Crédito PF  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Consignado INSS integra a família Loans \- Retail, subfamília Crédito PF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Consignado Privado**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Crédito PF  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Consignado Privado integra a família Loans \- Retail, subfamília Crédito PF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Cheque Especial (Overdraft)**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Crédito PF  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cheque Especial (Overdraft) integra a família Loans \- Retail, subfamília Crédito PF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Parcelamento do Cheque Especial**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Crédito PF  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Parcelamento do Cheque Especial integra a família Loans \- Retail, subfamília Crédito PF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Antecipação 13º Salário**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Crédito PF  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Antecipação 13º Salário integra a família Loans \- Retail, subfamília Crédito PF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Antecipação Restituição IR**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Crédito PF  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Antecipação Restituição IR integra a família Loans \- Retail, subfamília Crédito PF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Home Equity (Garantia de Imóvel)**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Crédito PF  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Home Equity (Garantia de Imóvel) integra a família Loans \- Retail, subfamília Crédito PF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Crédito com Garantia de Veículo**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Crédito PF  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Crédito com Garantia de Veículo integra a família Loans \- Retail, subfamília Crédito PF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Crédito com Garantia de Investimento**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Crédito PF  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Crédito com Garantia de Investimento integra a família Loans \- Retail, subfamília Crédito PF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Financiamento de Veículos (CDC)**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Financiamentos  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Financiamento de Veículos (CDC) integra a família Loans \- Retail, subfamília Financiamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Financiamento Imobiliário SFH**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Financiamentos  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Financiamento Imobiliário SFH integra a família Loans \- Retail, subfamília Financiamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Financiamento Imobiliário SFI**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Financiamentos  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Financiamento Imobiliário SFI integra a família Loans \- Retail, subfamília Financiamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Portabilidade de Crédito Imobiliário**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Financiamentos  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Portabilidade de Crédito Imobiliário integra a família Loans \- Retail, subfamília Financiamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Refinanciamento de Veículo**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Financiamentos  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Refinanciamento de Veículo integra a família Loans \- Retail, subfamília Financiamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Crediário/BNPL via Banco**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Financiamentos  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Crediário/BNPL via Banco integra a família Loans \- Retail, subfamília Financiamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Crédito Educacional**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Financiamentos  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Crédito Educacional integra a família Loans \- Retail, subfamília Financiamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Microcrédito PF**

Domínio: Tradicional  
Família / Subfamília: Loans \- Retail / Microcrédito  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Microcrédito PF integra a família Loans \- Retail, subfamília Microcrédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 2.418,08 | Custo com você (R$): R$ 1.763,00 | Economia (R$): R$ 655,08

## **Capital de Giro**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Crédito PJ  
Persona: PJ  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): Capital de Giro integra a família Loans \- SME/Corp, subfamília Crédito PJ. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Cheque Especial PJ**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Crédito PJ  
Persona: PJ  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): Cheque Especial PJ integra a família Loans \- SME/Corp, subfamília Crédito PJ. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Conta Garantida**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Crédito PJ  
Persona: PJ  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): Conta Garantida integra a família Loans \- SME/Corp, subfamília Crédito PJ. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Giro com Trava de Recebíveis**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Crédito PJ  
Persona: PJ  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): Giro com Trava de Recebíveis integra a família Loans \- SME/Corp, subfamília Crédito PJ. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Desconto de Duplicatas**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Crédito PJ  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Desconto de Duplicatas integra a família Loans \- SME/Corp, subfamília Crédito PJ. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Antecipação de Recebíveis de Cartão**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Crédito PJ  
Persona: PJ  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Antecipação de Recebíveis de Cartão integra a família Loans \- SME/Corp, subfamília Crédito PJ. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **NCE/CCE**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Crédito PJ  
Persona: PJ  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): NCE/CCE integra a família Loans \- SME/Corp, subfamília Crédito PJ. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **BNDES FINAME (repasse)**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Crédito PJ  
Persona: PJ  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): BNDES FINAME (repasse) integra a família Loans \- SME/Corp, subfamília Crédito PJ. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **BNDES Automático**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Crédito PJ  
Persona: PJ  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): BNDES Automático integra a família Loans \- SME/Corp, subfamília Crédito PJ. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **ACC (Adiantamento Contrato de Câmbio)**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Trade/Crédito PJ  
Persona: PJ  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): ACC (Adiantamento Contrato de Câmbio) integra a família Loans \- SME/Corp, subfamília Trade/Crédito PJ. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Exportador  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **ACE (Adiantamento Cambiais Entregues)**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Trade/Crédito PJ  
Persona: PJ  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): ACE (Adiantamento Cambiais Entregues) integra a família Loans \- SME/Corp, subfamília Trade/Crédito PJ. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Exportador  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Financiamento Máquinas/Equipamentos**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Financiamentos  
Persona: PJ  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): Financiamento Máquinas/Equipamentos integra a família Loans \- SME/Corp, subfamília Financiamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Financiamento de Veículos PJ**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Financiamentos  
Persona: PJ  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): Financiamento de Veículos PJ integra a família Loans \- SME/Corp, subfamília Financiamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Crédito para Construção/Real Estate Corp**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Financiamentos  
Persona: EPP  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): Crédito para Construção/Real Estate Corp integra a família Loans \- SME/Corp, subfamília Financiamentos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Project Finance**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Estruturado  
Persona: EPP  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): Project Finance integra a família Loans \- SME/Corp, subfamília Estruturado. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Empréstimo Sindicalizado**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Estruturado  
Persona: EPP  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): Empréstimo Sindicalizado integra a família Loans \- SME/Corp, subfamília Estruturado. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Linha Revolving (Standby)**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Crédito PJ  
Persona: EPP  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): Linha Revolving (Standby) integra a família Loans \- SME/Corp, subfamília Crédito PJ. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Microcrédito Produtivo Orientado**

Domínio: Tradicional  
Família / Subfamília: Loans \- SME/Corp / Microcrédito  
Persona: EPP  
Ticket padrão (R$): R$ 5.000,00  
Como funciona (XL): Microcrédito Produtivo Orientado integra a família Loans \- SME/Corp, subfamília Microcrédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: MEI/PME  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 5.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 1.511,30 | Custo com você (R$): R$ 1.101,87 | Economia (R$): R$ 409,43

## **Carta de Crédito – Importação**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / LCs  
Persona: PJ  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Carta de Crédito – Importação integra a família Trade Finance & Guarantees, subfamília LCs. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **Carta de Crédito – Exportação**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / LCs  
Persona: PJ  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Carta de Crédito – Exportação integra a família Trade Finance & Guarantees, subfamília LCs. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **Cobrança Documentária**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / Collections  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cobrança Documentária integra a família Trade Finance & Guarantees, subfamília Collections. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Remessas Diretas (Clean)**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / Collections  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Remessas Diretas (Clean) integra a família Trade Finance & Guarantees, subfamília Collections. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Forfaiting**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / Recebíveis  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Forfaiting integra a família Trade Finance & Guarantees, subfamília Recebíveis. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Confirming (Reverse Factoring)**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / SCF  
Persona: PJ  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Confirming (Reverse Factoring) integra a família Trade Finance & Guarantees, subfamília SCF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **Supply Chain Finance (SCF)**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / SCF  
Persona: PJ  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Supply Chain Finance (SCF) integra a família Trade Finance & Guarantees, subfamília SCF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **Invoice Discounting Internacional**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / Recebíveis  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Invoice Discounting Internacional integra a família Trade Finance & Guarantees, subfamília Recebíveis. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Garantia – Bid Bond**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / Garantias  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Garantia – Bid Bond integra a família Trade Finance & Guarantees, subfamília Garantias. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Garantia – Performance Bond**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / Garantias  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Garantia – Performance Bond integra a família Trade Finance & Guarantees, subfamília Garantias. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Garantia – Advance Payment**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / Garantias  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Garantia – Advance Payment integra a família Trade Finance & Guarantees, subfamília Garantias. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Garantia – Maintenance**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / Garantias  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Garantia – Maintenance integra a família Trade Finance & Guarantees, subfamília Garantias. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Standby Letter of Credit (SBLC)**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / Garantias  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Standby Letter of Credit (SBLC) integra a família Trade Finance & Guarantees, subfamília Garantias. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Aval em Títulos**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / Garantias  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Aval em Títulos integra a família Trade Finance & Guarantees, subfamília Garantias. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Seguro Garantia (via banco)**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / Garantias  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Seguro Garantia (via banco) integra a família Trade Finance & Guarantees, subfamília Garantias. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Trade Loans (Pós‑Shipment)**

Domínio: Tradicional  
Família / Subfamília: Trade Finance & Guarantees / Trade Loans  
Persona: PJ  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): Trade Loans (Pós‑Shipment) integra a família Trade Finance & Guarantees, subfamília Trade Loans. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Folha de Pagamento (Payroll)**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Cash Mgmt  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Folha de Pagamento (Payroll) integra a família Cash Management & Merchant, subfamília Cash Mgmt. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Gestão de Contas a Pagar (AP)**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Cash Mgmt  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Gestão de Contas a Pagar (AP) integra a família Cash Management & Merchant, subfamília Cash Mgmt. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Gestão de Contas a Receber (AR)**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Cash Mgmt  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Gestão de Contas a Receber (AR) integra a família Cash Management & Merchant, subfamília Cash Mgmt. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Conciliação Bancária Automática**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Cash Mgmt  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Conciliação Bancária Automática integra a família Cash Management & Merchant, subfamília Cash Mgmt. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Extratos CNAB/EDI**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Cash Mgmt  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Extratos CNAB/EDI integra a família Cash Management & Merchant, subfamília Cash Mgmt. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Lockbox**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Cash Mgmt  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Lockbox integra a família Cash Management & Merchant, subfamília Cash Mgmt. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Varredura (Sweeping) de Contas**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Cash Mgmt  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Varredura (Sweeping) de Contas integra a família Cash Management & Merchant, subfamília Cash Mgmt. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Pooling de Caixa (Notional/Physical)**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Cash Mgmt  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Pooling de Caixa (Notional/Physical) integra a família Cash Management & Merchant, subfamília Cash Mgmt. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Pagamentos Massivos (Lotes)**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Cash Mgmt  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Pagamentos Massivos (Lotes) integra a família Cash Management & Merchant, subfamília Cash Mgmt. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Split de Recebíveis Marketplace**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Acquiring  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Split de Recebíveis Marketplace integra a família Cash Management & Merchant, subfamília Acquiring. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Subadquirência (White‑label)**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Acquiring  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Subadquirência (White‑label) integra a família Cash Management & Merchant, subfamília Acquiring. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **POS – Aluguel/Comodato**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Acquiring  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): POS – Aluguel/Comodato integra a família Cash Management & Merchant, subfamília Acquiring. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Gateway de Pagamento Enterprise**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Acquiring  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Gateway de Pagamento Enterprise integra a família Cash Management & Merchant, subfamília Acquiring. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Antifraude Transacional**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Acquiring  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Antifraude Transacional integra a família Cash Management & Merchant, subfamília Acquiring. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **API Banking (Contas/Pagamentos)**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / APIs  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): API Banking (Contas/Pagamentos) integra a família Cash Management & Merchant, subfamília APIs. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Contas Virtuais (Virtual Accounts)**

Domínio: Tradicional  
Família / Subfamília: Cash Management & Merchant / Cash Mgmt  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Contas Virtuais (Virtual Accounts) integra a família Cash Management & Merchant, subfamília Cash Mgmt. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Tesouro Selic**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Government Bonds  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Tesouro Selic integra a família Investments \- Fixed Income, subfamília Government Bonds. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Tesouro Prefixado**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Government Bonds  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Tesouro Prefixado integra a família Investments \- Fixed Income, subfamília Government Bonds. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Tesouro IPCA+**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Government Bonds  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Tesouro IPCA+ integra a família Investments \- Fixed Income, subfamília Government Bonds. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **CDB Pós‑CDI**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Bank Bonds  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): CDB Pós‑CDI integra a família Investments \- Fixed Income, subfamília Bank Bonds. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **CDB Prefixado**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Bank Bonds  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): CDB Prefixado integra a família Investments \- Fixed Income, subfamília Bank Bonds. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **CDB Escalonado**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Bank Bonds  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): CDB Escalonado integra a família Investments \- Fixed Income, subfamília Bank Bonds. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **LCI**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Bank Bonds  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): LCI integra a família Investments \- Fixed Income, subfamília Bank Bonds. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **LCA**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Bank Bonds  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): LCA integra a família Investments \- Fixed Income, subfamília Bank Bonds. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **LC (Letra de Câmbio)**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Finance Companies  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): LC (Letra de Câmbio) integra a família Investments \- Fixed Income, subfamília Finance Companies. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Debêntures Simples**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Corporate Bonds  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Debêntures Simples integra a família Investments \- Fixed Income, subfamília Corporate Bonds. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Debêntures Incentivadas (Infra)**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Corporate Bonds  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Debêntures Incentivadas (Infra) integra a família Investments \- Fixed Income, subfamília Corporate Bonds. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **CRA**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Securitização  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): CRA integra a família Investments \- Fixed Income, subfamília Securitização. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **CRI**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Securitização  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): CRI integra a família Investments \- Fixed Income, subfamília Securitização. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Letras Financeiras (LF)**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Bank Bonds  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Letras Financeiras (LF) integra a família Investments \- Fixed Income, subfamília Bank Bonds. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **DPGE**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Bank Bonds  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): DPGE integra a família Investments \- Fixed Income, subfamília Bank Bonds. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Nota Promissória Comercial**

Domínio: Tradicional  
Família / Subfamília: Investments \- Fixed Income / Corporate Bonds  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Nota Promissória Comercial integra a família Investments \- Fixed Income, subfamília Corporate Bonds. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundo DI**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Fundos RF  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Fundo DI integra a família Investments \- Funds/ETFs/COE, subfamília Fundos RF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundo RF Crédito Privado**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Fundos RF  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Fundo RF Crédito Privado integra a família Investments \- Funds/ETFs/COE, subfamília Fundos RF. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundo Multimercado Macro**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Multimercados  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Fundo Multimercado Macro integra a família Investments \- Funds/ETFs/COE, subfamília Multimercados. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundo Long & Short Neutro**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Multimercados  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Fundo Long & Short Neutro integra a família Investments \- Funds/ETFs/COE, subfamília Multimercados. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundo Cambial Dólar**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Cambiais  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Fundo Cambial Dólar integra a família Investments \- Funds/ETFs/COE, subfamília Cambiais. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundo de Ações Ibovespa Ativo**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Ações  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Fundo de Ações Ibovespa Ativo integra a família Investments \- Funds/ETFs/COE, subfamília Ações. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundo de Ações Dividendos**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Ações  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Fundo de Ações Dividendos integra a família Investments \- Funds/ETFs/COE, subfamília Ações. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundo Small Caps**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Ações  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Fundo Small Caps integra a família Investments \- Funds/ETFs/COE, subfamília Ações. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundo Setorial (Infra/Utilidades)**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Ações  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Fundo Setorial (Infra/Utilidades) integra a família Investments \- Funds/ETFs/COE, subfamília Ações. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundo Quantitativo**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Multimercados  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Fundo Quantitativo integra a família Investments \- Funds/ETFs/COE, subfamília Multimercados. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundo ESG**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Ações/MM  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Fundo ESG integra a família Investments \- Funds/ETFs/COE, subfamília Ações/MM. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundo Internacional Global Equity**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Ações  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Fundo Internacional Global Equity integra a família Investments \- Funds/ETFs/COE, subfamília Ações. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundo Multimercado com Proteção**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Multimercados  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Fundo Multimercado com Proteção integra a família Investments \- Funds/ETFs/COE, subfamília Multimercados. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **ETF Ibovespa (ex. BOVA11)**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / ETFs  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): ETF Ibovespa (ex. BOVA11) integra a família Investments \- Funds/ETFs/COE, subfamília ETFs. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **ETF S\&P 500 (ex. IVVB11)**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / ETFs  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): ETF S\&P 500 (ex. IVVB11) integra a família Investments \- Funds/ETFs/COE, subfamília ETFs. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **ETF de Renda Fixa**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / ETFs  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): ETF de Renda Fixa integra a família Investments \- Funds/ETFs/COE, subfamília ETFs. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **ETF Setorial/Temático**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / ETFs  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): ETF Setorial/Temático integra a família Investments \- Funds/ETFs/COE, subfamília ETFs. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **FII – Tijolo**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Imobiliários  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): FII – Tijolo integra a família Investments \- Funds/ETFs/COE, subfamília Imobiliários. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **FII – Papel**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Imobiliários  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): FII – Papel integra a família Investments \- Funds/ETFs/COE, subfamília Imobiliários. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **FIDC**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Crédito Estruturado  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): FIDC integra a família Investments \- Funds/ETFs/COE, subfamília Crédito Estruturado. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Investidor Qualificado  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **COE – Autocallable**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / COE  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): COE – Autocallable integra a família Investments \- Funds/ETFs/COE, subfamília COE. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **COE – Twin Win**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / COE  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): COE – Twin Win integra a família Investments \- Funds/ETFs/COE, subfamília COE. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **COE – Capital Protegido (Moeda)**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / COE  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): COE – Capital Protegido (Moeda) integra a família Investments \- Funds/ETFs/COE, subfamília COE. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Fundo Previdenciário (Estrutura Master‑Feeder)**

Domínio: Tradicional  
Família / Subfamília: Investments \- Funds/ETFs/COE / Previdência em fundos  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Fundo Previdenciário (Estrutura Master‑Feeder) integra a família Investments \- Funds/ETFs/COE, subfamília Previdência em fundos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Conta de Corretora / Home Broker**

Domínio: Tradicional  
Família / Subfamília: Brokerage/Wealth / Brokerage  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Conta de Corretora / Home Broker integra a família Brokerage/Wealth, subfamília Brokerage. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Custódia de Ativos**

Domínio: Tradicional  
Família / Subfamília: Brokerage/Wealth / Brokerage  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Custódia de Ativos integra a família Brokerage/Wealth, subfamília Brokerage. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Aluguel de Ações (SLB)**

Domínio: Tradicional  
Família / Subfamília: Brokerage/Wealth / Brokerage  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Aluguel de Ações (SLB) integra a família Brokerage/Wealth, subfamília Brokerage. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Margem para Operações**

Domínio: Tradicional  
Família / Subfamília: Brokerage/Wealth / Brokerage  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Margem para Operações integra a família Brokerage/Wealth, subfamília Brokerage. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Negociação de Opções**

Domínio: Tradicional  
Família / Subfamília: Brokerage/Wealth / Brokerage  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Negociação de Opções integra a família Brokerage/Wealth, subfamília Brokerage. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Acesso a Futuros (BM\&F)**

Domínio: Tradicional  
Família / Subfamília: Brokerage/Wealth / Brokerage  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Acesso a Futuros (BM\&F) integra a família Brokerage/Wealth, subfamília Brokerage. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Mesa de Operações Estruturadas**

Domínio: Tradicional  
Família / Subfamília: Brokerage/Wealth / Wealth  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Mesa de Operações Estruturadas integra a família Brokerage/Wealth, subfamília Wealth. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Carteira Administrada (DPM)**

Domínio: Tradicional  
Família / Subfamília: Brokerage/Wealth / Wealth  
Persona: EPP  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Carteira Administrada (DPM) integra a família Brokerage/Wealth, subfamília Wealth. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **Advisory de Investimentos**

Domínio: Tradicional  
Família / Subfamília: Brokerage/Wealth / Wealth  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Advisory de Investimentos integra a família Brokerage/Wealth, subfamília Wealth. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Family Office**

Domínio: Tradicional  
Família / Subfamília: Brokerage/Wealth / Wealth  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Family Office integra a família Brokerage/Wealth, subfamília Wealth. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Acesso Offshore**

Domínio: Tradicional  
Família / Subfamília: Brokerage/Wealth / Wealth  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Acesso Offshore integra a família Brokerage/Wealth, subfamília Wealth. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Planejamento Sucessório**

Domínio: Tradicional  
Família / Subfamília: Brokerage/Wealth / Wealth  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Planejamento Sucessório integra a família Brokerage/Wealth, subfamília Wealth. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Seguro de Vida Temporário**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Vida  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Seguro de Vida Temporário integra a família Insurance & Protection, subfamília Vida. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Seguro de Vida Resgatável**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Vida  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Seguro de Vida Resgatável integra a família Insurance & Protection, subfamília Vida. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Seguro Doenças Graves**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Vida  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Seguro Doenças Graves integra a família Insurance & Protection, subfamília Vida. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Acidentes Pessoais**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Vida  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Acidentes Pessoais integra a família Insurance & Protection, subfamília Vida. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Seguro Prestamista (Credit Life)**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Vida/Crédito  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Seguro Prestamista (Credit Life) integra a família Insurance & Protection, subfamília Vida/Crédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Proteção Financeira/Perda de Renda**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Vida/Crédito  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Proteção Financeira/Perda de Renda integra a família Insurance & Protection, subfamília Vida/Crédito. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Seguro Residencial**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Ramos Elementares  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Seguro Residencial integra a família Insurance & Protection, subfamília Ramos Elementares. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Seguro Condomínio**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Ramos Elementares  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Seguro Condomínio integra a família Insurance & Protection, subfamília Ramos Elementares. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Seguro Empresarial (Multirrisco)**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Ramos Elementares  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Seguro Empresarial (Multirrisco) integra a família Insurance & Protection, subfamília Ramos Elementares. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Seguro Automóvel**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Auto  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Seguro Automóvel integra a família Insurance & Protection, subfamília Auto. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Seguro Frotas**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Auto  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Seguro Frotas integra a família Insurance & Protection, subfamília Auto. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Seguro Viagem**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Viagem  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Seguro Viagem integra a família Insurance & Protection, subfamília Viagem. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Seguro Cartão (Compra Protegida)**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Afinidades  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Seguro Cartão (Compra Protegida) integra a família Insurance & Protection, subfamília Afinidades. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Garantia Estendida**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Afinidades  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Garantia Estendida integra a família Insurance & Protection, subfamília Afinidades. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Seguro Celular/Portáteis**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Afinidades  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Seguro Celular/Portáteis integra a família Insurance & Protection, subfamília Afinidades. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Seguro Cibernético PME**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Riscos Especiais  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Seguro Cibernético PME integra a família Insurance & Protection, subfamília Riscos Especiais. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **D\&O (Directors & Officers)**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Responsabilidade  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): D\&O (Directors & Officers) integra a família Insurance & Protection, subfamília Responsabilidade. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **E\&O (Responsabilidade Profissional)**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Responsabilidade  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): E\&O (Responsabilidade Profissional) integra a família Insurance & Protection, subfamília Responsabilidade. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Seguro Garantia (Surety)**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Garantias  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Seguro Garantia (Surety) integra a família Insurance & Protection, subfamília Garantias. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Seguro Rural/Agrícola**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Riscos Especiais  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Seguro Rural/Agrícola integra a família Insurance & Protection, subfamília Riscos Especiais. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Agro  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Saúde Coletivo (parceria)**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Saúde/Odont  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Saúde Coletivo (parceria) integra a família Insurance & Protection, subfamília Saúde/Odont. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Dental Coletivo**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Saúde/Odont  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Dental Coletivo integra a família Insurance & Protection, subfamília Saúde/Odont. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Seguro Transporte (Carga)**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Ramos Elementares  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Seguro Transporte (Carga) integra a família Insurance & Protection, subfamília Ramos Elementares. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Seguro Pet**

Domínio: Tradicional  
Família / Subfamília: Insurance & Protection / Afinidades  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Seguro Pet integra a família Insurance & Protection, subfamília Afinidades. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Câmbio Turismo (Espécie)**

Domínio: Tradicional  
Família / Subfamília: FX & Hedging / FX Retail  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Câmbio Turismo (Espécie) integra a família FX & Hedging, subfamília FX Retail. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Cartão Viagem Multimoeda**

Domínio: Tradicional  
Família / Subfamília: FX & Hedging / FX Retail  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cartão Viagem Multimoeda integra a família FX & Hedging, subfamília FX Retail. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 301,87 | Custo com você (R$): R$ 195,79 | Economia (R$): R$ 106,08

## **Remessa Internacional PF (Envio)**

Domínio: Tradicional  
Família / Subfamília: FX & Hedging / Remittances  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Remessa Internacional PF (Envio) integra a família FX & Hedging, subfamília Remittances. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Remessa Internacional PJ (Envio)**

Domínio: Tradicional  
Família / Subfamília: FX & Hedging / Remittances  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Remessa Internacional PJ (Envio) integra a família FX & Hedging, subfamília Remittances. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Recebimento do Exterior (Wire In)**

Domínio: Tradicional  
Família / Subfamília: FX & Hedging / Remittances  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Recebimento do Exterior (Wire In) integra a família FX & Hedging, subfamília Remittances. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Contrato de Câmbio Pronto**

Domínio: Tradicional  
Família / Subfamília: FX & Hedging / FX Wholesale  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Contrato de Câmbio Pronto integra a família FX & Hedging, subfamília FX Wholesale. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **NDF (Câmbio Futuro)**

Domínio: Tradicional  
Família / Subfamília: FX & Hedging / Derivativos  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): NDF (Câmbio Futuro) integra a família FX & Hedging, subfamília Derivativos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Swap Cambial**

Domínio: Tradicional  
Família / Subfamília: FX & Hedging / Derivativos  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Swap Cambial integra a família FX & Hedging, subfamília Derivativos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Opções de Moeda (Vanilla)**

Domínio: Tradicional  
Família / Subfamília: FX & Hedging / Derivativos  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Opções de Moeda (Vanilla) integra a família FX & Hedging, subfamília Derivativos. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Pagamentos Globais Massivos**

Domínio: Tradicional  
Família / Subfamília: FX & Hedging / Remittances  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Pagamentos Globais Massivos integra a família FX & Hedging, subfamília Remittances. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Hedge de Importação**

Domínio: Tradicional  
Família / Subfamília: FX & Hedging / FX Wholesale  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Hedge de Importação integra a família FX & Hedging, subfamília FX Wholesale. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Hedge de Exportação**

Domínio: Tradicional  
Família / Subfamília: FX & Hedging / FX Wholesale  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Hedge de Exportação integra a família FX & Hedging, subfamília FX Wholesale. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Consórcio Imobiliário**

Domínio: Tradicional  
Família / Subfamília: Consórcios / Consórcios  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Consórcio Imobiliário integra a família Consórcios, subfamília Consórcios. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Consórcio Automóvel**

Domínio: Tradicional  
Família / Subfamília: Consórcios / Consórcios  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Consórcio Automóvel integra a família Consórcios, subfamília Consórcios. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Consórcio Motos**

Domínio: Tradicional  
Família / Subfamília: Consórcios / Consórcios  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Consórcio Motos integra a família Consórcios, subfamília Consórcios. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Consórcio Caminhões/Máquinas**

Domínio: Tradicional  
Família / Subfamília: Consórcios / Consórcios  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Consórcio Caminhões/Máquinas integra a família Consórcios, subfamília Consórcios. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Consórcio Serviços**

Domínio: Tradicional  
Família / Subfamília: Consórcios / Consórcios  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Consórcio Serviços integra a família Consórcios, subfamília Consórcios. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Consórcio Náutico**

Domínio: Tradicional  
Família / Subfamília: Consórcios / Consórcios  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Consórcio Náutico integra a família Consórcios, subfamília Consórcios. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **PGBL – Renda Fixa**

Domínio: Tradicional  
Família / Subfamília: Pensions & Previdência / Previdência  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): PGBL – Renda Fixa integra a família Pensions & Previdência, subfamília Previdência. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **PGBL – Multimercado**

Domínio: Tradicional  
Família / Subfamília: Pensions & Previdência / Previdência  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): PGBL – Multimercado integra a família Pensions & Previdência, subfamília Previdência. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **PGBL – Ações**

Domínio: Tradicional  
Família / Subfamília: Pensions & Previdência / Previdência  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): PGBL – Ações integra a família Pensions & Previdência, subfamília Previdência. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **VGBL – Renda Fixa**

Domínio: Tradicional  
Família / Subfamília: Pensions & Previdência / Previdência  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): VGBL – Renda Fixa integra a família Pensions & Previdência, subfamília Previdência. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **VGBL – Multimercado**

Domínio: Tradicional  
Família / Subfamília: Pensions & Previdência / Previdência  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): VGBL – Multimercado integra a família Pensions & Previdência, subfamília Previdência. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **VGBL – Ações**

Domínio: Tradicional  
Família / Subfamília: Pensions & Previdência / Previdência  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): VGBL – Ações integra a família Pensions & Previdência, subfamília Previdência. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Previdência Empresarial (Patrocinada)**

Domínio: Tradicional  
Família / Subfamília: Pensions & Previdência / Previdência  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Previdência Empresarial (Patrocinada) integra a família Pensions & Previdência, subfamília Previdência. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Previdência sob Medida (Fundo Exclusivo)**

Domínio: Tradicional  
Família / Subfamília: Pensions & Previdência / Previdência  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Previdência sob Medida (Fundo Exclusivo) integra a família Pensions & Previdência, subfamília Previdência. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **M\&A Advisory**

Domínio: Tradicional  
Família / Subfamília: Corporate & Investment Banking / IB Services  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): M\&A Advisory integra a família Corporate & Investment Banking, subfamília IB Services. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Underwriting – Debêntures (DCM)**

Domínio: Tradicional  
Família / Subfamília: Corporate & Investment Banking / IB Services  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Underwriting – Debêntures (DCM) integra a família Corporate & Investment Banking, subfamília IB Services. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Underwriting – Ações/Follow‑on (ECM)**

Domínio: Tradicional  
Família / Subfamília: Corporate & Investment Banking / IB Services  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Underwriting – Ações/Follow‑on (ECM) integra a família Corporate & Investment Banking, subfamília IB Services. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Coordenação de IPO**

Domínio: Tradicional  
Família / Subfamília: Corporate & Investment Banking / IB Services  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Coordenação de IPO integra a família Corporate & Investment Banking, subfamília IB Services. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Securitização (CRI/CRA/FIDC)**

Domínio: Tradicional  
Família / Subfamília: Corporate & Investment Banking / IB Services  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Securitização (CRI/CRA/FIDC) integra a família Corporate & Investment Banking, subfamília IB Services. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Project Finance (Estruturação)**

Domínio: Tradicional  
Família / Subfamília: Corporate & Investment Banking / IB Services  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Project Finance (Estruturação) integra a família Corporate & Investment Banking, subfamília IB Services. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Syndicated Loans (Coordenação)**

Domínio: Tradicional  
Família / Subfamília: Corporate & Investment Banking / IB Services  
Persona: EPP  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): Syndicated Loans (Coordenação) integra a família Corporate & Investment Banking, subfamília IB Services. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Private Placements**

Domínio: Tradicional  
Família / Subfamília: Corporate & Investment Banking / IB Services  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Private Placements integra a família Corporate & Investment Banking, subfamília IB Services. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Emissão de Letras Financeiras p/ Clientes**

Domínio: Tradicional  
Família / Subfamília: Corporate & Investment Banking / IB Services  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Emissão de Letras Financeiras p/ Clientes integra a família Corporate & Investment Banking, subfamília IB Services. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Derivativos de Taxa de Juros (IRS)**

Domínio: Tradicional  
Família / Subfamília: Corporate & Investment Banking / Markets  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Derivativos de Taxa de Juros (IRS) integra a família Corporate & Investment Banking, subfamília Markets. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Hedge de Commodities**

Domínio: Tradicional  
Família / Subfamília: Corporate & Investment Banking / Markets  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Hedge de Commodities integra a família Corporate & Investment Banking, subfamília Markets. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Structured Notes Corporativas**

Domínio: Tradicional  
Família / Subfamília: Corporate & Investment Banking / Markets  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Structured Notes Corporativas integra a família Corporate & Investment Banking, subfamília Markets. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Cesta de Serviços Essencial PF**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Pacotes  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cesta de Serviços Essencial PF integra a família Digital/Open Finance/Services, subfamília Pacotes. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Cesta de Serviços Especial PF**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Pacotes  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Cesta de Serviços Especial PF integra a família Digital/Open Finance/Services, subfamília Pacotes. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Cesta de Serviços PJ**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Pacotes  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cesta de Serviços PJ integra a família Digital/Open Finance/Services, subfamília Pacotes. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Alertas e Notificações (SMS/App)**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Serviços Digitais  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Alertas e Notificações (SMS/App) integra a família Digital/Open Finance/Services, subfamília Serviços Digitais. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Gerenciador Financeiro Pessoal (PFM)**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Serviços Digitais  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Gerenciador Financeiro Pessoal (PFM) integra a família Digital/Open Finance/Services, subfamília Serviços Digitais. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Disputa/Chargeback Cartões**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Serviços Cartões  
Persona: Ambos  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Disputa/Chargeback Cartões integra a família Digital/Open Finance/Services, subfamília Serviços Cartões. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **Token Físico (Chave de Segurança)**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Segurança  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Token Físico (Chave de Segurança) integra a família Digital/Open Finance/Services, subfamília Segurança. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Cofre Digital de Documentos**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Serviços Digitais  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cofre Digital de Documentos integra a família Digital/Open Finance/Services, subfamília Serviços Digitais. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Portal Open Finance – Consentimentos**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Open Finance  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Portal Open Finance – Consentimentos integra a família Digital/Open Finance/Services, subfamília Open Finance. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **API Pix para PJ**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Open Finance/APIs  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): API Pix para PJ integra a família Digital/Open Finance/Services, subfamília Open Finance/APIs. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **API de Dados de Conta/Transações**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Open Finance/APIs  
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): API de Dados de Conta/Transações integra a família Digital/Open Finance/Services, subfamília Open Finance/APIs. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PJ/Fintechs  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Onboarding Digital KYC/KYB**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Segurança  
Persona: Ambos  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Onboarding Digital KYC/KYB integra a família Digital/Open Finance/Services, subfamília Segurança. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Educação/Score Financeiro**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Serviços Digitais  
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Educação/Score Financeiro integra a família Digital/Open Finance/Services, subfamília Serviços Digitais. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Atendimento Priority/Concierge**

Domínio: Tradicional  
Família / Subfamília: Digital/Open Finance/Services / Serviços  
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Atendimento Priority/Concierge integra a família Digital/Open Finance/Services, subfamília Serviços. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Custódia Fria Segregada (PF/Wealth)**

Domínio: Crypto  
Família / Subfamília: Custody /   
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Chaves em HSM/cold storage; segregação por conta. Custódia Fria Segregada (PF/Wealth) integra a família Custody, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PF alta renda/Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Custódia Fria Segregada (Institucional)**

Domínio: Crypto  
Família / Subfamília: Custody /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Carteiras segregadas; relatórios SOC2/ISAE. Custódia Fria Segregada (Institucional) integra a família Custody, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Gestoras/Family Offices  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Custódia MPC (Multi‑Party Computation)**

Domínio: Crypto  
Família / Subfamília: Custody /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Assinaturas distribuídas (MPC). Custódia MPC (Multi‑Party Computation) integra a família Custody, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional/MM  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Custódia com Staking (ETH/SOL)**

Domínio: Crypto  
Família / Subfamília: Custody /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Validação e repasse de yield. Custódia com Staking (ETH/SOL) integra a família Custody, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Custódia com Seguro (Crime/Specie)**

Domínio: Crypto  
Família / Subfamília: Custody /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cobertura para chaveamento/armazenagem. Custódia com Seguro (Crime/Specie) integra a família Custody, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Custódia Off‑Exchange (Tri‑party)**

Domínio: Crypto  
Família / Subfamília: Custody /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Ativos no banco; trading na exchange via alçadas. Custódia Off‑Exchange (Tri‑party) integra a família Custody, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional/MM  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Custódia de Stablecoins**

Domínio: Crypto  
Família / Subfamília: Custody /   
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Guarda e gestão USDC/USDT/EURCV/USDCV. Custódia de Stablecoins integra a família Custody, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Tesouraria PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Custódia de Deposit Tokens**

Domínio: Crypto  
Família / Subfamília: Custody /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Tokens bancários representando depósitos. Custódia de Deposit Tokens integra a família Custody, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp/Tesouraria  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Custódia de Tokens de T‑bills**

Domínio: Crypto  
Família / Subfamília: Custody /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Guarda de tokens de T‑bills/MMFs. Custódia de Tokens de T‑bills integra a família Custody, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Escrow On‑chain**

Domínio: Crypto  
Família / Subfamília: Custody /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Contas escrow multi‑sig/MPC. Escrow On‑chain integra a família Custody, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp/IB  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **On‑ramp bancário (spot)**

Domínio: Crypto  
Família / Subfamília: Brokerage & Distribution /   
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Compra de BTC/ETH no app do banco. On‑ramp bancário (spot) integra a família Brokerage & Distribution, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Varejo/Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Distribuição ETFs BTC (EUA)**

Domínio: Crypto  
Família / Subfamília: Brokerage & Distribution /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Acesso aos 12 ETFs BTC spot. Distribuição ETFs BTC (EUA) integra a família Brokerage & Distribution, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Distribuição ETFs ETH (EUA)**

Domínio: Crypto  
Família / Subfamília: Brokerage & Distribution /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Acesso aos ETFs ETH spot. Distribuição ETFs ETH (EUA) integra a família Brokerage & Distribution, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Distribuição ETPs (Europa)**

Domínio: Crypto  
Família / Subfamília: Brokerage & Distribution /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): ETNs/ETCs/ETFs single‑asset/cestas. Distribuição ETPs (Europa) integra a família Brokerage & Distribution, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundos de Fundos Cripto**

Domínio: Crypto  
Família / Subfamília: Brokerage & Distribution /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): FoF entre ETPs/gestores. Fundos de Fundos Cripto integra a família Brokerage & Distribution, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Índices/Baskets (BTC+ETH)**

Domínio: Crypto  
Família / Subfamília: Brokerage & Distribution /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cestas via nota/ETP/mandato. Índices/Baskets (BTC+ETH) integra a família Brokerage & Distribution, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **ETFs de Miners/Infra**

Domínio: Crypto  
Família / Subfamília: Brokerage & Distribution /   
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Ações de mineração/infra. ETFs de Miners/Infra integra a família Brokerage & Distribution, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Varejo/Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Notas Privadas 144A/Reg S**

Domínio: Crypto  
Família / Subfamília: Brokerage & Distribution /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Veículos privados qualificados. Notas Privadas 144A/Reg S integra a família Brokerage & Distribution, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Inst./Wealth qualif.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Advisory & Research**

Domínio: Crypto  
Família / Subfamília: Brokerage & Distribution /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Relatórios e alocação tática. Advisory & Research integra a família Brokerage & Distribution, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Tax/Lot & Consolidação**

Domínio: Crypto  
Família / Subfamília: Brokerage & Distribution /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Relatórios e harvesting. Tax/Lot & Consolidação integra a família Brokerage & Distribution, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **DCA Programado**

Domínio: Crypto  
Família / Subfamília: Brokerage & Distribution /   
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Aportes recorrentes (DCA). DCA Programado integra a família Brokerage & Distribution, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Varejo/Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **OTC Spot (Mesa)**

Domínio: Crypto  
Família / Subfamília: Brokerage & Distribution /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Blocos via RFQ; DVP. OTC Spot (Mesa) integra a família Brokerage & Distribution, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Inst./Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Lombard vs BTC**

Domínio: Crypto  
Família / Subfamília: Credit & Financing /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Crédito com LTV 30–60%. Lombard vs BTC integra a família Credit & Financing, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Lombard vs ETH**

Domínio: Crypto  
Família / Subfamília: Credit & Financing /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Crédito com ETH colateral. Lombard vs ETH integra a família Credit & Financing, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Lombard vs Staked ETH**

Domínio: Crypto  
Família / Subfamília: Credit & Financing /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Mantém staking; LTV menor. Lombard vs Staked ETH integra a família Credit & Financing, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Lombard vs SOL/XRP**

Domínio: Crypto  
Família / Subfamília: Credit & Financing /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Alt blue‑chips com LTV 20–40%. Lombard vs SOL/XRP integra a família Credit & Financing, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Microcrédito Colateralizado**

Domínio: Crypto  
Família / Subfamília: Credit & Financing /   
Persona: PF  
Ticket padrão (R$): R$ 8.000,00  
Como funciona (XL): Limites baixos, varejo. Microcrédito Colateralizado integra a família Credit & Financing, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Varejo  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 8.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 869,74 | Custo com você (R$): R$ 602,52 | Economia (R$): R$ 267,22

## **Overdraft Garantido (Cripto)**

Domínio: Crypto  
Família / Subfamília: Credit & Financing /   
Persona: PJ  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cheque especial com colateral. Overdraft Garantido (Cripto) integra a família Credit & Financing, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/PJ  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Financiamento com Recebíveis Tokenizados**

Domínio: Crypto  
Família / Subfamília: Credit & Financing /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cessão on‑chain. Financiamento com Recebíveis Tokenizados integra a família Credit & Financing, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PME/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Repo vs BTC/ETFs BTC**

Domínio: Crypto  
Família / Subfamília: Credit & Financing /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Repos com ETFs/spot. Repo vs BTC/ETFs BTC integra a família Credit & Financing, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Trade Finance c/ Colateral Cripto**

Domínio: Crypto  
Família / Subfamília: Credit & Financing /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): ACC/ACE com garantia extra. Trade Finance c/ Colateral Cripto integra a família Credit & Financing, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Exportadores  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **SBL vs ETFs BTC/ETH**

Domínio: Crypto  
Família / Subfamília: Credit & Financing /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Empréstimo com ETFs spot. SBL vs ETFs BTC/ETH integra a família Credit & Financing, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Inventário p/ Market‑Making**

Domínio: Crypto  
Família / Subfamília: Credit & Financing /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Linha p/ MM com colateral cripto. Inventário p/ Market‑Making integra a família Credit & Financing, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Syndicated Loan c/ Colateral Cripto**

Domínio: Crypto  
Família / Subfamília: Credit & Financing /   
Persona: EPP  
Ticket padrão (R$): R$ 100.000,00  
Como funciona (XL): Pool de garantias digitais. Syndicated Loan c/ Colateral Cripto integra a família Credit & Financing, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp/Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.045000 | Você (a.m.): 0.033750 | Spread: 1.12 p.p. | Prazo ref.: 180d | Ticket padrão: R$ 100.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 180

Benchmarks & comparativos: Banco (a.m.): 4.50% a.m. | Você (a.m.): 3.38% a.m. | Juros banco (R$): R$ 30.226,01 | Custo com você (R$): R$ 22.037,45 | Economia (R$): R$ 8.188,56

## **Futuros BTC (CME)**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Hedge/exposição padronizado. Futuros BTC (CME) integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Inst./Wealth qualif.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Opções BTC (CME)**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Calls/puts semanais/mensais. Opções BTC (CME) integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Inst./Wealth qualif.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Futuros ETH (CME)**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Full/micro futures. Futuros ETH (CME) integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Opções ETH (CME)**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Opções sobre futuros ETH. Opções ETH (CME) integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Futuros SOL (CME)**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): SOL e micro‑SOL. Futuros SOL (CME) integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Futuros XRP (CME)**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): XRP e micro‑XRP. Futuros XRP (CME) integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **NDF BTC (OTC)**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cash‑settled em USD. NDF BTC (OTC) integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp/Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **TRS BTC**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Banco paga/recebe variação. TRS BTC integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **TRS ETH/Basket**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): TRS em ETH/cestas. TRS ETH/Basket integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Swap de Volatilidade**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Variance/vol swaps. Swap de Volatilidade integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **IRS Staking Yield (ETH)**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Troca yield staking vs fixo. IRS Staking Yield (ETH) integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Opções OTC Exóticas**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Barriers/asiáticas. Opções OTC Exóticas integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Hedge Basis (BTIC)**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Trava da base BRR/ETHRR. Hedge Basis (BTIC) integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional/APs  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Swaps USD‑Stablecoin**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Troca USD vs stablecoin. Swaps USD‑Stablecoin integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp/Tesouraria  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Forwards On‑chain**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Liquidação em deposit token. Forwards On‑chain integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Opções Semanais (BTC/ETH)**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Séries p/ eventos macro. Opções Semanais (BTC/ETH) integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Inst./Wealth qualif.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Calendar/Diagonal Spreads**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Estratégias com opções. Calendar/Diagonal Spreads integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Protective Puts**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Seguro da carteira. Protective Puts integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Covered Calls**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Renda sobre posição longa. Covered Calls integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Quanto Swaps (BTC‑USD/BRL)**

Domínio: Crypto  
Família / Subfamília: Derivatives & Hedging /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Swap com moeda distinta. Quanto Swaps (BTC‑USD/BRL) integra a família Derivatives & Hedging, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Capital Protegido BTC (Bond+Call)**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Tít. de renda fixa \+ call BTC. Capital Protegido BTC (Bond+Call) integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Capital Protegido ETH**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Estrutura similar com ETH. Capital Protegido ETH integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Autocallable BTC (Phoenix)**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cupons \+ autocalle. Autocallable BTC (Phoenix) integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth qualif.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Autocallable ETH**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cupons \+ autocalle. Autocallable ETH integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth qualif.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Barrier Reverse Convertible BTC**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 200.000,00  
Como funciona (XL): Cupom alto com risco de conversão. Barrier Reverse Convertible BTC integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth qualif.  
Taxas típicas (padronizada): Banco (a.m.): 0.025000 | Você (a.m.): 0.016250 | Spread: 0.88 p.p. | Prazo ref.: 45d | Ticket padrão: R$ 200.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 45

Benchmarks & comparativos: Banco (a.m.): 2.50% a.m. | Você (a.m.): 1.62% a.m. | Juros banco (R$): R$ 7.546,68 | Custo com você (R$): R$ 4.894,75 | Economia (R$): R$ 2.651,93

## **Dual Currency BTC/USDC**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cupom; liquidação em BTC/USDC. Dual Currency BTC/USDC integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Dual Currency ETH/USDC**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cupom; liquidação em ETH/USDC. Dual Currency ETH/USDC integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Range Accrual BTC**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cupom se preço em faixa. Range Accrual BTC integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Twin‑Win BTC**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Ganha em alta/baixa na faixa. Twin‑Win BTC integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **COE Multi‑Ativos (BTC+ETH+Ouro)**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cesta com barreiras. COE Multi‑Ativos (BTC+ETH+Ouro) integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Structured Note Tokenizada (ETH)**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Emissão on‑chain em lotes menores. Structured Note Tokenizada (ETH) integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **CLN Miners/Exchanges**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Credit‑linked note setor cripto. CLN Miners/Exchanges integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Proteção Parcial (95%)**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Floor parcial \+ upside limitado. Proteção Parcial (95%) integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Indexadas à Vol (BTC)**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Retorno ligado à vol implícita. Indexadas à Vol (BTC) integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Basket c/ Rebalance**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cesta BTC/ETH com rebalance. Basket c/ Rebalance integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Cupom de Staking (ETH)**

Domínio: Crypto  
Família / Subfamília: Structured Notes & COEs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cupom atrelado ao yield. Cupom de Staking (ETH) integra a família Structured Notes & COEs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Conta PJ em Stablecoin**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Operações USDC/USDT 24/7. Conta PJ em Stablecoin integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp/PME  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Cross‑border em Stablecoin**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Envio/recebimento global. Cross‑border em Stablecoin integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp/Marketplace  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Cash Sweep p/ Stablecoin**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Sobra diária em USDC/T‑bills. Cash Sweep p/ Stablecoin integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Tesouraria  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Deposit Tokens (JPMD/Citi)**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Liquidação com token bancário. Deposit Tokens (JPMD/Citi) integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Escrow Supply Chain**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Pagamento condicionado. Escrow Supply Chain integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Folha/Provisões em Stablecoin**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Pagamentos globais. Folha/Provisões em Stablecoin integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp/Creators  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Settlement Merchant em Stablecoin**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Liquidação adquirente em USDC. Settlement Merchant em Stablecoin integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: E‑commerce/global  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **FX on‑chain (USD–BRL)**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Conversão com DVP on‑chain. FX on‑chain (USD–BRL) integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Open Finance \+ Cripto**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Conciliação multi‑contas/carteiras. Open Finance \+ Cripto integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: PME/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **NF/Comprovantes on‑chain**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Selagem/auditoria. NF/Comprovantes on‑chain integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Citi Token Services (Cash)**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cash mgmt 24/7 programável. Citi Token Services (Cash) integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Multinacionais  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Stablecoin Bancária (EURCV/USDCV)**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Token de dinheiro eletrônico (MiCA). Stablecoin Bancária (EURCV/USDCV) integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Inst./Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Pagamentos com Deposit Token \+ FX**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Pagamento \+ câmbio. Pagamentos com Deposit Token \+ FX integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Treasury Dashboard On‑chain**

Domínio: Crypto  
Família / Subfamília: Treasury & Payments /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Saldos tokenizados \+ fiat. Treasury Dashboard On‑chain integra a família Treasury & Payments, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Tesourarias  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Prime Brokerage Cripto**

Domínio: Crypto  
Família / Subfamília: Prime & Institutional Services /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Execução \+ custódia \+ funding. Prime Brokerage Cripto integra a família Prime & Institutional Services, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Funds/MM  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Liquidez Multi‑Venue**

Domínio: Crypto  
Família / Subfamília: Prime & Institutional Services /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): SOR/RFQ multi‑venues. Liquidez Multi‑Venue integra a família Prime & Institutional Services, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Tri‑party Collateral Mgmt**

Domínio: Crypto  
Família / Subfamília: Prime & Institutional Services /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Agente de colateral on‑chain. Tri‑party Collateral Mgmt integra a família Prime & Institutional Services, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Risco & Travel Rule**

Domínio: Crypto  
Família / Subfamília: Prime & Institutional Services /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Screening e Travel Rule. Risco & Travel Rule integra a família Prime & Institutional Services, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Bancos/PSPs  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Settlement DVP on‑chain**

Domínio: Crypto  
Família / Subfamília: Prime & Institutional Services /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Entrega vs pagamento. Settlement DVP on‑chain integra a família Prime & Institutional Services, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Controle de Rehipoteca**

Domínio: Crypto  
Família / Subfamília: Prime & Institutional Services /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Mandatos de rehypothecation. Controle de Rehipoteca integra a família Prime & Institutional Services, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Proof‑of‑Reserves (PoR)**

Domínio: Crypto  
Família / Subfamília: Prime & Institutional Services /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Atestação de reservas. Proof‑of‑Reserves (PoR) integra a família Prime & Institutional Services, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Emissores/Plataformas  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Lend/Borrow de Ativos**

Domínio: Crypto  
Família / Subfamília: Prime & Institutional Services /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Empréstimo de BTC/ETH/stables. Lend/Borrow de Ativos integra a família Prime & Institutional Services, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Institucional  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Distribuição de T‑Bills Tokenizados**

Domínio: Crypto  
Família / Subfamília: Tokenization & RWAs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Acesso a tokens de T‑bills/MMFs. Distribuição de T‑Bills Tokenizados integra a família Tokenization & RWAs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Securitização de Recebíveis**

Domínio: Crypto  
Família / Subfamília: Tokenization & RWAs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): FIDC/ABS on‑chain. Securitização de Recebíveis integra a família Tokenization & RWAs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp/PME  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Tokenização de Dívida Corp.**

Domínio: Crypto  
Família / Subfamília: Tokenization & RWAs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Debêntures/notes on‑chain. Tokenização de Dívida Corp. integra a família Tokenization & RWAs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Corp/Wealth  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Equity Privado Tokenizado**

Domínio: Crypto  
Família / Subfamília: Tokenization & RWAs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Quotas/ações privadas. Equity Privado Tokenizado integra a família Tokenization & RWAs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: VC/FO  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Fundos Tokenizados**

Domínio: Crypto  
Família / Subfamília: Tokenization & RWAs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Cotas tokenizadas. Fundos Tokenizados integra a família Tokenization & RWAs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Imobiliário Tokenizado**

Domínio: Crypto  
Família / Subfamília: Tokenization & RWAs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): SPVs fracionados. Imobiliário Tokenizado integra a família Tokenization & RWAs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Qualif.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Notas Estruturadas Tokenizadas**

Domínio: Crypto  
Família / Subfamília: Tokenization & RWAs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Emissão on‑chain do banco. Notas Estruturadas Tokenizadas integra a família Tokenization & RWAs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Wealth/Inst.  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

## **Programa de Stablecoin Bancária**

Domínio: Crypto  
Família / Subfamília: Tokenization & RWAs /   
Persona: EPP  
Ticket padrão (R$): R$ 160.000,00  
Como funciona (XL): Token de dinheiro eletrônico. Programa de Stablecoin Bancária integra a família Tokenization & RWAs, subfamília nan. Mecânica: estrutura do produto, atores e fluxos financeiros do início à liquidação. Condições usuais: elegibilidade, garantias quando aplicável, canais de contratação e prazos. Riscos: crédito, mercado, liquidez e operacional, com práticas de mitigação e suitability. Custos e taxas: visão referencial; confira Benchmarks & comparativos.  
Público-alvo: Inst./Corp  
Taxas típicas (padronizada): Banco (a.m.): 0.035000 | Você (a.m.): 0.024500 | Spread: 1.05 p.p. | Prazo ref.: 90d | Ticket padrão: R$ 160.000,00  
Volume de mercado (snapshot): —  
Prazo (dias): 90

Benchmarks & comparativos: Banco (a.m.): 3.50% a.m. | Você (a.m.): 2.45% a.m. | Juros banco (R$): R$ 17.394,86 | Custo com você (R$): R$ 12.050,47 | Economia (R$): R$ 5.344,39

# **Patch não-destrutivo (v5.8p) — Relatório & Especificações**

Escopo: manter 100% do conteúdo do catálogo v5.8 e acrescentar melhorias operacionais sem alterar o layout/texto original. Este patch adiciona colunas auxiliares e marcações opcionais para BI, pricing e qualidade.

## **Achados (deep-dive)**

* Duplicatas por nome entre famílias (exemplos: CDB Pós‑CDI, CDB Prefixado, CDB Escalonado, LCI, LCA, LC).  
* Entradas com Subfamília em branco, com destaque para o domínio Crypto.  
* Linhas de serviços/pagamentos/cartões/digital com métricas de a.m. (juros) onde o adequado é fees/MDR/settlement/SLA.

  ***a.m.***

## **Deduplicação “soft” (com alias, sem excluir)**

Marcar 1 ocorrência como canônica e as demais como alias (campos auxiliares alias\_of, alias\_status), preservando texto original.

***alias\_of***

***alias\_status***

***Produto; Canônico (onde manter); Alias (onde manter)***  
***CDB Pós‑CDI; Investments → Fixed Income → Bank Bonds; Accounts & Deposits → Depósitos a prazo***  
***CDB Prefixado; Investments → Fixed Income → Bank Bonds; Accounts & Deposits → Depósitos a prazo***  
***CDB Escalonado; Investments → Fixed Income → Bank Bonds; Accounts & Deposits → Depósitos a prazo***  
***LCI; Investments → Fixed Income; Accounts & Deposits***  
***LCA; Investments → Fixed Income; Accounts & Deposits***  
***LC (Letra de Câmbio); Investments → Finance Companies; Accounts & Deposits***

## **Subfamília — Heurística (Crypto)**

Completar apenas a Subfamília derivando do nome do produto quando ausente. Exemplos sugeridos: Fria Segregada, MPC, Staking, Insured, Off‑exchange, Stablecoins, Deposit Tokens, Tokenized Treasuries, Escrow.

***Fria Segregada***

***MPC***

***Staking***

***Insured***

***Off‑exchange***

***Stablecoins***

***Deposit Tokens***

***Tokenized Treasuries***

***Escrow***

## **Mapeamento para colunas auxiliares (overlay)**

***Finalidade; Colunas auxiliares (não substituem as originais)***  
***Serviços / Pagamentos / Digital; aux\_fee\_fixed\_bank,aux\_fee\_rate\_bank,aux\_fee\_fixed\_offer,aux\_fee\_rate\_offer,aux\_mdr\_credit,aux\_mdr\_debit,aux\_settlement\_days,aux\_sla***  
***Loans / CreditLoan; aux\_rate\_bank\_am,aux\_rate\_offer\_am,aux\_tenor\_days,aux\_cet\_am***  
***Investments; aux\_expected\_yield,aux\_indexer,aux\_duration\_days,aux\_tax\_treatment***  
***Insurance; aux\_premium\_monthly,aux\_premium\_annual,aux\_coverage\_sum,aux\_deductible***  
***FX & Hedging; aux\_spread\_fx,aux\_points,aux\_tenor\_days,aux\_notional***  
***Aliases; alias\_of,alias\_status(=deprecatedou vazio)***

***aux\_fee\_fixed\_bank***

***aux\_fee\_rate\_bank***

***aux\_fee\_fixed\_offer***

***aux\_fee\_rate\_offer***

***aux\_mdr\_credit***

***aux\_mdr\_debit***

***aux\_settlement\_days***

***aux\_sla***

***aux\_rate\_bank\_am***

***aux\_rate\_offer\_am***

***aux\_tenor\_days***

***aux\_cet\_am***

***aux\_expected\_yield***

***aux\_indexer***

***aux\_duration\_days***

***aux\_tax\_treatment***

***aux\_premium\_monthly***

***aux\_premium\_annual***

***aux\_coverage\_sum***

***aux\_deductible***

***aux\_spread\_fx***

***aux\_points***

***aux\_tenor\_days***

***aux\_notional***

***alias\_of***

***alias\_status***

***deprecated***

## **Especificações (YAML)**

***version: 5.8p***  
***overlay\_columns:***  
  ***common:***  
    ***\- alias\_of***  
    ***\- alias\_status   \# deprecated | ''***  
    ***\- aux\_pricing\_model\_hint  \# Fees|CreditLoan|Investment|Insurance|Hedging|Fees/Spread***  
  ***services\_and\_payments:***  
    ***\- aux\_fee\_fixed\_bank***  
    ***\- aux\_fee\_rate\_bank***  
    ***\- aux\_fee\_fixed\_offer***  
    ***\- aux\_fee\_rate\_offer***  
    ***\- aux\_mdr\_credit***  
    ***\- aux\_mdr\_debit***  
    ***\- aux\_settlement\_days***  
    ***\- aux\_sla***  
  ***loans\_credit:***  
    ***\- aux\_rate\_bank\_am***  
    ***\- aux\_rate\_offer\_am***  
    ***\- aux\_tenor\_days***  
    ***\- aux\_cet\_am***  
  ***investments:***  
    ***\- aux\_expected\_yield***  
    ***\- aux\_indexer***  
    ***\- aux\_duration\_days***  
    ***\- aux\_tax\_treatment***  
  ***insurance:***  
    ***\- aux\_premium\_monthly***  
    ***\- aux\_premium\_annual***  
    ***\- aux\_coverage\_sum***  
    ***\- aux\_deductible***  
  ***fx\_hedging:***  
    ***\- aux\_spread\_fx***  
    ***\- aux\_points***  
    ***\- aux\_tenor\_days***  
    ***\- aux\_notional***

***version: 5.8p***  
***overlay\_columns:***  
  ***common:***  
    ***\- alias\_of***  
    ***\- alias\_status   \# deprecated | ''***  
    ***\- aux\_pricing\_model\_hint  \# Fees|CreditLoan|Investment|Insurance|Hedging|Fees/Spread***  
  ***services\_and\_payments:***  
    ***\- aux\_fee\_fixed\_bank***  
    ***\- aux\_fee\_rate\_bank***  
    ***\- aux\_fee\_fixed\_offer***  
    ***\- aux\_fee\_rate\_offer***  
    ***\- aux\_mdr\_credit***  
    ***\- aux\_mdr\_debit***  
    ***\- aux\_settlement\_days***  
    ***\- aux\_sla***  
  ***loans\_credit:***  
    ***\- aux\_rate\_bank\_am***  
    ***\- aux\_rate\_offer\_am***  
    ***\- aux\_tenor\_days***  
    ***\- aux\_cet\_am***  
  ***investments:***  
    ***\- aux\_expected\_yield***  
    ***\- aux\_indexer***  
    ***\- aux\_duration\_days***  
    ***\- aux\_tax\_treatment***  
  ***insurance:***  
    ***\- aux\_premium\_monthly***  
    ***\- aux\_premium\_annual***  
    ***\- aux\_coverage\_sum***  
    ***\- aux\_deductible***  
  ***fx\_hedging:***  
    ***\- aux\_spread\_fx***  
    ***\- aux\_points***  
    ***\- aux\_tenor\_days***  
    ***\- aux\_notional***

## **SQL (DDL de referência)**

***\-- Tabela overlay (opcional para BI)***  
***create table if not exists catalogo\_v58\_overlay (***  
  ***id text primary key,***  
  ***alias\_of text,***  
  ***alias\_status text check (alias\_status in ('deprecated', '')),***  
  ***aux\_pricing\_model\_hint text,***  
  ***aux\_fee\_fixed\_bank numeric(18,2),***  
  ***aux\_fee\_rate\_bank numeric(6,5),***  
  ***aux\_fee\_fixed\_offer numeric(18,2),***  
  ***aux\_fee\_rate\_offer numeric(6,5),***  
  ***aux\_mdr\_credit numeric(6,5),***  
  ***aux\_mdr\_debit numeric(6,5),***  
  ***aux\_settlement\_days int,***  
  ***aux\_sla text,***  
  ***aux\_rate\_bank\_am numeric(6,5),***  
  ***aux\_rate\_offer\_am numeric(6,5),***  
  ***aux\_tenor\_days int,***  
  ***aux\_cet\_am numeric(6,5),***  
  ***aux\_expected\_yield text,***  
  ***aux\_indexer text,***  
  ***aux\_duration\_days int,***  
  ***aux\_tax\_treatment text,***  
  ***aux\_premium\_monthly numeric(18,2),***  
  ***aux\_premium\_annual numeric(18,2),***  
  ***aux\_coverage\_sum numeric(18,2),***  
  ***aux\_deductible numeric(18,2),***  
  ***aux\_spread\_fx numeric(6,5),***  
  ***aux\_points numeric(10,4),***  
  ***aux\_notional numeric(18,2)***  
***);***

***\-- Tabela overlay (opcional para BI)***  
***create table if not exists catalogo\_v58\_overlay (***  
  ***id text primary key,***  
  ***alias\_of text,***  
  ***alias\_status text check (alias\_status in ('deprecated', '')),***  
  ***aux\_pricing\_model\_hint text,***  
  ***aux\_fee\_fixed\_bank numeric(18,2),***  
  ***aux\_fee\_rate\_bank numeric(6,5),***  
  ***aux\_fee\_fixed\_offer numeric(18,2),***  
  ***aux\_fee\_rate\_offer numeric(6,5),***  
  ***aux\_mdr\_credit numeric(6,5),***  
  ***aux\_mdr\_debit numeric(6,5),***  
  ***aux\_settlement\_days int,***  
  ***aux\_sla text,***  
  ***aux\_rate\_bank\_am numeric(6,5),***  
  ***aux\_rate\_offer\_am numeric(6,5),***  
  ***aux\_tenor\_days int,***  
  ***aux\_cet\_am numeric(6,5),***  
  ***aux\_expected\_yield text,***  
  ***aux\_indexer text,***  
  ***aux\_duration\_days int,***  
  ***aux\_tax\_treatment text,***  
  ***aux\_premium\_monthly numeric(18,2),***  
  ***aux\_premium\_annual numeric(18,2),***  
  ***aux\_coverage\_sum numeric(18,2),***  
  ***aux\_deductible numeric(18,2),***  
  ***aux\_spread\_fx numeric(6,5),***  
  ***aux\_points numeric(10,4),***  
  ***aux\_notional numeric(18,2)***  
***);***

Gerado automaticamente.

**Apêndice – Fontes e Notas de Metodologia**

**• Consignado PF (≈ R$ 683 bi, jun/2025):** \- CLT: saldo atingiu R$ 46,437 bi em jun/2025, segundo fala do BC e imprensa. Fontes: IstoÉ Dinheiro/Estadão Conteúdo (28/07/2025). INSS e Servidores: usados saldos de dez/2024 reportados por Agência Brasil (INSS ≈ R$ 270,8 bi; Servidores ≈ R$ 365,4 bi). BC revisou séries em jun/2025.

**• Conta Garantida PJ (≈ R$ 1,6 tri, proxy):** Não há divulgação pública consolidada mensal por modalidade facilmente acessível; usamos como proxy o crédito livre PJ total (R$ 1,6 tri em jun/2025, BC). Para séries por modalidade (PJ – Conta Garantida), ver portal de dados abertos/SGS.

**• Capital de Giro PJ:** Série específica existe no SGS (código 20550 – saldo de capital de giro total – PJ). Por instabilidade no acesso automático, mantivemos nota metodológica e sugerimos usar a série como referência pontual quando necessário.

**• CRIs (≈ R$ 207 bi, jun/2024):** Estoque informado pela B3 (jun/2024). Últimos dados consolidados públicos encontrados até o fechamento deste documento.

**• CRAs (≈ R$ 160 bi, jun/2025):** Estoque publicado pela B3 (Bora Investir, 10/07/2025).

**• FIDCs (≈ R$ 690 bi, abr/2025):** Patrimônio líquido agregado da classe, segundo Uqbar (mai/2025), em linha com dados da ANBIMA; reportagens de jul/2025 citam ≈ R$ 687,4 bi em jun/2025.