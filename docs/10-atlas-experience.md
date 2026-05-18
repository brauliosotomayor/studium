# Pilot Map & Discovery Logic

**Version:** Remediated Phase II · 2026-05-17  
**Status:** Deferred UX planning note before app implementation  
**Visibility:** Internal  
**Canonical gate:** Use `19-technology-and-data-architecture.md` before any app, map or public prototype work.

This file is a future product reference. It does not authorize app, marketplace, public map or booking implementation before governance, consent and archive controls are tested.

---

## Design intent

The first interface should support **field documentation and careful discovery**. The map should help a small team understand where relationships exist, what permissions apply and what documentation is ready for review.

Public-facing language should describe this as a **pilot map prototype** during field validation.

---

## Current use case

| Need | Interface response |
|------|--------------------|
| Show the current pilot area | Northern Portugal region card and research boundary |
| Track practitioner relationships | Candidate / contacted / consented / documented statuses |
| Record steward review | Steward contact, permission level, restrictions |
| Publication restraint | Hide sensitive locations until approved |
| Support fieldwork | Interview checklist, photo permissions, archive notes |

---

## Map layers

| Layer | Default | Description |
|-------|---------|-------------|
| **Pilot region** | On | Northern Portugal research area |
| **Practitioner status** | On | Candidate, contacted, consented, documented |
| **Craft focus** | On | Practical categories such as vineyard management, stone, cork, ceramics |
| **Steward review** | On | Consent status, media limits, local review partner |
| **Sensitivity** | On | Low / Medium / High review requirement |
| **Archive readiness** | Off | Whether interview, photos and permissions are publishable |

---

## Zoom levels

| Level | View | Behavior |
|-------|------|----------|
| **Region** | Northern Portugal | Show pilot scope and methodology |
| **Sub-region** | Douro, Minho, Serra da Estrela, Tras-os-Montes | Show research areas while protecting private sites |
| **Practitioner** | Approved relationships only | Show craft, consent status and documentation summary |
| **Workshop / field site** | Restricted | Visible only after explicit permission |

---

## Filters

| Filter | Purpose |
|--------|---------|
| Craft / land-management focus | Understand pilot coverage |
| Relationship status | Separate verified relationships from dataset candidates |
| Documentation status | Interviewed, photographed, reviewed, publishable |
| Sensitivity | Apply additional review before display |
| Steward type | Practitioner, local partner, land steward, advisor |

Use filters for field readiness, consent, craft focus and steward review status before commercial discovery.

---

## Practitioner card

```text
Craft / land-management title
Sub-region · Portugal

Status: contacted / consented / documented
Steward review: pending / approved / restricted
Documentation: interview, workshop photos, field notes

Primary action: request review
Primary action: request review
```

---

## Publication rules

1. Exact private locations stay hidden unless approved.
2. A practitioner card becomes public after consent and review.
3. Sensitive practices require additional cultural or ecological review.
4. Student applications should open only after the pilot model is tested.
5. The interface should always distinguish source data from field-verified relationships.

---

## Static site use

The current `docs/index.html` should present:

- current pilot status;
- what exists today;
- what remains experimental;
- steward authority principles;
- documentation method;
- links to working documents.

It should present the current pilot map prototype and distinguish field-verified relationships from source data.

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
