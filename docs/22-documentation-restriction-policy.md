# Documentation Restriction Policy

**Version:** Phase IV draft · 2026-05-17
**Status:** Drafted restriction policy before archive ingestion and field documentation

---

## Purpose

This policy defines documentation access categories, prohibited documentation conditions and required ownership for restricting, sealing, reviewing or publishing Studium materials.

This policy is drafted. It becomes implemented only when archive records, storage controls and audit logs enforce these categories.

---

## Access categories

| Category | Function | Who approves | Who records | Who stores | Who reviews | Who can revoke |
|----------|----------|--------------|-------------|------------|-------------|----------------|
| Sealed | Store material with no routine access pending explicit re-approval | Individual, practitioner or community authority plus archive steward | Archive steward | Archive steward in restricted storage | Governance steward at review date | Authority who granted consent, archive steward for risk, governance steward for harm |
| Community-only | Permit access only to named community reviewers or partner group | Community authority | Archive steward | Archive steward with named access group | Community authority and archive steward | Community authority or governance steward |
| Practitioner-only | Return or hold material for the practitioner without Studium reuse | Practitioner | Archive steward | Archive steward or practitioner export channel | Practitioner | Practitioner |
| Internal restricted | Permit Studium internal review for consent, editing, risk or archive work | Archive steward | Archive steward | Archive steward | Archive steward and governance steward | Participant, practitioner, community authority, archive steward |
| Public | Permit approved public display or release | All applicable individual, practitioner, community and site authorities | Communications owner plus archive steward | Public copy stored apart from raw archive | Communications owner and relevant steward | Any granting authority can request restriction review |
| Withdrawn | Remove from active use and retain only a tombstone record where needed | Granting authority or governance steward | Archive steward | Tombstone record without sensitive content | Governance steward | Granting authority controls any future re-entry |

---

## Default rule

All documentation defaults to `internal_restricted` before review. Use `sealed` when:

- community authority is unresolved;
- harm level is high;
- material includes restricted knowledge;
- exact site data appears;
- consent scope is unclear;
- withdrawal request is pending;
- access tier conflicts with reviewer instruction.

Public access is an exception that requires affirmative review, timestamped approval and access-tier change logging.

---

## Restriction triggers

| Trigger | Required category | Owner | Completion criterion |
|---------|-------------------|-------|----------------------|
| Pre-consent note, image, audio or transcript | Internal restricted | Archive steward | Consent ID absent or draft status marked restricted |
| Sensitive method, trade detail or teaching sequence | Sealed | Practitioner plus archive steward | Public excerpt field left blank |
| Shared community knowledge | Community-only or sealed | Community authority | Named review group recorded |
| Exact private location | Sealed or internal restricted | Site authority plus archive steward | Location precision reduced to region or sub-region |
| Youth, vulnerable person or private household | Sealed | Governance steward | Advisor review required before any use |
| Practitioner profile draft | Internal restricted | Documentation owner | Draft marked not public until practitioner approval |
| Raw field notes | Internal restricted | Documentation owner | Stored outside public repository |
| Revocation request | Withdrawn, sealed or practitioner-only | Archive steward | Access suspended and action logged |
| Disputed public copy | Internal restricted | Communications owner | Public page removed or revised pending review |

---

## Prohibited documentation conditions

Studium must not document, store or publish under these conditions:

1. A person declines recording, photography, transcription or note-taking.
2. A practitioner permits participation but denies documentation.
3. A community authority has not reviewed shared knowledge or community representation.
4. A site owner or land steward denies location capture.
5. Documentation would reveal restricted knowledge, sacred practice, trade method, ecological vulnerability or private route.
6. Compensation, review rights or withdrawal terms have not been explained.
7. Student or visitor media capture is proposed without practitioner approval.
8. Documentation is requested to satisfy funder, marketing or product needs before consent.
9. Archive storage cannot enforce the assigned access tier.
10. The person recording cannot identify who approves, records, stores, reviews and revokes the material.

If a prohibited condition appears during fieldwork, documentation stops and any captured material becomes sealed until review.

---

## Category change procedure

| Change | Required approval | Required log fields |
|--------|-------------------|---------------------|
| Internal restricted to public | Individual, practitioner and any applicable community or site authority | requester, approvers, timestamp, archive IDs, public copy path, review date |
| Internal restricted to community-only | Community authority and archive steward | named access group, reviewer, expiration or review date |
| Sealed to any access tier | Original authority plus governance steward | reason for reopening, scope, access tier, next review |
| Public to restricted | Any granting authority or governance steward | takedown time, affected surfaces, replacement status |
| Any tier to withdrawn | Granting authority or governance steward | withdrawal type, retained tombstone fields, future-use rule |

No category change is complete until the archive record, access log and review calendar are updated.

---

## Storage rules

| Material type | Storage rule | Public repository rule |
|---------------|--------------|------------------------|
| Consent agreements | Secure private storage with pointer ID | No signatures, addresses, phone numbers or identity documents |
| Raw audio or video | Restricted media storage | No raw files |
| Transcripts | Restricted text storage | Approved excerpts only |
| Photos | Restricted media storage with image-level access tier | Approved public copies only |
| Field notes | Restricted internal storage | Summaries only after review |
| Metadata | Archive system or CSV schema with coded IDs | No sensitive notes |
| Public summaries | Public docs or website | Must link to approval record internally |

---

## Enforcement checks

Before any material leaves restricted storage, the archive steward verifies:

- consent ID exists;
- consent status is active;
- applicable authority layers are recorded;
- access tier allows the proposed use;
- prohibited uses do not include the proposed use;
- review date has not passed;
- withdrawal status is `none_requested`;
- public copy is separate from raw material;
- audit log records the release.

If any check fails, release is denied and the material remains restricted or sealed.
