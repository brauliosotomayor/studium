# Technology and Data Architecture

**Version:** Phase III · 2026-05-17  
**Status:** Internal architecture constraints before implementation

---

## Purpose

This document defines the technology posture for Studium: data and tools must support consent, stewardship and archive governance. Technology must not create scale pressure before governance exists.

Do not build an app, marketplace, public map or booking system before governance, consent and archive architecture are approved.

---

## Architecture principle

The archive is a governed record system, not a growth product. Access rules, consent records and stewardship decisions are first-class data.

---

## Mukurtu-first archive logic

Studium should evaluate Mukurtu or a Mukurtu-aligned approach before inventing a custom archive because it supports:

- community-controlled access protocols;
- cultural metadata;
- restricted sharing;
- differential access by community or role;
- archive governance patterns beyond simple public/private toggles.

The decision is not "use Mukurtu at all costs." The decision is that any tool must support equivalent consent and stewardship controls before storing sensitive records.

---

## Data objects

| Object | Purpose | Public by default |
|--------|---------|-------------------|
| Practitioner record | Relationship, status, craft, consent and compensation notes | No |
| Steward record | Review role and authority | No |
| Consent record | Approved uses, restrictions, withdrawal terms | No |
| Archive item | Interview, photo, field note, transcript or metadata | No |
| Place record | Region, sub-region, site sensitivity and location precision | No |
| Student application | Intent, screening, conduct agreement | No |
| Partner target | Outreach status and relationship notes | No |
| Risk item | Failure pattern, owner, mitigation and review | No |

Public display should be generated only from approved fields, never directly from raw records.

---

## Metadata schema

Minimum archive metadata:

- archive ID;
- title or working label;
- material type;
- practitioner or steward link;
- place precision level;
- sensitivity;
- consent ID;
- access tier;
- allowed uses;
- prohibited uses;
- review date;
- withdrawal terms;
- steward decision ID;
- storage location;
- public summary approval status.

---

## Access tiers

| Tier | Description | Technical requirement |
|------|-------------|-----------------------|
| Public | Approved for public display | Separate reviewed public copy |
| Internal restricted | Studium team only | Role-based access and audit log |
| Practitioner-only | Returned to or controlled by practitioner | Export and deletion path |
| Community / steward | Shared with defined reviewers | Named access group |
| Sealed | Stored but not accessed without re-approval | Access disabled except archive steward |
| Withdrawn | Removed from active use | Tombstone record without sensitive content |

---

## Data sovereignty rules

1. Consent controls use, not possession.
2. Raw documentation remains restricted unless explicitly approved.
3. Exact site data is hidden unless site permission exists.
4. Community-controlled knowledge requires community-level review.
5. Withdrawal and restriction must be technically possible.
6. Public summaries must be separate from raw archive material.
7. No archive material may be used for AI training, dataset licensing or automated enrichment without explicit future governance approval.

---

## Prohibited technology before governance exists

Do not build:

- public marketplace;
- instant booking;
- public global atlas;
- recommendation or ranking system;
- creator or influencer publishing flow;
- student self-service access to sensitive records;
- AI feature using practitioner documentation;
- automated scraping or enrichment pipeline;
- public map with exact private locations.

---

## Allowed Phase III tooling

Allowed tools are administrative and low-scale:

- CSV registers for planning;
- private consent tracker;
- private archive inventory;
- restricted file storage;
- decision log;
- public static pages only for pilot-stage language;
- internal map notes without exact sensitive locations.

---

## Technology readiness gate

No app or marketplace planning should proceed until:

- governance decision rights are documented;
- consent workflow is approved;
- archive schema and access tiers are tested;
- first three practitioner relationships have consent records;
- compensation and participation terms are drafted;
- legal and safety review exists for student activity;
- advisory review approves the next product scope.

---

## Data minimization

Collect the least sensitive useful data:

- use sub-region instead of exact address by default;
- use status categories instead of private notes in shared files;
- store contact details outside public repository files;
- separate consent records from public summaries;
- do not store signatures or identity documents in CSVs;
- delete or restrict raw material if its purpose is unclear.

