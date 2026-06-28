# Module 01 — Principles and Objectives of Penetration Testing

> Only test systems that you own or have explicit written permission to test.
> If authorization or scope is unclear, stop and ask before continuing.

## 1. What is Penetration Testing?

Penetration testing is an authorized security assessment in which a tester
simulates realistic attacker behaviour to find and safely prove security
weaknesses.

The goal is not simply to produce a list of vulnerabilities. A professional
test should:

- Validate whether a weakness can be exploited.
- Demonstrate the minimum impact needed.
- Collect reliable evidence.
- Explain the technical and business risk.
- Recommend practical remediation.
- Restore the environment when testing is complete.

**Simple meaning:**

> Penetration testing is an authorized simulated attack used to find, prove,
> document, and help fix security risks.

## 2. Penetration Testing vs. Vulnerability Scanning

A vulnerability scanner automatically looks for known weaknesses. It can cover
many systems quickly, but its results may contain false positives or lack
business context.

A penetration tester uses human reasoning to validate selected weaknesses,
understand how they might connect, and determine their real impact.

| Vulnerability scanning | Penetration testing |
| --- | --- |
| Finds possible known weaknesses | Validates whether selected weaknesses are real |
| Mostly automated | Combines tools with human judgement |
| Produces leads for investigation | Produces verified evidence and impact |
| May not understand business context | Connects technical issues to business risk |
| Usually stops at detection | Includes validation, reporting, and remediation advice |

**Simple difference:**

> Vulnerability scanning finds possible weaknesses. Penetration testing safely
> proves exploitability and impact.

## 3. Why Written Authorization Is Important

Written authorization gives the tester legal and organizational permission to
perform the agreed assessment. It protects both the client and the tester.

Authorization should clearly define:

- The systems, applications, people, and locations in scope.
- Items that must not be tested.
- The permitted testing dates and time zone.
- Allowed and prohibited techniques.
- Rules of engagement.
- Evidence-handling requirements.
- Emergency contacts and stop conditions.
- Cleanup and reporting responsibilities.

Good intentions are not permission. A reachable system is not automatically an
authorized system.

**Important reminder:**

> No written authorization means no testing.

## 4. The Three Main Phases

A beginner-friendly penetration testing process can be divided into three main
phases:

1. Pre-Attack
2. Attack
3. Post-Attack

The exact names may vary between methodologies, but the underlying flow remains
similar: prepare, test, and report.

## 5. Pre-Attack Phase

The Pre-Attack phase prepares the assessment and helps the tester understand
the target before attempting exploitation.

Typical activities include:

- Confirming written authorization.
- Defining scope and objectives.
- Agreeing on rules of engagement.
- Passive and active reconnaissance.
- Domain Name System (DNS) and registration research.
- Host and port discovery.
- Service enumeration.
- Operating system identification.
- Planning evidence collection and cleanup.

Reconnaissance, scanning, and enumeration can still affect systems or trigger
security alerts. Active work must remain inside the approved scope.

**Simple meaning:**

> Pre-Attack means preparing for the assessment and understanding the target
> before exploitation.

## 6. Attack Phase

During the Attack phase, the tester safely validates identified weaknesses in
accordance with the rules of engagement.

Permitted activities may include:

- Controlled exploitation.
- Gaining access to an approved lab target.
- Privilege escalation.
- Credential testing.
- Web application or database testing.
- Lateral movement between approved systems.
- Controlled post-exploitation.
- Maintaining access only when explicitly authorized.

The tester should stop after collecting enough evidence to prove the agreed
impact. Unnecessary access creates risk without adding value.

**Simple meaning:**

> Attack means safely proving whether an identified weakness can be exploited.

## 7. Post-Attack Phase

The Post-Attack phase returns the environment to the agreed state and turns
technical evidence into useful actions.

Typical activities include:

- Saving relevant requests, responses, logs, and screenshots.
- Recording the affected asset and time of each result.
- Removing test files, accounts, listeners, and other artifacts.
- Restoring approved configuration changes.
- Confirming that systems still operate normally.
- Writing clear findings.
- Explaining technical and business impact.
- Recommending root-cause remediation.
- Retesting fixes when requested.

Evidence should be accurate and sufficient, but it should not expose reusable
credentials, tokens, personal data, or unrelated sensitive information.

**Simple meaning:**

> Post-Attack means cleaning up, reporting the evidence, and helping the
> organization fix the issue.

## 8. EC-Council LPT Methodology

The EC-Council Licensed Penetration Tester (LPT) methodology provides a
structured process for a professional penetration test.

The 11 steps are:

1. Planning and Scoping
2. Reconnaissance and Information Gathering
3. Vulnerability Assessment
4. Gaining Access
5. Privilege Escalation
6. Lateral Movement
7. Maintaining Access
8. Data Exfiltration
9. Clearing Tracks
10. Documentation and Reporting
11. Remediation Testing

In an authorized assessment, data exfiltration should use the smallest safe
proof permitted by the rules of engagement. Clearing tracks means removing
approved testing artifacts during cleanup; it does not mean concealing
unauthorized activity or destroying organizational logs.

**Simple meaning:**

> The LPT methodology is EC-Council's structured process for planning,
> performing, documenting, and closing a penetration test.

## 9. MITRE ATT&CK

MITRE ATT&CK is a knowledge base of adversary tactics and techniques observed
in the real world. It helps testers and defenders use a shared language when
describing behaviour.

Examples of Enterprise ATT&CK tactics include:

1. Reconnaissance
2. Resource Development
3. Initial Access
4. Execution
5. Persistence
6. Privilege Escalation
7. Defense Evasion
8. Credential Access
9. Discovery
10. Lateral Movement
11. Collection
12. Command and Control
13. Exfiltration
14. Impact

ATT&CK is not a step-by-step penetration testing methodology. It is a reference
for understanding, mapping, detecting, and discussing adversary behaviour.

**Simple meaning:**

> MITRE ATT&CK is a map of how real attackers behave.

## 10. Compliance-Driven Penetration Testing

Some organizations perform penetration tests to help meet legal, regulatory,
contractual, or industry requirements.

| Example | Main area |
| --- | --- |
| PCI DSS | Payment card data |
| GDPR | Personal data protected by European data-protection law |
| HIPAA | Protected healthcare information in the United States |
| SOC 2 | Controls at service organizations |
| ISO/IEC 27001 | Information security management systems |
| SOX | Financial reporting controls in the United States |
| FedRAMP | Security requirements for United States federal cloud services |

Compliance does not automatically prove that a system is secure. The exact test
scope and evidence requirements depend on the applicable standard, organization,
and assessor.

**Simple meaning:**

> A compliance-driven penetration test helps demonstrate that required security
> controls have been assessed.

## 11. AI-Driven Penetration Testing

Artificial intelligence (AI) can support a penetration tester by helping with:

- Summarizing authorized scan results.
- Explaining tool output.
- Drafting scripts and checklists.
- Finding patterns in large data sets.
- Organizing evidence.
- Improving the clarity of reports.
- Translating technical findings for different audiences.

AI output must always be reviewed by a human tester. AI can produce false
information, unsafe suggestions, weak code, or conclusions that ignore scope
and business context.

Never provide an AI system with real credentials, customer information, private
evidence, or sensitive target data unless the engagement explicitly permits the
chosen service and data handling.

**Important reminder:**

> AI can assist the tester, but it cannot replace human authorization,
> judgement, verification, or responsibility.

## 12. Module 01 Key Takeaways

- [ ] Penetration testing is an authorized simulated attack.
- [ ] Vulnerability scanning finds possible weaknesses.
- [ ] Penetration testing validates exploitability and impact.
- [ ] Written authorization and scope are required before testing.
- [ ] The three main phases are Pre-Attack, Attack, and Post-Attack.
- [ ] The LPT methodology provides a structured testing process.
- [ ] MITRE ATT&CK maps adversary behaviour; it is not a testing checklist.
- [ ] Compliance requirements can influence scope and evidence.
- [ ] AI can assist a tester, but every result requires human verification.
- [ ] Cleanup, reporting, and remediation are part of the assessment.

## 13. My Own Summary

Write a three-to-five-sentence explanation in your own words:

> How is penetration testing different from vulnerability scanning, and why
> are authorization, evidence, and reporting important?
