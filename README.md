# CreditForge — Marketplace P2P de Crédito com Leilão Reverso (Uniform-Price)

[![Release](https://img.shields.io/github/v/release/gustavomhss/CreditForge?include_prereleases)](https://github.com/gustavomhss/CreditForge/releases)
[![Downloads](https://img.shields.io/github/downloads/gustavomhss/CreditForge/total)](https://github.com/gustavomhss/CreditForge/releases)
[![License: Proprietary](https://img.shields.io/badge/License-Proprietary-red.svg)](LICENSE)
![Status](https://img.shields.io/badge/status-active-success)

> **O que é**: Marketplace P2P onde tomadores abrem leilões de crédito e investidores competem com ofertas; o clearing é **preço único (uniform-price)**.
> **Por que importa**: releases versionados (tags) criam um **ponto canônico** para clonar, testar e auditar a mesma base de código.

---

## 📦 Release atual (canônico)
- **Tag estável:** `vA3.1.11`
- **Página do release:** https://github.com/gustavomhss/CreditForge/releases/tag/vA3.1.11
- **ZIP do tag:** https://github.com/gustavomhss/CreditForge/archive/refs/tags/vA3.1.11.zip

> Sempre compartilhe a **página do release**: notas, assets e link estável para download.

---

## 🧭 Sumário
- [Visão Geral](#-visão-geral)
- [Arquitetura](#-arquitetura)
- [Funcionalidades](#-funcionalidades)
- [Fluxos Principais](#-fluxos-principais)
- [Quickstart](#-quickstart)
- [Requisitos](#-requisitos)
- [Instalação & Configuração](#-instalação--configuração)
- [Execução (Dev/Prod)](#-execução-devprod)
- [Scripts](#-scripts)
- [Qualidade (Lint/Test/Format)](#-qualidade-linttestformat)
- [Testes (Unit/Integration/E2E)](#-testes-unitintegratione2e)
- [API (exemplos)](#-api-exemplos)
- [Modelos de Dados](#-modelos-de-dados)
- [Observabilidade (Logs/Metrics/Tracing)](#-observabilidade-logsmetricstracing)
- [Segurança & Compliance](#-segurança--compliance)
- [Versionamento & Releases](#-versionamento--releases)
- [Estrutura do Repositório](#-estrutura-do-repositório)
- [Contribuindo](#-contribuindo)
- [Roadmap](#-roadmap)
- [FAQ](#-faq)
- [Troubleshooting](#-troubleshooting)
- [Links úteis](#-links-úteis)
- [Créditos & Licença](#-créditos--licença)

---

## 🔎 Visão Geral
O **CreditForge** permite que **Tomadores** criem leilões (Auction) definindo valor, prazo e garantias. **Investidores** propõem **ofertas** (Offer) com juros e condições. O leilão liquida em **preço único**, priorizando melhor taxa até preencher o montante.

**Pilares**
- Leilão reverso (uniform-price) com regras anti-manipulação.
- LoanVault: registro de empréstimos e pagamentos.
- Releases canônicos: cada entrega marcada por tag + página de release.

---

## 🧱 Arquitetura
~~~text
┌───────────────┐      HTTP/WS      ┌──────────────────┐
│   Web Client  │ ◀──────────────── ▶│    API (NestJS)  │
└───────────────┘                    ├──────────────────┤
                                      │  Auction/Offer  │
                                      │    LoanVault    │
                                      │    Auth (JWT)   │
                                      └─────────┬────────┘
                                                │
                                     ┌──────────┴──────────┐
                                     │  PostgreSQL   Redis │
                                     └─────────────────────┘
~~~
> Stack oficial: **Next.js 14 (TS)** · **NestJS 10** · **PostgreSQL 15 (Prisma)** · **Redis 7 (BullMQ)** · **Docker Compose**.

---

## 🧩 Funcionalidades
- Criar/editar/cancelar **leilão** (Auction).
- Registrar **ofertas** (Offer) e calcular **clearing price**.
- Emissão de eventos (`AuctionCreated`, `OfferPlaced`, …).
- Painel do investidor (carteira e histórico).
- Export de relatórios (CSV/JSON).

---

## 🔁 Fluxos Principais
1) **Tomador** cria leilão → define `valor`, `prazo`, `colateral`.
2) **Investidores** ofertam → `taxa_bps`, `quantia`.
3) Ao fechar: ordena por taxa, preenche alvo → **preço único**.
4) Contrato no LoanVault + cronograma de pagamentos.

---

## 🚀 Quickstart
~~~bash
git clone https://github.com/gustavomhss/CreditForge.git
cd CreditForge
git checkout tags/vA3.1.11
npm i && npm run dev
~~~

---

## 🔧 Requisitos
- Node LTS (18+), Git  
- (Opcional) Docker 24+

---

## 🛠️ Instalação & Configuração
### Opção A — Node local
~~~bash
npm i
cp .env.example .env
~~~

### Opção B — Docker (serviços locais)
~~~bash
docker compose up -d postgres redis
# docker compose ps              # status
# docker compose logs -f postgres # logs do DB
~~~

### Variáveis de ambiente (exemplo)
| Variável       | Exemplo                                                                  | Descrição                 |
|----------------|--------------------------------------------------------------------------|---------------------------|
| `PORT`         | `3000`                                                                   | Porta HTTP                |
| `DATABASE_URL` | `postgres://postgres:postgres@localhost:5432/creditengine?schema=public` | Conexão Postgres (Prisma) |
| `REDIS_URL`    | `redis://localhost:6379`                                                 | Cache/Fila (BullMQ)       |
| `LOG_LEVEL`    | `info`                                                                   | `debug` \| `info` \| `warn` \| `error` |

> **Segredos**: não comite `.env` (adicione ao `.gitignore`).

---

## ▶️ Execução (Dev/Prod)
**Dev**
~~~bash
npm run dev
~~~

**Build & Prod**
~~~bash
npm run build && npm run start
~~~

**Docker (app completo)**
~~~bash
docker compose up --build
~~~

---

## 📜 Scripts
~~~bash
npm run dev        # hot reload
npm run build      # build
npm run start      # produção
npm run lint       # ESLint
npm run format     # Prettier
npm run test       # unit
npm run test:e2e   # end-to-end (exemplo)
~~~

---

## ✅ Qualidade (Lint/Test/Format)
- ESLint, Prettier, Type-check (`tsc --noEmit`).  
- Sugestão: Husky para `pre-commit` rodar `lint`/`test`.

---

## 🧪 Testes (Unit/Integration/E2E)
- **Unit**: funções puras (ordenar ofertas, clearing).  
- **Integration**: API + DB (criar leilão, ofertar, fechar).  
- **E2E**: fluxo usuário (abrir leilão → ofertar → liquidar).

Exemplo (pseudo):
~~~ts
it('ordena ofertas e calcula preço único', () => {
  const ofertas = [ {taxa_bps:900, q:500}, {taxa_bps:850, q:400} ];
  const { preco, aloc } = liquidar(ofertas, 800);
  expect(preco).toBe(900);
  expect(aloc.total).toBe(800);
});
~~~

---

## 🌐 API (exemplos)
**Criar leilão**
~~~http
POST /api/auction
Content-Type: application/json

{
  "valor": 100000,
  "prazo_dias": 180,
  "colateral": "recebiveis"
}
~~~

**Enviar oferta**
~~~http
POST /api/auction/{id}/offer
{
  "taxa_bps": 870,
  "quantia": 20000
}
~~~

**Fechar leilão**
~~~http
POST /api/auction/{id}/close
~~~
> Auth (Bearer) e validações conforme backend real.

---

## 🗃️ Modelos de Dados (simplificado)
~~~text
Auction(id, valor, prazo_dias, status)
Offer(id, auction_id, taxa_bps, quantia, status)
Loan(id, auction_id, principal, juros_bps, schedule_json)
~~~

---

## 👀 Observabilidade (Logs/Metrics/Tracing)
- Logs estruturados (JSON; nível via `LOG_LEVEL`).  
- Métricas: latência, erros, criação/fechamento de leilões.  
- Tracing: `trace_id` nos headers para correlação.

---

## 🔐 Segurança & Compliance
- Headers seguros (CSP, HSTS, X-Content-Type-Options).  
- `npm audit` / `pnpm audit` para dependências.  
- Contato: security@seu-dominio.com (divulgação responsável).

---

## 🏷️ Versionamento & Releases
- Tags `vA*` (ex.: `vA3.1.11`), **página do release** e **ZIP do tag**.  
- Fluxo típico:
~~~bash
git switch main && git pull
# commits/merge
git tag -a vA3.1.12 -m "Release vA3.1.12"
git push origin vA3.1.12
# criar release:
gh release create vA3.1.12 --generate-notes
~~~
**URLs canônicas**  
Página: `.../releases/tag/<TAG>` · ZIP: `.../archive/refs/tags/<TAG>.zip`

---

## 🗂️ Estrutura do Repositório
~~~text
.
├─ src/                      # código-fonte
├─ docs/                     # docs extras
├─ .github/                  # templates/workflows
│  ├─ ISSUE_TEMPLATE/
│  ├─ workflows/
│  └─ PULL_REQUEST_TEMPLATE.md
├─ README.md
└─ CHANGELOG.md
~~~

---

## 🤝 Contribuindo
1) Abra uma **issue** para discutir a mudança.  
2) Crie branch `feat/...` ou `fix/...`.  
3) Use **Conventional Commits** (`feat:`, `fix:`, `docs:`, ...).  
4) Abra PR com escopo claro e evidências (prints/logs).

---

## 🗺️ Roadmap (resumo)
- vA3.1.12: melhorias no fechamento do leilão.  
- vA3.1.13: dashboard de KPIs.  
- vA3.1.14: auditoria de eventos on-chain.

---

## ❓ FAQ
**Por que clonar pelo tag?** Garante que todos usem a **mesma versão**.  
**Por que a página do release é canônica?** Consolida notas/assets num link estável.  
**Posso usar Docker?** Sim — vide *Instalação & Configuração*.

---

## 🛠️ Troubleshooting
- **404** na página do release → repo privado ou release em draft.  
- **ZIP 404** → tag no commit errado; refaça tag e `push -f`.  
- **Deps quebradas** → remova `node_modules` e reinstale.

---

## 🔗 Links úteis
- Releases: https://github.com/gustavomhss/CreditForge/releases  
- ZIP (tag atual): https://github.com/gustavomhss/CreditForge/archive/refs/tags/vA3.1.11.zip  
- Changelog: `CHANGELOG.md`

---

## 👤 Créditos & Licença
Maintainer: **Gustavo Schneiter**  
Licença: **Proprietária — All Rights Reserved** (veja `LICENSE`).
