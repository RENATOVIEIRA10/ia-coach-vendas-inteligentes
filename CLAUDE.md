# CLAUDE.md

## Agent skills

Plugin `mattpocock-skills`, configurado por `setup-matt-pocock-skills` em 25/09/2026. O GSD continua sendo o fluxo; as skills do Matt complementam.

### Issue tracker

GSD em `.planning/` e documentacao versionada, sem Cockpit operacional. Sem GitHub Issues nem `.scratch/` como tracker neste repositorio. See `docs/agents/issue-tracker.md`.

### Triage labels

Os cinco papéis padrão (`needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix`), gravados como linha `Status:` no item GSD. See `docs/agents/triage-labels.md`.

### Domain docs

Single-context: `CONTEXT.md` + `docs/adr/` na raiz, criados sob demanda. See `docs/agents/domain.md`.

### Uso junto com o GSD

- Antes de `/gsd-plan-phase` de fase nova: rodar `mattpocock-skills:grill-me` (ou `grill-with-docs` quando houver `CONTEXT.md`/ADRs).
- Planejar em fatia vertical (tracer bullet) e definir antes o seam de teste.
- Não usar `to-spec`, `to-tickets` nem `implement`.
