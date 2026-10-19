# Issue tracker: GSD (`.planning/`)

O trabalho deste repo é rastreado pelo GSD em `.planning/` (`ROADMAP.md`, `STATE.md`, `phases/`, todos e backlog). Tarefas operacionais, decisões e evidências ficam no planejamento e na documentação versionada do projeto. O Cockpit foi descontinuado em 19/10/2026. Não há GitHub Issues nem `.scratch/` como tracker.

## Quando uma skill disser "publish to the issue tracker"

Não criar issue no GitHub nem arquivo em `.scratch/`. Entregar ao GSD:

- Spec, decisões fechadas ou saída de grilling → virar fase (`/gsd-add-phase`, `/gsd-insert-phase`) ou alimentar `/gsd-plan-phase` / `/gsd-discuss-phase`.
- Ideia para depois → `/gsd-add-backlog`.
- Tarefa pequena → `/gsd-add-todo`.

## Quando uma skill disser "fetch the relevant ticket"

Ler a fase referenciada em `.planning/phases/` (`*-CONTEXT.md`, `*-PLAN.md`, `*-SUMMARY.md`) ou o todo/backlog que o usuário apontar.

## Fluxo

GSD é o fluxo de planejar, executar, verificar e shipar. `to-spec`, `to-tickets`, `implement` e `wayfinder` não são usados neste repo: seriam um segundo fluxo concorrendo com `.planning/`.

## Pull requests as a triage surface

**PRs as a request surface: no.**
