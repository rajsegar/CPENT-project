# Module 03 — OSINT Collection Plan Lab

## Status

**Status:** Completed  
**Student:** RedteamAI  
**Module:** CPENT Module 03 — Open Source Intelligence  
**Completion date:** 26 July 2026  
**Assessment type:** Authorized fictional-company planning exercise  
**Collection mode:** Passive planning only  
**Active scanning:** Not permitted  
**Timezone:** Europe/London

## 1. Fictional Target

```text
Company: Acme Cyber Labs
Domain: acme-lab.example
Environment: Fictional training environment
Owner: Fictional lab owner
Authorization: Training exercise only
```

> No real person, company, domain, email address, or IP address was investigated for this lab.

## 2. Lab Objective

Create a structured OSINT collection plan that demonstrates how to:

- define intelligence questions;
- choose suitable public source types;
- evaluate source reliability;
- distinguish passive from active collection;
- separate fact, inference, and unknown information;
- apply data minimization;
- assign confidence;
- record evidence safely; and
- build a simple attack-surface map.

## 3. Intelligence Questions

### Question 1 — Domains and Subdomains

**Question:** Which public domains and subdomains may be associated with Acme Cyber Labs?

**Source types:**

1. Public DNS or certificate records
2. Official fictional website or published document

**Reliability note:** DNS and certificate records may be historical, stale, shared, or linked to third-party infrastructure. Ownership and scope must still be confirmed.

### Question 2 — Technology Clues

**Question:** Which technologies may be publicly associated with Acme Cyber Labs?

**Source types:**

1. Fictional public job advertisement
2. Fictional technical documentation or code repository

**Reliability note:** A technology mentioned in a job advertisement or document does not prove that it is currently deployed, Internet-facing, or vulnerable.

### Question 3 — Security-Relevant Business Roles

**Question:** Which public business roles may be relevant to the organization’s security exposure?

**Source types:**

1. Fictional official staff or leadership page
2. Fictional professional-role description

**Reliability note:** Only role-related information should be collected. Unrelated personal data must not be retained.

## 4. Passive and Active Boundary

### Passive activities allowed

- Review fictional official pages and public documents.
- Review fictional third-party DNS and certificate records.
- Review fictional job advertisements and archived pages.
- Record source type, date, reliability, and confidence.

### Active activities prohibited

- Port scanning or live-host discovery.
- Banner grabbing.
- DNS zone-transfer requests.
- Login, password-reset, or account-enumeration attempts.
- Direct contact with employees.
- Testing any real domain, hostname, email address, or IP address.

## 5. Data-Minimization Rule

Only information directly required to answer the three approved intelligence questions will be collected. Unrelated personal information, credentials, tokens, private addresses, family information, personal photographs, private accounts, and unrelated sensitive information will not be retained or reported.

## 6. Fact, Inference, and Unknown

| Type | Example |
| --- | --- |
| Fact | A fictional public job advertisement states that Acme Cyber Labs is looking for an engineer with AWS experience. |
| Inference | Acme Cyber Labs may use AWS or another cloud-based environment. |
| Unknown | The advertisement does not prove that AWS is used in production, how it is configured, or whether any AWS system is vulnerable. |

## 7. Source Reliability

| Source type | Suggested reliability | Important limitation |
| --- | --- | --- |
| Official company page | High | The page may contain outdated content |
| Official public document | High to medium | The document may be old |
| Public DNS record | Medium to high | It may point to shared or third-party infrastructure |
| Certificate record | Medium | It may be historical or stale |
| Job advertisement | Medium | It shows desired skills, not confirmed deployment |
| Archived page | Medium to low | It proves historical visibility, not current operation |
| Search-result snippet | Low | The full source and context must be checked |

## 8. Simple Attack-Surface Map

| Asset or clue | Exposure | Source type | Confidence | Limitation | Next authorized step |
| --- | --- | --- | --- | --- | --- |
| `portal.acme-lab.example` | Possible web portal | Fictional certificate record | Medium | Ownership and current use unconfirmed | Confirm ownership and written scope |
| `mail.acme-lab.example` | Possible mail service | Fictional DNS record | Medium | May use third-party infrastructure | Confirm provider and tenant boundary |
| AWS | Technology clue | Fictional job advertisement | Medium | Deployment and configuration unknown | Corroborate with an independent authorized source |
| Security Administrator role | Privileged business role | Fictional staff page | High | No account details collected | Record role only; do not contact person |

## 9. Evidence Record

```text
Observation:
A fictional public job advertisement states that Acme Cyber Labs is looking for an engineer with AWS experience.

Fictional asset:
Acme Cyber Labs technology environment

Source type:
Fictional public job advertisement

Collection date:
26 July 2026

Timezone:
Europe/London

Collection mode:
Passive

Confidence:
Medium

Reliability limitation:
A job advertisement shows a desired skill, but it does not prove that AWS is currently deployed, used in production, or configured in a particular way.

Possible business impact:
Public technology clues may help an attacker form hypotheses about the organization’s digital footprint and likely cloud environment.

Next authorized validation step:
Corroborate the technology clue with an independent authorized source. Confirm ownership and written scope before active validation.
```

## 10. Reflection

### What is the difference between data and intelligence?

Data consists of raw, unorganized facts, numbers, observations, or symbols. Intelligence is data that has been processed, analyzed, placed into context, and connected to a defined question so that it supports decisions.

### What is the difference between passive and active collection?

Passive collection gathers information from public or third-party sources without directly probing the target. Active collection sends traffic or requests directly to the target and may be logged, trigger alerts, or affect the system, so it requires explicit authorization.

### Why is a discovered asset not automatically in scope?

A discovered asset may belong to a third party, cloud provider, shared infrastructure, or an unrelated organization. Ownership, scope boundaries, and written authorization must be confirmed before active testing.

### Why must fact and inference be separated?

Separating facts from inferences keeps the report credible and transparent. A fact is directly supported by evidence, while an inference is an interpretation; separating them prevents assumptions from being presented as confirmed findings.

### What did you learn from this lab?

I learned about passive reconnaissance, digital footprinting, and safe OSINT tool utilization. I also learned to evaluate source reliability, distinguish facts from inferences, protect unrelated personal data, and confirm written scope before active testing.

## 11. Quiz Result

```text
Final quiz score: 21/25 — 84%
Status: Passed
Review completed:
- DNS zone transfers require explicit authorization.
- Corroboration means checking a claim against an independent source.
- A fact states exactly what the evidence says.
- Decommissioning unused or legacy Internet-facing assets reduces exposure.
```

## 12. Completion Checklist

- [x] I created three intelligence questions.
- [x] I identified two public source types for each question.
- [x] I explained source reliability and limitations.
- [x] I separated passive and active activities.
- [x] I documented a data-minimization rule.
- [x] I separated facts, inferences, and unknowns.
- [x] I reviewed the simple attack-surface map.
- [x] I completed the evidence record fields.
- [x] I answered the reflection questions in my own words.
- [x] I captured sanitized screenshots.
- [x] I did not investigate a real person or organization.

## 13. Final Result

```text
Module 03 practical lab: COMPLETED
Module 03 final quiz: PASSED — 21/25 (84%)
Evidence screenshots: SUBMITTED
Module 03 final completion: COMPLETED
Ready for Module 04: YES
```
