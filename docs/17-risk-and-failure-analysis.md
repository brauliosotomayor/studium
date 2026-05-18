# Risk and Failure Analysis

**Version:** Phase III · 2026-05-17  
**Status:** Operating risk register and failure monitoring model

---

## Purpose

This document defines Studium's failure-pattern registry, risk matrix, mitigation ownership and stop / pivot / continue criteria.

The goal is not to eliminate risk. The goal is to see failure early enough to slow down, repair, restrict or stop.

---

## Risk categories

| Category | Description | Primary owner |
|----------|-------------|---------------|
| Governance | Missing entity, unclear authority, founder overreach | Governance steward |
| Consent | Documentation without valid permission or review | Archive steward |
| Community harm | Misrepresentation, unwanted exposure, local disruption | Stewardship reviewer |
| Practitioner burden | Underpaid, over-documented or over-scheduled participation | Founder |
| Archive exposure | Sensitive records accessible too widely | Archive steward |
| Legal / liability | Safety, payment, privacy or contract gaps | Legal advisor |
| Funding distortion | Money changes priorities toward outputs or scale | Governance steward |
| Technology drift | App or marketplace work begins before governance readiness | Founder |
| Public language | Claims exceed evidence | Communications owner |

---

## Failure-pattern registry

| Failure pattern | Early warning | Mitigation | Stop trigger |
|-----------------|---------------|------------|--------------|
| Consent debt | Media or notes lack consent ID | Freeze publication and audit records | Material cannot be matched to consent |
| Public overclaiming | Copy implies active partners or global authority | Rewrite and add evidence gate | Partner or practitioner disputes claim |
| Practitioner extraction | More asks than compensation or benefit | Reduce scope; pay review time | Practitioner reports harm or burden |
| Archive leakage | Restricted material appears in public location | Remove, audit access, notify affected person | Sensitive material exposed externally |
| Governance theater | Advisors named without authority | Define charter or remove claim | Advisor objects to representation |
| Student access too early | Recruitment before safety and agreements | Close applications and complete policies | Student activity occurs without agreement |
| Funding capture | Grant deliverables exceed capacity | Renegotiate or decline | Funding requires violating consent or pace |
| Technology scale bias | Roadmap prioritizes bookings, ranking or growth | Gate product work through governance | App build starts before approval |
| Atlas expansion | New regions published before pilot proof | Reclassify internal | Public corridor claim made without fieldwork |

---

## Risk matrix

| Severity | Meaning | Example |
|----------|---------|---------|
| Low | Manageable operational issue | Late review, unclear checklist |
| Medium | Could create trust, payment or documentation problem | Incomplete media approval |
| High | Could harm practitioner, community, site or legal posture | Unapproved profile, unsafe visit |
| Critical | Requires immediate pause | Sensitive data exposure, consent violation |

| Likelihood | Meaning |
|------------|---------|
| Rare | Unlikely under current controls |
| Possible | Could occur during active pilot |
| Likely | Expected unless actively managed |

High or Critical severity items must have an owner, next action and review date.

---

## Stop / pivot / continue criteria

### Continue

Continue when:

- consent records are complete;
- stewardship review is on schedule;
- practitioner burden remains acceptable;
- funding terms match mission and capacity;
- no unresolved High or Critical risks are open.

### Pivot

Pivot when:

- a sub-region lacks trusted access;
- compensation assumptions are wrong;
- advisors identify a better legal path;
- fieldwork reveals student programming is premature;
- archive tool choice does not support access rules.

### Stop or pause

Pause immediately when:

- a practitioner or steward withdraws consent for active material;
- restricted archive material is exposed;
- public language creates a false claim of partnership or endorsement;
- safety or liability terms are not ready for a planned visit;
- the founder cannot maintain governance, consent and archive records.

---

## Monitoring cadence

| Cadence | Review |
|---------|--------|
| Weekly during fieldwork | Open risks, consent gaps, practitioner burden |
| Monthly | Full risk register review |
| Quarterly | Archive access and public language audit |
| Before publication | Consent, steward review and claim verification |
| Before funding acceptance | Mission, deliverables and reporting obligations |
| Before app work | Governance readiness and technology gate |

---

## Incident response

1. Restrict affected material or activity immediately.
2. Record the incident in the risk register.
3. Notify the affected practitioner, steward or advisor when appropriate.
4. Identify whether the issue is consent, archive, language, safety or governance.
5. Decide repair, restriction, deletion, apology, compensation or pause.
6. Log the outcome and next review date.

---

## Required artifacts

Risk monitoring should connect to:

- `data/studium_risk_register.csv`;
- `data/studium_consent_schema.csv`;
- `data/studium_archive_schema.csv`;
- governance decision log;
- archive access log;
- public language review notes.

