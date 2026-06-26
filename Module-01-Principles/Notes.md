# Module 01 — Principles and Objectives of Penetration Testing

## 1. What is penetration testing?

Penetration testing is an authorized security assessment where a tester simulates real attacker behaviour to find weaknesses before criminals do.

The goal is not just to find vulnerabilities. The real goal is to prove risk, explain business impact, and help the organization fix the problem safely.

## 2. Penetration testing vs vulnerability scanning

A vulnerability scan mainly finds known weaknesses using automated tools.

A penetration test goes further. It validates whether the weakness can be exploited, whether it can be chained with other issues, and what real impact it could have.

Example:

A scanner may say:

> Apache version is outdated.

A penetration tester asks:

- Can I exploit this?
- Can I get access?
- Can I escalate privileges?
- Can I move to another system?
- Can sensitive business data be accessed?

## 3. Why authorization is important

Authorization is what separates a penetration tester from an attacker.

Before testing, you need written permission, agreed scope, timing, rules of engagement, and emergency contacts.

No authorization means the activity can become illegal, even if your intention is good.

## 4. Three penetration testing phases

### Pre-Attack

This is the planning and information-gathering stage.

Common activities:

- Define scope
- Understand goals
- Passive reconnaissance
- Active reconnaissance
- Port scanning
- Service enumeration
- OS fingerprinting

### Attack

This is where the tester attempts controlled exploitation.

Common activities:

- Exploitation
- Privilege escalation
- Credential attacks
- Web application testing
- Database testing
- Wireless testing
- Lateral movement
- Maintaining access only if allowed

### Post-Attack

This is the cleanup and reporting stage.

Common activities:

- Restore modified settings
- Remove test files
- Document evidence
- Explain impact
- Provide remediation
- Deliver final report

## 5. EC-Council LPT methodology — 11 steps

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

## 6. MITRE ATT&CK Enterprise tactics

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

## 7. Compliance-driven penetration testing

Some penetration tests are performed because a company must meet compliance requirements.

Important examples:

- PCI DSS: payment card data
- HIPAA: healthcare data
- GDPR: EU personal data
- SOX: financial reporting
- FedRAMP: US federal cloud
- SOC 2: service organization controls
- ISO/IEC 27001: information security management system

## 8. AI-driven penetration testing

AI can help with speed, automation, summarization, scripting, and pattern detection.

But AI still needs human oversight because it can produce false positives, miss context, or suggest unsafe actions.

## 9. Beginner explanation

A vulnerability scanner is like a checklist.

A penetration tester is like a security professional proving what an attacker could actually do with the weaknesses found.

## 10. Your summary

Write your own 3–5 sentence answer here:

> Why is penetration testing different from vulnerability scanning?

