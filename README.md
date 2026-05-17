# Studium

An early-stage pilot for place-based apprenticeship, documentation, and cultural preservation in Northern Portugal.

**Student · Master · Steward**

## Repository

| Path | Description |
|------|-------------|
| [`docs/index.html`](docs/index.html) | Front page (pilot status, stewardship, documentation method) |
| **Live site** | https://brauliosotomayor.github.io/studium/ |
| [`docs/00-overview.md`](docs/00-overview.md) | Start here — project summary and doc index |
| [`data/studium_atlas_master.csv`](data/studium_atlas_master.csv) | Normalized atlas (266 nodes) |
| [`docs/05-corridor-registry.md`](docs/05-corridor-registry.md) | Phase II — corridor registry |
| [`docs/01-marketplace-and-business.md`](docs/01-marketplace-and-business.md) | Business model and launch strategy |
| [`docs/02-triangle-philosophy.md`](docs/02-triangle-philosophy.md) | Philosophical architecture |
| [`docs/03-manifesto.md`](docs/03-manifesto.md) | Brand manifesto |
| [`docs/04-pilot-plan.md`](docs/04-pilot-plan.md) | First-year pilot (Northern Portugal) |
| [`docs/ORCHESTRATOR.md`](docs/ORCHESTRATOR.md) | Remote orchestrator handoff |
| [`src/chat.md`](src/chat.md) | Original conversation export |
| [`data/`](data/) | Source dataset (masters atlas, drafts, visuals) |

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

Read [`docs/ORCHESTRATOR.md`](docs/ORCHESTRATOR.md) for current repo state, priorities, and suggested next tasks.

## License

TBD
