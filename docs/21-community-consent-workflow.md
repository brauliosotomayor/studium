# Community Consent Workflow

**Version:** Phase IV draft · 2026-05-17
**Status:** Drafted operating workflow before practitioner outreach, archive ingestion, field documentation or public representation

---

## Purpose

This workflow defines the consent sequence Studium must complete before any work affects a practitioner, community, site, archive record or public representation.

This document is a drafted system. It becomes implemented only after named owners, secure storage, review logs and signed consent records exist.

---

## Consent layers

| Layer | Authority | Scope | Required record |
|-------|-----------|-------|-----------------|
| Individual consent | Named person being interviewed, photographed, recorded or quoted | Personal story, likeness, voice, name, biography and personal participation | Individual consent record |
| Practitioner consent | Practitioner hosting documentation, teaching, review or apprenticeship activity | Workshop access, teaching scope, compensation, media selection and profile review | Practitioner agreement |
| Community authority consent | Recognized community steward, association, cooperative, elder group, lineage holder or local governance body | Shared practice, place context, collective representation, community-only archive access and public framing | Community consent agreement |
| Land or site consent | Site owner, land steward, workshop host or authorized custodian | Site access, seasonal limits, location precision, safety rules and ecological restrictions | Site permission note |
| Archive consent | Participant plus archive steward with any required community authority | Storage, metadata, access tier, review cadence, export, restriction, withdrawal and deletion | Archive permission record |

Participation in a conversation, visit, interview or demonstration grants no documentation right by itself.

---

## Operational owners

| Function | Owner before implementation | Owner after implementation | Completion evidence |
|----------|-----------------------------|----------------------------|---------------------|
| Consent intake | Founder | Consent coordinator or governance steward | Dated intake checklist |
| Authority mapping | Founder with local advisor | Community steward or local coordinator | Authority map with source notes |
| Consent negotiation | Founder plus governance advisor | Consent coordinator plus relevant steward | Signed or recorded consent decision |
| Archive tier assignment | Archive steward | Archive steward | Access tier log entry |
| Public-use review | Communications owner | Communications owner plus steward reviewer | Approved publication record |
| Revocation handling | Archive steward | Archive steward plus governance steward | Revocation log and action timestamp |
| Dispute escalation | Governance steward | Governance steward plus advisory reviewer | Escalation decision note |

---

## Workflow

| Step | Action | Owner | Required output | Completion criterion |
|------|--------|-------|-----------------|----------------------|
| 1. Introduction | Provide a plain-language brief covering Studium status, planned activity, documentation types, storage, possible audiences, compensation and rights to decline | Consent coordinator | Introduction note | Recipient confirms receipt before any documentation |
| 2. Authority identification | Identify individual, practitioner, community and site authorities affected by the work | Consent coordinator with local advisor | Authority map | Each authority type marked applicable, not applicable or unresolved |
| 3. Harm classification | Complete `data/studium_documentation_harm_matrix.csv` fields for proposed activity | Archive steward | Harm assessment row | Risk level assigned before consent negotiation |
| 4. Consent negotiation | Review allowed uses, denied uses, access tier, review dates, compensation and withdrawal terms | Consent coordinator | Draft consent record | All non-public permissions recorded as restricted until signed |
| 5. Community authority review | Submit community-affecting material and framing to identified authority | Community steward | Review decision | Community authority approves, restricts, revises or declines |
| 6. Documentation permission | Confirm media types, location precision and archive scope before capture | Practitioner or site authority | Capture permission note | Media scope and storage path recorded before capture |
| 7. Archive entry | Store material under restricted default access with linked consent ID | Archive steward | Archive record | Access tier set to `internal_restricted`, `community_only`, `practitioner_only` or `sealed` unless public approval exists |
| 8. Participant review | Share transcripts, captions, clips, images or summaries for review | Documentation owner | Review packet | Reviewer decision logged with timestamp |
| 9. Steward review | Review community-sensitive, site-sensitive or high-risk materials | Relevant steward | Steward decision | Decision logged before access tier change |
| 10. Publication or access change | Change access only after required approvals | Archive steward | Access change record | Public, community or practitioner access matches signed approval |
| 11. Ongoing review | Reconfirm consent at scheduled date or when use, audience or context changes | Archive steward | Review renewal, restriction or withdrawal | Review completed by due date or access remains restricted |

---

## Archive permission default

All new archive records start at restricted access. Public access requires all applicable approvals:

1. Individual approval for name, likeness, voice, quote or personal story.
2. Practitioner approval for workshop, teaching method, profile or compensation references.
3. Community authority approval for shared practice, place context, lineage or community representation.
4. Site authority approval for location precision above region level.
5. Archive steward confirmation that the record has consent ID, access tier, review date, withdrawal terms and audit log entry.

If any approval is missing, expired, disputed or unclear, the archive steward keeps or moves the record to restricted access.

---

## Review cycles

| Trigger | Reviewer | SLA | Default during review |
|---------|----------|-----|-----------------------|
| New consent record | Archive steward | 5 business days | Restricted |
| New media capture | Practitioner or participant | 10 business days | Restricted |
| Community-affecting material | Community authority | 20 business days | Community-only or sealed |
| High-risk documentation | Governance steward plus advisor | 30 business days | Sealed |
| Public-use request | Participant plus required steward | 15 business days | Restricted |
| Use, audience or platform change | Original authority where reachable | 15 business days | Restricted |
| Withdrawal or restriction request | Archive steward | First action within 2 business days | Access suspended |

---

## Withdrawal and revocation

Any individual, practitioner, community authority or site authority may restrict or revoke access for materials under their authority.

Revocation procedure:

1. Archive steward receives the request and timestamps it.
2. Archive steward suspends public and shared access within 2 business days.
3. Consent coordinator identifies affected archive IDs, public pages, media exports and derived text.
4. Governance steward reviews external obligations, printed materials or third-party copies.
5. Archive steward updates access tier to `withdrawn`, `sealed`, `practitioner_only` or `community_only`.
6. Communications owner removes affected public material within 5 business days when applicable.
7. Archive steward records action, owner, timestamp, affected paths and next review date.

The revocation log must not expose sensitive reasoning in public repository files.

---

## Dispute escalation

| Dispute | First action | Escalation owner | Required decision |
|---------|--------------|------------------|-------------------|
| Practitioner disputes wording, caption or image | Restrict affected material | Governance steward | Revise, withdraw, seal or retain restricted |
| Community authority disputes representation | Remove public access | Governance steward plus community steward | Community-approved wording or no public use |
| Site authority disputes location display | Hide location and maps | Archive steward | Region-only, sealed or withdrawn |
| Individual and community permissions conflict | Restrict material | Governance steward plus advisory reviewer | Narrowest access level controls |
| External party requests restricted material | Deny by default | Archive steward | Release only with all required approvals |

---

## Audit traceability

Each consent and access action must record:

- record ID;
- authority type;
- owner who recorded the action;
- reviewer name or coded reviewer ID;
- timestamp;
- source document pointer;
- access tier before and after;
- approval, restriction, denial or revocation result;
- affected archive IDs;
- next review date;
- escalation path if unresolved.

Completion is measurable only when the audit record exists outside chat memory and links to the archive record.
