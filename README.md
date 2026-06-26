# CPENT Master Knowledge Base

A beginner-friendly, practical study repository for the EC-Council Certified
Penetration Testing Professional (CPENT) curriculum.

Student: RedteamAI  
Study goal: CPENT practical exam preparation before November 2026

> Use every technique only in an isolated lab or on a system for which you have
> explicit written authorization. A target being reachable does not make it
> authorized.

## Start here

1. Read the notes for one module.
2. Explain the key ideas in your own words.
3. Complete the quiz without looking at the answer key.
4. Review the flashcards.
5. Run the suggested exercise in an authorized lab.
6. Record evidence and write a short finding.

Use [Templates/Lab-Template.md](Templates/Lab-Template.md) before each lab and
[Reports/Finding-Report-Template.md](Reports/Finding-Report-Template.md) when a
lab produces a reportable issue.

## Core modules

This structure follows the current 14-module CPENT course outline published by
[EC-Council](https://www.eccouncil.org/train-certify/certified-penetration-testing-professional-cpent-north-america/).

| Module | Topic | Study material |
| --- | --- | --- |
| 01 | Introduction to Penetration Testing and Methodologies | [Open module](Module-01-Principles/) |
| 02 | Penetration Testing Scoping and Engagement | [Open module](Module-02-Scoping-and-Engagement/) |
| 03 | Open Source Intelligence (OSINT) | [Open module](Module-03-OSINT/) |
| 04 | Social Engineering Penetration Testing | [Open module](Module-04-Social-Engineering/) |
| 05 | Web Application Penetration Testing | [Open module](Module-05-Web-Application-Penetration-Testing/) |
| 06 | API and JSON Web Token Penetration Testing | [Open module](Module-06-API-and-JWT-Penetration-Testing/) |
| 07 | Perimeter Defense Evasion Techniques | [Open module](Module-07-Perimeter-Defense-Evasion/) |
| 08 | Windows Exploitation and Privilege Escalation | [Open module](Module-08-Windows-Exploitation-and-Privilege-Escalation/) |
| 09 | Active Directory Penetration Testing | [Open module](Module-09-Active-Directory-Penetration-Testing/) |
| 10 | Linux Exploitation and Privilege Escalation | [Open module](Module-10-Linux-Exploitation-and-Privilege-Escalation/) |
| 11 | Reverse Engineering, Fuzzing, and Binary Exploitation | [Open module](Module-11-Reverse-Engineering-Fuzzing-and-Binary-Exploitation/) |
| 12 | Lateral Movement and Pivoting | [Open module](Module-12-Lateral-Movement-and-Pivoting/) |
| 13 | IoT Penetration Testing | [Open module](Module-13-IoT-Penetration-Testing/) |
| 14 | Report Writing and Post-Testing Actions | [Open module](Module-14-Report-Writing-and-Post-Testing-Actions/) |

Course outlines change. Compare this repository with the material supplied for
your own course edition before using it as an exam checklist.

## Repository map

| Path | Purpose |
| --- | --- |
| Module-01 through Module-14 | Notes, quizzes, flashcards, and safe lab exercises |
| [Cheatsheets](Cheatsheets/) | Fast revision material |
| [Labs](Labs/) | Lab workspace guidance and evidence conventions |
| [Reports](Reports/) | Finding and full-report templates |
| [Templates](Templates/) | Reusable note, quiz, flashcard, and lab templates |
| [AGENTS.md](AGENTS.md) | Rules for AI assistants contributing to this repository |

## Suggested weekly routine

| Day | Activity |
| --- | --- |
| Monday | Learn one topic and rewrite the main idea in plain language |
| Tuesday | Review flashcards and repeat the quiz |
| Wednesday | Complete a small authorized lab |
| Thursday | Repeat the lab from memory and improve the notes |
| Friday | Write one finding with evidence and remediation |
| Saturday | Complete a larger lab or practice machine |
| Sunday | Review weak areas and plan the next week |

## Safe practice platforms

- PortSwigger Web Security Academy
- OWASP Juice Shop or WebGoat in a local lab
- Metasploitable or another intentionally vulnerable local VM
- TryHackMe or Hack The Box content covered by your account and lab terms
- A private Active Directory lab that you own and can restore

Never substitute a random public IP address, website, wireless network, or
cloud tenant for an authorized lab.

## Progress tracking

Copy the checklist below into your own study log:

- [ ] I can explain the module without reading the notes.
- [ ] I scored at least 80% on the quiz.
- [ ] I reviewed every flashcard.
- [ ] I completed an authorized lab.
- [ ] I saved useful evidence.
- [ ] I wrote or improved a finding.
- [ ] I recorded what I need to revisit.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Keep examples synthetic, redact secrets,
and prefer simple explanations before advanced detail.
