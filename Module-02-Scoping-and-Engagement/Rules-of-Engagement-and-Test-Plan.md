# Module 02 — Rules of Engagement and Test Plan

## Status

Completed

## Module

CPENT Module 02 — Penetration Testing Scoping and Engagement

## Tester

RedteamAI

## Assessment Type

Authorized local lab planning exercise

## Target

```text
Target name: DVWA Local Lab
Target URL: http://localhost:4280
Environment: Local Kali Linux / Docker lab
Owner: RedteamAI
Permission source: Self-owned local training environment
Testing type: Grey-box local web application assessment
Timezone: Europe/London
```

## 1. Purpose of the Engagement

The purpose of this engagement is to practise professional penetration testing preparation before technical testing begins.

This exercise focuses on:

```text
Authorization
Scope definition
Rules of Engagement
Allowed and prohibited actions
Testing window
Stop conditions
Evidence handling
Cleanup planning
Reporting deliverables
```

The goal is not to exploit the target yet. The goal is to create a clear and safe test plan that another beginner could follow without guessing.

## 2. Authorization

This assessment is authorized because the target is a self-owned local training lab.

DVWA is intentionally vulnerable and is being used only for private cybersecurity learning.

No public websites, real company systems, third-party services, or unrelated network devices are included in this assessment.

## 3. Scope

### In Scope

```text
DVWA local web application
URL: http://localhost:4280
Local browser access
Local Burp Suite proxy configuration
Manual observation
Evidence screenshots
Documentation and reporting
```

### Out of Scope

```text
Public websites
Real company systems
Home router
Other devices on the network
Other local services not related to DVWA
Internet-facing systems
Cloud systems
Social engineering
Denial of Service testing
Malware
Persistence
Real credential attacks
Testing without authorization
```

## 4. Rules of Engagement

### Allowed Actions

```text
Access DVWA through the local browser
Use Burp Suite for observing local HTTP traffic
Take screenshots for evidence
Write notes
Create a test plan
Document scope and boundaries
Record assumptions, constraints, and stop conditions
```

### Prohibited Actions

```text
Do not test public websites
Do not test real company systems
Do not attack the home router
Do not test other devices on the network
Do not perform Denial of Service
Do not perform destructive testing
Do not use malware
Do not create persistence
Do not expose DVWA to the internet
Do not store real credentials in DVWA
```

## 5. Testing Window

```text
Testing date: 14 July 2026
Testing start time: Study session
Testing end time: Within 2 hours
Timezone: Europe/London
Maximum duration: 2 hours
```

## 6. Assumptions

```text
DVWA is running locally.
The tester owns the local lab environment.
The target is intentionally vulnerable.
The lab is not exposed to the internet.
No real user data is stored in the lab.
```

## 7. Constraints

```text
Testing is limited to the local DVWA application.
Testing time is limited to the agreed study window.
Only safe planning and observation are allowed in this module.
No exploitation is required for Module 02.
No testing may continue if scope becomes unclear.
```

## 8. Stop Conditions

Testing must stop immediately if:

```text
The target becomes unstable.
Docker or Kali becomes unstable.
Testing reaches a system outside http://localhost:4280.
A public website is accidentally reached.
Unexpected sensitive data appears.
The tester is unsure whether an action is allowed.
```

## 9. Evidence Handling

Evidence should include:

```text
Date
Time
Timezone
Target URL
Purpose of screenshot
Short explanation
Sanitized notes
```

Evidence must not include:

```text
Real passwords
Private tokens
Personal data
Client data
Unrelated system information
Sensitive screenshots
```

## 10. Cleanup Plan

After the exercise:

```text
Stop the DVWA container if it is no longer needed.
Close Burp Suite and browser sessions.
Save screenshots in the private evidence folder.
Commit only sanitized notes to GitHub.
Do not upload sensitive evidence to a public repository.
```

## 11. Deliverables

The deliverables for this Module 02 exercise are:

```text
Completed Rules of Engagement
Completed Test Plan
Evidence checklist
Module 02 reflection answers
Sanitized GitHub notes
```

## 12. Success Criteria

This exercise is successful if:

```text
The target is clearly defined.
In-scope and out-of-scope items are documented.
Allowed and prohibited actions are documented.
Stop conditions are documented.
Evidence handling is documented.
Cleanup plan is documented.
The tester understands what is allowed before testing begins.
```

## 13. Reflection

### What is scope?

Scope is the exact boundary of the penetration test. It defines what systems, applications, URLs, users, or areas are allowed and what must not be tested.

### What are Rules of Engagement?

Rules of Engagement are the operational rules the penetration tester must follow during the assessment. They define allowed tools, prohibited actions, testing windows, safety limits, stop conditions, evidence handling, and reporting requirements.

### Why is this important?

This is important because a professional penetration test must be legal, safe, controlled, and useful. Clear scope and rules protect the client, the tester, and the systems being tested.

## 14. Final Status

```text
Module 02 Rules of Engagement: Completed
Module 02 Test Plan: Completed
Evidence checklist: Completed
Ready for Module 02 quiz: Yes
```
