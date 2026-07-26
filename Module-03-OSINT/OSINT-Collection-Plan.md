# Module 03 — OSINT Collection Plan Lab

## Status

**Status:** Practical answers completed — evidence screenshots pending  
**Student:** RedteamAI  
**Module:** CPENT Module 03 — Open Source Intelligence  
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

> Do not investigate a real person, company, domain, email address, or IP address for this lab.

## 2. Lab Objective

Create a structured OSINT collection plan that demonstrates how to:

- define intelligence questions;
- choose suitable public source types;
- evaluate source reliability;
- distinguish passive from active collection;
- separate fact, inference, and unknown information;
- apply data minimization;
- assign confidence; and
- record evidence safely.

## 3. Intelligence Questions

### Question 1 — Domains and Subdomains

**Intelligence question:**  
Which public domains and subdomains may be associated with Acme Cyber Labs?

**Public source type 1:** Public DNS or certificate records  
**Public source type 2:** Official fictional website or published document

**Reliability note:**  
DNS and certificate records may provide useful leads, but they may be historical, stale, shared, or associated with third-party infrastructure. Ownership and scope must still be confirmed.

### Question 2 — Technology Clues

**Intelligence question:**  
Which technologies may be publicly associated with Acme Cyber Labs?

**Public source type 1:** Fictional public job advertisement  
**Public source type 2:** Fictional technical documentation or code repository

**Reliability note:**  
A technology mentioned in a job advertisement or document does not prove that it is currently deployed, Internet-facing, or vulnerable.

### Question 3 — Security-Relevant Business Roles

**Intelligence question:**  
Which public business roles may be relevant to the organization’s security exposure?

**Public source type 1:** Fictional official staff or leadership page  
**Public source type 2:** Fictional professional-role description

**Reliability note:**  
Only role-related information should be collected. Personal-life information, home addresses, family details, private accounts, and unrelated personal data must not be retained.

## 4. Passive and Active Boundary

### Passive activities allowed for this planning exercise

- Review fictional official pages.
- Review fictional public documents.
- Review fictional third-party DNS information.
- Review fictional certificate records.
- Review fictional job advertisements.
- Review fictional archived pages.
- Record sources, dates, reliability, and confidence.

### Active activities prohibited

- Port scanning.
- Live-host discovery.
- Banner grabbing.
- DNS zone-transfer requests.
- Login attempts.
- Password-reset testing.
- Account enumeration.
- Direct contact with employees.
- Testing any real domain, hostname, email address, or IP address.

## 5. Data-Minimization Rule

Only information directly required to answer the three approved intelligence questions will be collected.

The following information must not be retained or reported:

- unrelated personal information;
- credentials or authentication tokens;
- private addresses;
- family information;
- personal photographs;
- private account details; and
- sensitive information unrelated to the assessment objective.

## 6. Fact, Inference, and Unknown Table

| Type | Example |
| --- | --- |
| Fact | A fictional job advertisement states that Acme Cyber Labs is seeking an engineer with PostgreSQL experience. |
| Inference | Acme Cyber Labs may use PostgreSQL somewhere in its environment. |
| Unknown | The advertisement does not prove which system uses PostgreSQL, which version is installed, or whether it is Internet-facing. |
| Fact | A fictional certificate record contains `portal.acme-lab.example`. |
| Inference | The hostname may have been associated with a public portal. |
| Unknown | Current ownership, availability, security status, and authorization to test remain unconfirmed. |

### Student example

| Type | Student answer |
| --- | --- |
| Fact | A fictional public job advertisement states that Acme Cyber Labs is looking for an engineer with AWS experience. |
| Inference | Acme Cyber Labs may use AWS or another cloud-based environment. |
| Unknown | The advertisement does not prove that AWS is used in production, how it is configured, or whether any AWS system is vulnerable. |

## 7. Source Reliability Table

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
| PostgreSQL | Technology clue | Fictional job advert | Low | Deployment and version unknown | Seek independent evidence |
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

Collection time:
Not applicable — fictional planning exercise completed through guided study

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
Corroborate the technology clue with an independent authorized source. Confirm ownership and written scope before any active validation.
```

## 10. Evidence Screenshots

Capture and keep the following screenshots in your private evidence folder:

- [ ] Screenshot 1 — This file open in GitHub or your editor.
- [ ] Screenshot 2 — Fact, Inference, and Unknown table.
- [ ] Screenshot 3 — Attack-Surface Map.
- [ ] Screenshot 4 — Final completion checklist.

Do not upload screenshots containing real personal data, credentials, tokens, private email addresses, or unrelated system information.

## 11. Reflection

### What is the difference between data and intelligence?

Data consists of raw, unorganized facts, numbers, observations, or symbols. Intelligence is data that has been processed, analyzed, placed into context, and connected to a defined question so that it tells a meaningful story and supports decisions.

### What is the difference between passive and active collection?

Passive collection gathers information from public or third-party sources without directly probing the target system. Active collection sends traffic or requests directly to the target and may be logged, trigger alerts, or affect the system, so it requires explicit authorization.

### Why is a discovered asset not automatically in scope?

A discovered asset may belong to a third party, cloud provider, shared infrastructure, or an unrelated organization. Formal ownership, scope boundaries, and written authorization must be confirmed before active testing.

### Why must fact and inference be separated?

Separating facts from inferences keeps the report credible and transparent for decision-makers. A fact is directly supported by evidence, while an inference is an interpretation; separating them prevents assumptions from being presented as confirmed findings.

### What did you learn from this lab?

I learned about passive reconnaissance, digital footprinting, and safe OSINT tool utilization. I also learned to evaluate source reliability, distinguish facts from inferences, protect unrelated personal data, and confirm written scope before active testing.

## 12. Quiz Result

```text
Final quiz score: 21/25 — 84%
Status: Completed
Review topics:
- DNS zone transfers require explicit authorization.
- Corroboration means checking a claim against an independent source.
- A fact states exactly what the evidence says.
- Defensive exposure reduction includes decommissioning unused or legacy Internet-facing assets.
```

## 13. Completion Checklist

- [x] I created three intelligence questions.
- [x] I identified two public source types for each question.
- [x] I explained source reliability and limitations.
- [x] I separated passive and active activities.
- [x] I documented a data-minimization rule.
- [x] I separated facts, inferences, and unknowns.
- [x] I reviewed the simple attack-surface map.
- [x] I completed the evidence record fields.
- [x] I answered the reflection questions in my own words.
- [ ] I captured sanitized screenshots.
- [x] I did not investigate a real person or organization.

## 14. Final Result

```text
Module 03 practical answers: COMPLETED
Module 03 final quiz: COMPLETED — 21/25 (84%)
Evidence screenshots: PENDING
Module 03 final completion: PENDING SCREENSHOT EVIDENCE
```
