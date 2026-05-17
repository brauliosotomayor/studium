# Pilot Map & Discovery Logic

**Version:** Remediated Phase II · 2026-05-17  
**Status:** UX planning note; no app implementation yet

---

## Design intent

The first interface should support **field documentation and careful discovery**, not broad consumer browsing. The map should help a small team understand where relationships exist, what permissions apply, and what documentation is ready for review.

Public-facing language should describe this as a **pilot map prototype**, not a completed atlas.

---

## Current use case

| Need | Interface response |
|------|--------------------|
| Show the current pilot area | Northern Portugal region card and research boundary |
| Track practitioner relationships | Candidate / contacted / consented / documented statuses |
| Record stewardship review | Steward contact, permission level, restrictions |
| Avoid over-publication | Hide sensitive locations until approved |
| Support fieldwork | Interview checklist, photo permissions, archive notes |

---

## Map layers

| Layer | Default | Description |
|-------|---------|-------------|
| **Pilot region** | On | Northern Portugal research area |
| **Practitioner status** | On | Candidate, contacted, consented, documented |
| **Craft focus** | On | Practical categories such as vineyard stewardship, stone, cork, ceramics |
| **Stewardship review** | On | Consent status, media limits, community partner |
| **Sensitivity** | On | Low / Medium / High review requirement |
| **Archive readiness** | Off | Whether interview, photos, and permissions are publishable |

---

## Zoom levels

| Level | View | Behavior |
|-------|------|----------|
| **Region** | Northern Portugal | Show pilot scope and methodology |
| **Sub-region** | Douro, Minho, Serra da Estrela, Tras-os-Montes | Show research areas, not exact private sites |
| **Practitioner** | Approved relationships only | Show craft, consent status, and documentation summary |
| **Workshop / field site** | Restricted | Visible only after explicit permission |

---

## Filters

| Filter | Purpose |
|--------|---------|
| Craft / stewardship focus | Understand pilot coverage |
| Relationship status | Separate real relationships from dataset candidates |
| Documentation status | Interviewed, photographed, reviewed, publishable |
| Sensitivity | Apply additional review before display |
| Steward type | Practitioner, community partner, land steward, institution |

Avoid filters for price, popularity, ratings, or “near me” discovery.

---

## Practitioner card

```text
Craft / stewardship title
Sub-region · Portugal

Status: contacted / consented / documented
Stewardship review: pending / approved / restricted
Documentation: interview, workshop photos, field notes

Primary action: request review
Not: instant book
```

---

## Publication rules

1. Exact private locations stay hidden unless approved.
2. A practitioner card should not go public before consent and review.
3. Sensitive practices require additional cultural or ecological review.
4. Student applications should open only after the pilot model is tested.
5. The interface should always distinguish source data from field-verified relationships.

---

## Static site use

The current `docs/index.html` should present:

- current pilot status;
- what exists today;
- what remains experimental;
- stewardship principles;
- documentation method;
- links to working documents.

It should not present a broad global map as if it already exists operationally.

---

## Next UX deliverable

After founder decisions D1-D3, create:

`docs/11-pilot-ia-and-data-model.md`

Required contents:

- relationship status lifecycle;
- field documentation schema;
- consent and media permission model;
- minimal public profile fields;
- admin-only fields for steward review;
- criteria for when a candidate becomes public.
