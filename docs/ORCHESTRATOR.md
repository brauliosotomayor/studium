# Orchestrator Handoff — Studium

**Repo:** `brauliosotomayor/studium`  
**Branch:** `main`  
**Last updated:** 2026-05-17 (Phase IV consolidation pass)  
**Audience:** Remote orchestrator / agent coordinator assigning work to agents

---

## Current phase

Studium is in **Phase IV — Systems Consolidation and Pilot Readiness**.

The repository has moved from concept generation into an operational workspace. The immediate task is to make the workspace coherent: canonical documents must be clearly separated from exploratory, archival and superseded materials.

Do not generate new strategy until the consolidation layer is stable.

---

## Operating posture

Studium is a pre-institutional pilot initiative. It is not yet:

- a legally constituted institution;
- an active field program;
- a partner network;
- a public atlas;
- an app or marketplace;
- a student recruitment program.

Current public framing:

> An early-stage pilot for place-based apprenticeship, documentation and cultural preservation in Northern Portugal.

Use a research posture: speak from documented fieldwork, verified relationships and explicit governance records.

---

## Canonical operating spine

Read and maintain these files in order:

1. `README.md`
2. `docs/00-overview.md`
3. `docs/20-public-language-and-positioning-guide.md`
4. `docs/11-governance-blueprint.md`
5. `docs/12-stewardship-operating-model.md`
6. `docs/13-consent-and-documentation-ethics.md`
7. `docs/19-technology-and-data-architecture.md`
8. `docs/16-operational-pilot-plan.md`
9. `docs/17-risk-and-failure-analysis.md`

These files supersede older conceptual framing wherever there is conflict.

---

## Document authority classes

| Class | Files | Use |
|-------|-------|-----|
| Canonical public | `README.md`, `docs/index.html`, `docs/20-public-language-and-positioning-guide.md` | Public-facing language and repository entrypoints |
| Canonical operating | `docs/11`, `docs/12`, `docs/13`, `docs/16`, `docs/17`, `docs/19` | Governance, consent, archive, pilot and risk authority |
| Operational internal | `docs/06`, `docs/09`, `docs/14`, `docs/15`, `docs/18`, `data/*.csv` | Taxonomy, evaluation, funding, schemas and registers |
| Archival / exploratory | `docs/01`, `docs/02`, `docs/03`, `docs/04`, `docs/05`, `docs/07`, `docs/10`, `src/chat.md` | Historical context and planning references only |
| Superseded | `docs/08-stewardship-framework.md` | Historical ethics framework; authority moved to `docs/11`, `docs/12`, `docs/13` |

---

## Phase IV work lanes

### Lane A — Governance consolidation

Authoritative artifacts: `docs/11`, `docs/12`, `docs/13`

Maintain:

- founder authority limits;
- steward veto and pause authority;
- advisory board structure;
- decision-rights matrix;
- escalation and conflict systems.

### Lane B — Archive and data governance

Authoritative artifacts: `docs/19`, `data/studium_archive_schema.csv`, `data/studium_consent_schema.csv`

Maintain:

- metadata schema;
- archive access tiers;
- consent linkage model;
- restricted-material workflows;
- public/private node logic.

### Lane C — Public positioning

Authoritative artifacts: `docs/20`, `README.md`, `docs/index.html`

Maintain:

- pre-institutional pilot language;
- prohibition on active partnership or practitioner claims without evidence;
- separation of public copy from internal atlas planning.

### Lane D — Operational pilot readiness

Authoritative artifacts: `docs/16`, `docs/14`, `data/studium_operational_checklists.csv`

Maintain:

- Northern Portugal sequence;
- fieldwork cadence;
- compensation logic;
- student-readiness gate;
- evaluation criteria.

### Lane E — Institutional ecosystem

Authoritative artifacts: `docs/18`, `data/studium_partner_targets.csv`, `data/studium_advisor_candidates.csv`

Maintain:

- fiscal sponsorship review;
- Portuguese association path;
- advisor candidate categories;
- partner target categories;
- funding constraints.

### Lane F — Repository consolidation

Authoritative artifacts: `README.md`, `docs/00-overview.md`, `docs/ORCHESTRATOR.md`

Maintain:

- canonical reading order;
- status and visibility labels;
- superseded/archive markers;
- contributor navigation.

---

## Prohibited work until consolidation stabilizes

Do not:

- add atlas regions;
- add new symbolic or conceptual frameworks;
- build app, booking or marketplace flows;
- publish active practitioner, steward, advisor or partner claims;
- turn internal candidate data into public copy;
- use old business or atlas docs as current authority;
- expand beyond Northern Portugal public scope.

---

## Precision language rules

Replace vague institutional language with implementation-state language:

- `real` -> documented, verified, field-validated or operational;
- `actual` -> documented, verified or existing;
- `legitimate` -> legally constituted, governed or community-authorized;
- `authentic` -> place-rooted, lineage-based or community-held;
- `meaningful` -> relationship-based, long-duration or high-engagement;
- `deep` -> immersive, field-based or multi-year;
- `living knowledge` -> place-based craft transmission or intergenerational practices;
- `institution` -> prototype or pilot initiative when describing the current state.

---

## Current blockers

| Blocker | Required resolution |
|---------|---------------------|
| Legal form unresolved | Compare fiscal sponsorship, Portuguese association and future nonprofit paths |
| Advisor roles unfilled | Recruit candidates only after role letters and authority limits are clear |
| No practitioner relationships verified | Keep names and field claims internal until consented |
| Archive tooling unresolved | Evaluate Mukurtu or equivalent access-control model before custom build |
| Old docs still overlap with new authority | Add status labels and route readers to canonical docs |

---

## Repo conventions for agents

- Preserve `src/chat.md` as archive.
- Do not delete exploratory materials until they are explicitly archived.
- Prefer updating `docs/00-overview.md` when document authority changes.
- Keep secrets (`.env`, tokens) out of commits.
- Do not commit unrelated modified files.
- Commits use imperative mood and should focus on why.

---

## Immediate next instruction

Continue Phase IV consolidation only:

1. Keep the canonical operating spine current.
2. Mark old conceptual docs with status and visibility labels.
3. Resolve duplicated authority by routing readers to canonical docs.
4. Run public-language scans before any public page update.
5. Do not add strategy, product scope or atlas expansion.

---

## Contact / ownership

- **Founder:** Braulio Sotomayor (`brauliosotomayor`)
- **GitHub:** https://github.com/brauliosotomayor/studium
