# CPENT 20-Week Study Plan

## Target

| Item | Plan |
| --- | --- |
| Plan starts | 28 June 2026 |
| Provisional exam date | 15 November 2026 |
| Time available | 140 days, or 20 weeks |
| Weekly study target | 14-18 hours |
| Main objective | Be ready for the practical exam and report submission |

The official CPENT exam is practical and can be taken as one 24-hour session or
two 12-hour sessions. A penetration test report must be submitted within seven
days of the final session. Confirm the current requirements in the
[official CPENT exam details](https://www.eccouncil.org/train-certify/certified-penetration-testing-professional-cpent-north-america/)
when booking.

## The rule that makes this plan work

Spend approximately:

- 25% of study time reading, reviewing, and making flashcards.
- 60% completing authorized hands-on labs.
- 15% organizing evidence and writing reports.

Do not count passive video watching as practical time. Repeat important labs
without step-by-step guidance.

## Weekly rhythm

Adjust the clock times around work and family, but keep the purpose of each day.

| Day | Activity | Time |
| --- | --- | ---: |
| Monday | Beginner notes, key terms, and flashcards | 1.5 hours |
| Tuesday | Guided authorized lab | 2 hours |
| Wednesday | Second lab or deeper investigation | 2 hours |
| Thursday | Repeat the main task without notes | 2 hours |
| Friday | Quiz, evidence review, and one short finding | 1.5 hours |
| Saturday | Integrated lab or practice machine | 4-6 hours |
| Sunday | Review mistakes, update notes, and rest | 1-2 hours |

Minimum target: 14 hours. Strong target: 16-18 hours. Take a lighter evening
when concentration becomes poor; exhausted practice teaches sloppy habits.

## Day 0: Sunday, 28 June

- [ ] Read the repository [README](README.md).
- [ ] Create a private study log using the [lab template](Templates/Lab-Template.md).
- [ ] Confirm access to legal training labs.
- [ ] Record a baseline quiz score for Module 1.
- [ ] Reserve weekly study blocks in the calendar.
- [ ] Check the intended exam-voucher expiry and booking process.

## Weeks 1-4: Engagement foundations

### Week 1: 29 June-5 July

**Focus:** [Module 01 - Introduction and Methodologies](Module-01-Principles/README.md)

- Explain scanning versus penetration testing.
- Learn the main assessment phases and evidence habits.
- Complete the Module 1 scope lab.
- Write a one-page explanation of authorization and business impact.
- Score at least 80% on the quiz.

**Deliverable:** One completed lab record and one short finding.

### Week 2: 6-12 July

**Focus:** [Module 02 - Scoping and Engagement](Module-02-Scoping-and-Engagement/README.md)

- Draft rules of engagement for one local vulnerable VM.
- Define targets, time zone, allowed actions, stop conditions, and cleanup.
- Practise identifying ambiguous scope statements.
- Rewrite the engagement so another student can follow it without guessing.

**Deliverable:** Completed rules of engagement and test plan.

### Week 3: 13-19 July

**Focus:** [Module 03 - OSINT](Module-03-OSINT/README.md)

- Separate passive collection from active interaction.
- Practise source reliability, corroboration, and confidence ratings.
- Use only a fictional organization for the repository exercise.
- Build a small attack-surface table from authorized lab information.

**Deliverable:** An evidence-based OSINT summary with facts and inferences
clearly separated.

### Week 4: 20-26 July

**Focus:** [Module 04 - Social Engineering](Module-04-Social-Engineering/README.md)

- Learn authorization, privacy, deconfliction, and stop conditions.
- Design a tabletop simulation that collects no real credentials.
- Review the exercise from participant, legal, and incident-response viewpoints.
- Do not contact real people.

**Gate 1:** By 26 July, explain Modules 1-4 without notes, score at least 80% on
their quizzes, and produce a safe engagement plan.

## Weeks 5-8: Web, API, and perimeter testing

### Week 5: 27 July-2 August

**Focus:** [Module 05 - Web Applications](Module-05-Web-Application-Penetration-Testing/README.md)

- Map pages, roles, inputs, sessions, and sensitive objects.
- Complete beginner authentication and authorization labs.
- Use OWASP Juice Shop, WebGoat, or PortSwigger Academy only.
- Manually verify results instead of copying scanner output.

**Deliverable:** Application map and one evidence-backed finding.

### Week 6: 3-9 August

**Focus:** Web testing continued

- Practise access control, session handling, input handling, and business logic.
- Repeat two previous labs without walkthroughs.
- Redact tokens and cookies from every screenshot.
- Write remediation that addresses the root cause.

**Deliverable:** Two additional findings and a short executive summary.

### Week 7: 10-16 August

**Focus:** [Module 06 - API and JWT](Module-06-API-and-JWT-Penetration-Testing/README.md)

- Inventory methods, endpoints, objects, roles, and expected responses.
- Compare two authorized lab users with different object ownership.
- Learn JWT structure, signature purpose, expiry, issuer, and audience.
- Never commit a usable bearer token.

**Deliverable:** A two-user authorization matrix and one API finding.

### Week 8: 17-23 August

**Focus:** [Module 07 - Perimeter Defense](Module-07-Perimeter-Defense-Evasion/README.md)

- Draw network zones, allowed flows, and control points.
- Compare expected firewall or gateway policy with observed lab behavior.
- Verify both enforcement and logging.
- Avoid flooding, destructive payloads, and stealth exercises.

**Deliverable:** Network-flow matrix and defensive telemetry notes.

## Weeks 9-13: Systems, identity, binaries, and pivoting

### Week 9: 24-30 August

**Focus:** [Module 08 - Windows Privilege Escalation](Module-08-Windows-Exploitation-and-Privilege-Escalation/README.md)

- Understand tokens, integrity, permissions, services, and scheduled tasks.
- Use a snapshot of an intentionally vulnerable Windows VM.
- Connect a writable object to the privileged component that trusts it.
- Restore the VM and verify normal operation.

**Gate 2:** By 30 August, complete a four-hour web/API/perimeter mini-assessment
and deliver a report with at least two verified findings.

### Week 10: 31 August-6 September

**Focus:** [Module 09 - Active Directory](Module-09-Active-Directory-Penetration-Testing/README.md)

- Learn domains, principals, groups, policies, Kerberos, and trusts.
- Build a small private AD lab diagram.
- Trace one candidate permission path.
- Label theoretical relationships separately from verified impact.

**Deliverable:** AD relationship diagram and an evidence checklist for each
path step.

### Week 11: 7-13 September

**Focus:** [Module 10 - Linux Privilege Escalation](Module-10-Linux-Exploitation-and-Privilege-Escalation/README.md)

- Understand users, groups, sudo, capabilities, services, and scheduled tasks.
- Use an intentionally vulnerable Linux VM.
- Connect a controllable object to a privileged consumer.
- Repeat the lab from a fresh snapshot without a walkthrough.

**Deliverable:** One verified lab finding with complete cleanup notes.

### Week 12: 14-20 September

**Focus:** [Module 11 - Reverse Engineering and Fuzzing](Module-11-Reverse-Engineering-Fuzzing-and-Binary-Exploitation/README.md)

- Distinguish static analysis, dynamic analysis, fuzzing, and exploitation.
- Work only with a toy or course-provided binary in a disposable VM.
- Record hashes and minimize one reproducible test case.
- Explain why a crash alone does not prove critical impact.

**Deliverable:** Crash-triage record and code-level remediation notes.

### Week 13: 21-27 September

**Focus:** [Module 12 - Lateral Movement and Pivoting](Module-12-Lateral-Movement-and-Pivoting/README.md)

- Distinguish reachability, pivoting, authentication, and lateral movement.
- Draw one approved multi-hop lab path.
- Demonstrate only a narrow route to the assigned destination.
- Remove every temporary route, listener, and file.

**Gate 3:** By 27 September, complete a six-hour Windows, AD, Linux, and
pivoting lab. Produce a timeline showing the host, identity, action, and
evidence for every important step.

## Weeks 14-16: IoT, reporting, and integration

### Week 14: 28 September-4 October

**Focus:** [Module 13 - IoT](Module-13-IoT-Penetration-Testing/README.md)

- Map device, firmware, app, cloud, network, and update surfaces.
- Practise static review on an approved firmware image or emulator.
- Record recovery and safety risks before testing.
- Do not publish extracted secrets or connect a lab device to production.

**Deliverable:** IoT system diagram and firmware-analysis summary.

### Week 15: 5-11 October

**Focus:** [Module 14 - Reporting and Post-Testing](Module-14-Report-Writing-and-Post-Testing-Actions/README.md)

- Turn raw evidence into precise findings.
- Separate observation, verified impact, possible impact, and limitation.
- Write technical and executive sections for different readers.
- Practise severity reasoning, root-cause remediation, and retesting.

**Deliverable:** One complete report using the
[full report template](Reports/Penetration-Test-Report-Template.md).

### Week 16: 12-18 October

**Focus:** First integrated assessment

- Run a six-to-eight-hour authorized lab covering web, API, system, and pivoting.
- Work from a written scope and keep a live evidence index.
- Stop using walkthroughs.
- Submit your practice report within 48 hours.

**Gate 4 - booking decision:** Continue with the November exam only if you can:

- Complete most assigned objectives without step-by-step help.
- Recover when the first technique fails.
- Explain every command or tool result you rely on.
- Keep organized evidence while under time pressure.
- Produce a clear report within 48 hours.

If several items are missing, moving the exam is a sensible professional
decision, not a failure.

## Weeks 17-20: Timed preparation

### Week 17: 19-25 October

**Focus:** Repair the weakest three areas

- Review Gate 4 results.
- Choose only three priority weaknesses.
- Complete focused labs and repeat each one from a clean state.
- Build short decision checklists rather than copying long command lists.

**Deliverable:** A one-page plan for each weak area.

### Week 18: 26 October-1 November

**Focus:** First 12-hour mock assessment

- Prepare sleep, food, breaks, scope, evidence folders, and note structure.
- Complete a 12-hour authorized practice assessment.
- Record unsuccessful paths as well as successful ones.
- Submit a complete report within 36 hours.
- Aim for at least 75% of your defined objectives.

**Deliverable:** Mock report 1 and an honest lessons-learned list.

### Week 19: 2-8 November

**Focus:** Final mock and readiness confirmation

- Fix the problems found in mock 1.
- Complete a second timed assessment using different lab targets.
- Submit the report within 24 hours.
- Aim for at least 80% of your defined objectives.
- Confirm exam booking, identity documents, proctoring, equipment, and backups.

**Readiness rule:** Sit the exam only if your process is repeatable and your
report is clear. A single lucky lab result is not readiness.

### Week 20: 9-15 November

**Focus:** Taper and exam

- Monday-Tuesday: Review scope, methodology, pivots, evidence, and reporting.
- Wednesday: Complete only short confidence-building exercises.
- Thursday: Check the system, exam access, files, power, network, and clock.
- Friday onward: Protect sleep and avoid learning large new topics.
- Exam day: Work methodically, take breaks, save evidence immediately, and
  leave enough energy for the report.

Do not attempt a long practice machine during the final 48 hours.

## Weekly scorecard

Copy this table into a private study log each Sunday.

| Measure | Target | Result |
| --- | ---: | --- |
| Focused study hours | 14-18 | TODO |
| Hands-on hours | 8 or more | TODO |
| Quiz score | 80% or more | TODO |
| Labs repeated without guidance | 1 or more | TODO |
| Findings written | 1 or more | TODO |
| Cleanup verified | Every lab | TODO |
| Weakest skill for next week | One named skill | TODO |

## Exam readiness checklist

- [ ] I can read a scope and immediately identify boundaries and stop conditions.
- [ ] I can enumerate before choosing an exploitation path.
- [ ] I can test web and API authorization with multiple roles.
- [ ] I can reason about Windows, AD, and Linux privilege paths.
- [ ] I can map and clean up a narrow pivot.
- [ ] I can triage a toy binary crash without overstating impact.
- [ ] I can analyze an approved IoT image safely.
- [ ] I keep timestamps, targets, identities, and evidence organized.
- [ ] I can explain business impact and root-cause remediation.
- [ ] I completed two timed mock assessments.
- [ ] I can produce a professional report while tired.
- [ ] I have checked the current official exam and report requirements.

## If a week is missed

Do not squeeze two full weeks into one. Drop optional reading, preserve the core
lab and reporting work, and use Week 17 for recovery. If two or more major
weeks remain incomplete at Gate 4, choose a later exam date.
