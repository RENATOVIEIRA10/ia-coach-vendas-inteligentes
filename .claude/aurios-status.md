# AUR.IOS Engineering Governance — ia-coach-vendas-inteligentes

> Leia este arquivo no inicio de toda sessao neste repo.
> Atualizar ao fechar cada ciclo.

---

## Identidade do repo

- **Produto:** IA Coach de Vendas — agente consultivo com empatia e estrategia para times comerciais
- **Status:** PRE-DEV — esqueleto inicial (README + app-config.json apenas)
- **Stack:** A definir (3 commits, sem package.json, sem arquitetura implementada)
- **Supabase:** A definir
- **Deploy:** A definir
- **Branch principal:** main
- **Mapeado em:** 2026-05-07

---

## Registro de Ciclos

| # | Titulo | Status | Commits | Data |
|---|--------|--------|---------|------|
| 001 | Product brief + arquitetura + setup inicial | PENDENTE | — | — |
| 002 | MVP conversacional — primeiro fluxo end-to-end | PENDENTE | — | — |

---

## Ciclo fechado mais recente

Nenhum ciclo fechado ainda. Repo em estado pre-dev.

---

## Ciclo atual

- **Ciclo:** 001
- **Status:** PENDENTE
- **Titulo:** Product brief + arquitetura + setup inicial
- **Severidade:** MEDIA (produto nao tem usuarios ainda)

**Problema 1 — Sem arquitetura definida:**
Repo tem apenas README.md e app-config.json. Nao ha package.json, nenhuma stack escolhida, sem schema de banco, sem definicao de canais (WhatsApp? Web? API?). Impossivel comecar a implementar sem decisoes de produto e tecnicas documentadas.

**Problema 2 — Escopo ambiguo:**
"Vendas consultivas com empatia e estrategia" e o conceito, mas o produto nao define: quem e o usuario (vendedor? gerente? empresa?), qual e o fluxo principal (roteiro de pitch? analise de leads? simulacao de objecoes?), nem qual dado de contexto o agente precisa.

**Escopo minimo:**
1. `/product-brief` — 20-40 min de discovery com CEO: problema, usuario, jornada, metrica de sucesso
2. Escolha de stack (Node.js + WhatsApp? Next.js + web? API headless?)
3. Setup inicial: `npm init`, `.gitignore`, `.env.example`, estrutura de pastas
4. Ciclo 001 so fecha com `/tech-spec` aprovado e repo buildavel

**Arquivo central:**
- `README.md` (unico arquivo existente alem de app-config.json)

**Gatilho Codex:** NAO — ainda sem codigo sensivel

**Agente inicial recomendado:** `/product-brief` → `/tech-spec` → `aurios-implementation-agent`

---

## Proxima task recomendada

**Ciclo 001** — Product brief

Nao faz sentido implementar sem saber o que construir. O `/product-brief` responde as perguntas fundamentais em 20-40 minutos e evita retrabalho. Com brief aprovado, a escolha de stack e o setup inicial saem em menos de 1 hora.

---

## Backlog priorizado

| Ciclo | Titulo | Severidade | Esforco | Por que agora |
|-------|--------|------------|---------|---------------|
| 001 | Product brief + stack decision + setup inicial | MEDIA | 2-4h | Sem brief, qualquer implementacao e especulacao |
| 002 | MVP conversacional — fluxo principal end-to-end | ALTA | sessao dedicada | Primeiro teste real com usuario define toda arquitetura downstream |
| 003 | Integracao com canal de distribuicao (WhatsApp/Web) | ALTA | sessao dedicada | Nenhum canal = produto invisivel |

---

## Riscos abertos

| Risco | Severidade | Arquivo | Ciclo alvo |
|-------|------------|---------|------------|
| Escopo indefinido — produto pode ser construido na direcao errada | ALTA | — | 001 |
| Stack indefinida — decisao tardia gera retrabalho | ALTA | — | 001 |
| Zero testes (produto ainda nao existe) | MEDIA | — | 002 |

---

## Ritual obrigatorio — integracoes sensiveis

Quando houver codigo implementado que toque WhatsApp, LLM, Supabase, auth, billing ou dados de leads:

```
1. Implementacao minima
2. Testes de borda na funcao central
3. aurios-security-reviewer
4. codex:adversarial-review --background
5. Fechar todos os FLAGs relevantes
6. Verificar enforcement em todos os callers
7. Atualizar este arquivo
```

---

## Notas de inicializacao

- **Inicializado por:** aurios-repo-cartographer + Claude Sonnet 4.6
- **Data:** 2026-05-07
- **Branch:** main
- **Observacoes:** Repo pre-dev. 3 commits. Sem stack implementada. Primeiro passo obrigatorio: product brief antes de qualquer codigo.
