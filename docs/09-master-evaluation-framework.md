# Founder Candidate Evaluation System

**Version:** Phase II · 2026-05-17  
**Status:** Scoring framework for atlas inclusion (not booking ratings)

---

## Purpose

Evaluate **whether a practitioner should become an atlas node**—not whether they are “good enough” as a brand. Studium seeks **living archives**, not service providers.

**Output:** `Candidate` → `Founding 13` → `Active` → `Archive (honored)` statuses in CSV.

---

## Scoring model (100 points)

| Criterion | Weight | Description |
|-----------|--------|-------------|
| **Lineage depth** | 20 | Years of practice, named teachers, generational continuity |
| **Ecological relevance** | 15 | Place-based systems; climate and land integration |
| **Teaching capacity** | 15 | Ability and willingness to transmit (not just perform) |
| **Continuity risk** | 15 | Urgency: knowledge endangered if node not supported |
| **Geographic importance** | 10 | Helps balance the pilot or future corridor dataset |
| **Symbolic importance** | 10 | Founding 13 balance; represents underrepresented archetype |
| **Accessibility** | 5 | Travel feasibility without tourism distortion |
| **Stewardship alignment** | 10 | Steward partner available; anti-extraction fit |

---

## Rubric detail

### Lineage depth (0–20)

| Score | Indicator |
|-------|-----------|
| 18–20 | 20+ years; named lineage; apprentices produced |
| 12–17 | 10–20 years; clear teacher chain |
| 6–11 | Skilled practitioner; lineage partially documented |
| 0–5 | Recent skill; insufficient transmission history |

### Ecological relevance (0–15)

| Score | Indicator |
|-------|-----------|
| 13–15 | Land stewardship core to practice |
| 8–12 | Craft integrated with local ecology |
| 4–7 | Place-aware but craft-primary |
| 0–3 | No meaningful land connection |

### Teaching capacity (0–15)

| Score | Indicator |
|-------|-----------|
| 13–15 | Active apprentices; structured pedagogy |
| 8–12 | Willing to teach small groups |
| 4–7 | Teaching possible with support |
| 0–3 | Performance only; refuses transmission |

### Continuity risk (0–15)

| Score | Indicator |
|-------|-----------|
| 13–15 | UNESCO/endangered context; <10 global practitioners |
| 8–12 | Aging master; declining apprentices |
| 4–7 | Stable but worth preserving |
| 0–3 | Thriving industrial alternative exists |

### Geographic importance (0–10)

| Score | Indicator |
|-------|-----------|
| 9–10 | Fills empty corridor or Founding 13 slot |
| 5–8 | Strengthens existing cluster |
| 0–4 | Redundant with nearby nodes |

### Symbolic importance (0–10)

| Score | Indicator |
|-------|-----------|
| 9–10 | Completes archetype or cultural balance in Founding 13 |
| 5–8 | Supports documented regional balance |
| 0–4 | Marginal symbolic contribution |

### Accessibility (0–5)

| Score | Indicator |
|-------|-----------|
| 5 | Reachable without resort infrastructure |
| 3 | Moderate access; steward supports logistics |
| 0 | Access requires exploitative tourism chain |

### Stewardship alignment (0–10)

| Score | Indicator |
|-------|-----------|
| 9–10 | Steward partner committed; framework signed |
| 5–8 | Steward identified; onboarding in progress |
| 0–4 | No steward; High sensitivity without path |

---

## Decision thresholds

| Total | Decision |
|-------|----------|
| **85–100** | Founding 13 priority — fast track with steward |
| **70–84** | Approved candidate — standard onboarding |
| **55–69** | Hold — develop steward or teaching plan |
| **<55** | Decline or revisit in 12 months |

**Veto:** Any High sensitivity node without steward partner — automatic hold regardless of score.

---

## Evaluation workflow

1. **Nomination** — Data in `studium_atlas_master.csv` with `Status = Candidate`  
2. **Desk research** — Notes, endangered context, archetype fit  
3. **Founder interview** — 60–90 min; teaching intent  
4. **Steward consultation** — Required for Medium/High  
5. **Scorecard** — Document in internal record (future: `data/evaluations/`)  
6. **Council** — Founder + steward sign-off for Founding 13  
7. **Update CSV** — `Founder Phase`, `Status`

---

## Founding 13 prioritization

Within score band 85+, rank by:

1. Continuity risk (desc)  
2. Corridor gap (geographic)  
3. Archetype gap (taxonomic)  
4. Founder signal alignment (Douro anchor first)

---

## Anti-patterns (automatic decline)

- Instant booking expectation  
- Refusal of apprentice time commitment  
- No community or steward contact  
- Commoditized “experience” packaging  
- Intellectual property hoarding with no transmission  

---

## Related artifacts

- `08-stewardship-framework.md`  
- `07-founding-13.md`  
- `data/studium_atlas_master.csv`
