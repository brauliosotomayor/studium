# Orchestrator Handoff — Studium

**Repo:** `brauliosotomayor/studium`  
**Branch:** `main`  
**Last updated:** 2026-05-17 (credibility remediation complete)  
**Audience:** Remote orchestrator / agent coordinator assigning work to subagents

---

## Critical remediation complete

Public positioning has been narrowed from broad atlas/institutional language to:

> **Pilot stewardship network for place-based apprenticeship and cultural preservation.**

Use a research posture. Do not speak as an institution, imply field validation that does not exist, or foreground symbolic planning models.

### Current public framing

| Item | Current stance |
|------|----------------|
| Stage | Pre-fieldwork prototype |
| Public scope | One-region Northern Portugal pilot |
| Near-term proof | 3 documented practitioner relationships |
| App code | Not started; do not build yet |
| Required evidence | Interviews, field photography, consent terms, steward review |

### Prohibited public framing

- broad legacy-scale language
- symbolic scale explanations
- global representation claims
- marketplace language that sounds like tourism or creator bookings
- claims of institutional authority before advisors and partners exist

---

## Phase II complete (atlas infrastructure)

| Deliverable | Path | Status |
|-------------|------|--------|
| P0 Corridor registry | `docs/05-corridor-registry.md` | ✅ |
| P1 Knowledge archetypes | `docs/06-knowledge-archetypes.md` | ✅ |
| P2 Founding 13 | `docs/07-founding-13.md` | ✅ |
| P3 Atlas CSV | `data/studium_atlas_master.csv` (266 nodes) | ✅ |
| P4 Stewardship | `docs/08-stewardship-framework.md` | ✅ |
| P5 Evaluation | `docs/09-master-evaluation-framework.md` | ✅ |
| P6 Map UX | `docs/10-atlas-experience.md` | ✅ |
| P7 Site | `docs/index.html` + `docs/assets/` | ✅ |

**Next phase:** Proof of Reality — 3 practitioner relationships, one steward framework tested in practice, one documented interview, and a participation / consent policy. **No app code yet.**

---

## Mission (one sentence)

Build a small, documented pilot for **Studium**: place-based apprenticeship with craftspeople and land stewards, starting in Northern Portugal, governed by consent, community review, and measured outcomes.

---

## Current state

| Area | Status |
|------|--------|
| Vision & strategy | ✅ Documented in `docs/` (split from `src/chat.md`) |
| Atlas taxonomy & CSV | ✅ Phase II (`05–10`, `studium_atlas_master.csv`) |
| Brand / manifesto | ✅ `docs/03-manifesto.md` |
| Product philosophy | ✅ `docs/02-triangle-philosophy.md` |
| Business case | ✅ `docs/01-marketplace-and-business.md` |
| Pilot spec | ✅ `docs/04-pilot-plan.md` (includes open questions) |
| Code / app | ❌ Not started |
| Practitioner relationships | ❌ Not documented publicly |
| Design system / UI | ❌ Not started |
| Legal / payments / liability | ❌ Not specified |

**Canonical source of truth for product intent:** `docs/00-overview.md` → linked docs. Do not re-derive strategy from `src/chat.md` unless reconciling gaps.

---

## Non-negotiables (from founder conversation)

1. **Not tourism** — devotion to learning; reject experiences-marketplace positioning.
2. **Place-rooted** — every experience tied to geography, lineage, and steward context.
3. **Triangle is internal model** — public materials should lead with fieldwork, consent, and governance.
4. **Start narrow** — crafts in Southern Europe before full ecology/land expansion.
5. **Pilot before scale** — year one proves masters participate, students commit deeply, and stories spread organically.
6. **Minimal v1 app** — map, master profiles, listings, applications, secure booking only.

---

## Priority queue for next work

Assign subagents in parallel where tasks are independent. Respect dependencies noted.

### P0 — Decisions (human or orchestrator-led)

| ID | Task | Owner | Blocks |
|----|------|-------|--------|
| D1 | Choose first **practitioner relationship** to document | Founder | Fieldwork, outreach |
| D2 | Confirm first field site / sub-region in Northern Portugal | Founder | Logistics, photography |
| D3 | Resolve first craft / stewardship focus | Founder | Interview protocol |

### P1 — Parallel workstreams (no code required yet)

| ID | Task | Suggested output | Depends on |
|----|------|------------------|------------|
| W1 | **Practitioner relationship brief** — one real candidate, contact path, consent questions | `docs/11-practitioner-relationship-brief.md` | D1, D2 |
| W2 | **Documentation playbook** — interview, photo, permissions, archive standards | `docs/12-documentation-playbook.md` | D1 |
| W3 | **Consent and participation policy** — student, practitioner, steward terms | `docs/13-consent-participation-policy.md` | D1 |
| W4 | **Pilot economics** — compensation, fees, expenses, cancellation, liability boundaries | `docs/14-pilot-economics.md` | D1 |
| W5 | **Advisor map** — academic, cultural, ecological advisor candidates | `docs/15-advisor-map.md` | — |

### P2 — Product & technical (after P0 decisions)

| ID | Task | Suggested output | Depends on |
|----|------|------------------|------------|
| T1 | **Information architecture** — pages, flows, data model for v1 | `docs/10-ia-and-data-model.md` | D3, W2 |
| T2 | **Wireframes** — map, profile, listing, apply, book | `design/` or Figma link in doc | T1 |
| T3 | **Tech stack proposal** — map provider, auth, payments, hosting | `docs/11-tech-stack.md` | T1 |
| T4 | **MVP implementation** — scaffold app per pilot scope | `app/` | T1–T3 |

### P3 — Business operations

| ID | Task | Suggested output |
|----|------|------------------|
| B1 | Booking/payments/cancellation policy draft | `docs/12-operations-policy.md` |
| B2 | Master agreement / revenue share template | `docs/13-master-agreement-draft.md` |
| B3 | Content license for student/master documentation | `docs/14-content-license.md` |

---

## Suggested subagent prompts (copy-paste)

**W1 — Founding masters**
> Read `docs/04-pilot-plan.md` and `docs/01-marketplace-and-business.md`. Draft `docs/05-founding-masters.md`: 10 candidate master profiles (fictional or template placeholders) across Northern Portugal sub-regions, with craft/land type, sample workshop title, and why they fit the founding circle. Flag which slot should be the founding master per open questions.

**W2 — Experience catalog**
> Read `docs/04-pilot-plan.md`. Create `docs/06-experience-catalog.md` with 3–5 apprenticeship templates (duration, group size, price range €, learning outcomes). Align with pilot metrics (3–6 students per run, ~50 completions/year).

**T1 — IA and data model**
> Read `docs/02-triangle-philosophy.md`, `docs/04-pilot-plan.md`, and `docs/00-overview.md`. Produce `docs/10-ia-and-data-model.md`: entities (Student, Master, Steward, Place, Experience, Application, Booking), core user flows, and v1 feature exclusions.

---

## Success metrics (year one — do not change without founder approval)

- 10 participating masters  
- ~50 students completing apprenticeships  
- Meaningful documented stories (photos, film, interviews)  
- 1–2 institutional partnerships emerging  

---

## Risks and blockers

| Risk | Mitigation |
|------|------------|
| Scope creep (social, feed, AI features) | Enforce v1 exclusions in `docs/04-pilot-plan.md` |
| Tourism positioning | Manifesto and copy review on all outward-facing material |
| Master cold-start | Prioritize D1 founding master + personal network outreach |
| Auth/push to GitHub from local agent | Human runs `gh auth login` once; then `git push origin main` |

---

## Repo conventions for agents

- New strategy docs: `docs/NN-slug.md` (increment number)  
- Do not edit `src/chat.md` (archive)  
- Prefer updating `docs/00-overview.md` doc map when adding files  
- No commits containing secrets (`.env`, tokens)  
- Commits: imperative mood, focus on *why*  

---

## Immediate next instruction (for orchestrator)

1. **Confirm** founder decisions **D1–D3** (or assign a subagent to draft options doc for founder review).  
2. **Launch in parallel:** W1, W2, W3, W4, W5 (five subagents, read-only on `src/chat.md`).  
3. **Gate** T1–T4 until D3 and W2 drafts exist.  
4. **Report back** with links to new docs and updated open-questions list in `docs/04-pilot-plan.md`.

---

## Contact / ownership

- **Founder:** Braulio Sotomayor (`brauliosotomayor`)  
- **GitHub:** https://github.com/brauliosotomayor/studium  
