# Studium

Studium is a pre-institutional pilot initiative for place-based apprenticeship, documentation and cultural preservation in Northern Portugal.

**Pilot · Fieldwork · Governance**

## Operational state

Studium is not yet a legally constituted institution, field program or partner network. The repository currently defines the governance, consent, archive and pilot-readiness systems required before field activity, public recruitment or product implementation.

## Canonical reading hierarchy

Read these files in order when evaluating the current operating model:

1. [`docs/00-overview.md`](docs/00-overview.md) — project map and status labels
2. [`docs/20-public-language-and-positioning-guide.md`](docs/20-public-language-and-positioning-guide.md) — public copy boundaries
3. [`docs/11-governance-blueprint.md`](docs/11-governance-blueprint.md) — legal path, advisory board and decision rights
4. [`docs/12-stewardship-operating-model.md`](docs/12-stewardship-operating-model.md) — steward authority, review cycles and escalation
5. [`docs/13-consent-and-documentation-ethics.md`](docs/13-consent-and-documentation-ethics.md) — consent workflow and documentation ethics
6. [`docs/19-technology-and-data-architecture.md`](docs/19-technology-and-data-architecture.md) — archive, metadata and technology gate
7. [`docs/16-operational-pilot-plan.md`](docs/16-operational-pilot-plan.md) — 24-month Northern Portugal pilot sequence
8. [`docs/17-risk-and-failure-analysis.md`](docs/17-risk-and-failure-analysis.md) — risk register and stop / pivot / continue criteria

## Repository

| Path | Description |
|------|-------------|
| **Live site** | https://brauliosotomayor.github.io/studium/ |
| [`docs/index.html`](docs/index.html) | Public pilot page |
| [`docs/00-overview.md`](docs/00-overview.md) | Canonical repository map |
| [`docs/ORCHESTRATOR.md`](docs/ORCHESTRATOR.md) | Phase IV agent handoff and work lanes |
| [`data/`](data/) | Operational CSV schemas and internal research data |
| [`src/chat.md`](src/chat.md) | Original conversation export, preserved as archive |

## Archival and exploratory materials

Older strategy and atlas-planning docs remain in the repository for context, but they are not the current operating authority. Use `docs/00-overview.md` for status and visibility labels before citing them.

## Publishing the site (branch deploy — not Actions)

Static site files live in `docs/`. **Do not use GitHub Actions** for Pages; deploy from the branch only.

1. **GitHub → Settings → Pages**
2. **Build and deployment:** Source = **Deploy from a branch** (not “GitHub Actions”)
3. **Branch:** `main` · **Folder:** `/docs`
4. On the free plan, the repo must be **public** for Pages to work.

`docs/.nojekyll` disables Jekyll so `index.html` is served as-is.

**URL after deploy:** https://brauliosotomayor.github.io/studium/  
(Open `docs/index.html` locally anytime for a preview.)

## For agents and orchestrators

Read [`docs/ORCHESTRATOR.md`](docs/ORCHESTRATOR.md) for current repo state, priorities and suggested next tasks.

## License

TBD
