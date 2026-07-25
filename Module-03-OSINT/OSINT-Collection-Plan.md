# Module 03 — OSINT Collection Plan Lab

## Status

**Status:** In progress  
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

Complete or review the examples below.

| Type | Example |
| --- | --- |
| Fact | A fictional job advertisement states that Acme Cyber Labs is seeking an engineer with PostgreSQL experience. |
| Inference | Acme Cyber Labs may use PostgreSQL somewhere in its environment. |
| Unknown | The advertisement does not prove which system uses PostgreSQL, which version is installed, or whether it is Internet-facing. |
| Fact | A fictional certificate record contains `portal.acme-lab.example`. |
| Inference | The hostname may have been associated with a public portal. |
| Unknown | Current ownership, availability, security status, and authorization to test remain unconfirmed. |

### Student example

| Type | Your example |
| --- | --- |
| Fact | [Write one evidence-supported fact] |
| Inference | [Write one careful interpretation] |
| Unknown | [Write what the evidence does not prove] |

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

For every important observation, record:

```text
Observation:
Fictional asset:
Source type:
Collection date:
Collection time:
Timezone: Europe/London
Collection mode: Passive
Confidence: High / Medium / Low
Reliability limitation:
Possible business impact:
Next authorized validation step:
```

## 10. Evidence Screenshots

Capture and keep the following screenshots in your private evidence folder:

- [ ] Screenshot 1 — This file open in GitHub or your editor.
- [ ] Screenshot 2 — Fact, Inference, and Unknown table.
- [ ] Screenshot 3 — Attack-Surface Map.
- [ ] Screenshot 4 — Final completion checklist.

Do not upload screenshots containing real personal data, credentials, tokens, private email addresses, or unrelated system information.

## 11. Reflection

Answer in your own words.

### What is the difference between data and intelligence?

[Write your answer]

### What is the difference between passive and active collection?

[Write your answer]

### Why is a discovered asset not automatically in scope?

[Write your answer]

### Why must fact and inference be separated?

[Write your answer]

### What did you learn from this lab?

[Write your answer]

## 12. Completion Checklist

- [ ] I created three intelligence questions.
- [ ] I identified two public source types for each question.
- [ ] I explained source reliability and limitations.
- [ ] I separated passive and active activities.
- [ ] I documented a data-minimization rule.
- [ ] I separated facts, inferences, and unknowns.
- [ ] I reviewed the simple attack-surface map.
- [ ] I completed the evidence record fields.
- [ ] I answered the reflection questions in my own words.
- [ ] I captured sanitized screenshots.
- [ ] I did not investigate a real person or organization.

## 13. Final Result

```text
Module 03 practical lab: [IN PROGRESS / COMPLETED]
Evidence screenshots: [PENDING / SUBMITTED]
Ready for final quiz: [NO / YES]
```
