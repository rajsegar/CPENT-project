# Module 07: Perimeter Defense Evasion Techniques

## In plain language

Perimeter testing evaluates whether boundary controls enforce the organization's
intended network and application policy. "Evasion" in an authorized assessment
means safely checking for gaps and inconsistent paths, then helping defenders
improve visibility and enforcement.

## Key ideas

| Control | Main purpose |
| --- | --- |
| Firewall | Permit or deny network flows according to policy |
| Web Application Firewall (WAF) | Inspect and control web requests |
| Intrusion Detection or Prevention System | Detect or block suspicious activity |
| Proxy or gateway | Mediate and log access between network zones |
| Network segmentation | Limit which systems can communicate |
| Rate control | Reduce abusive request volume |
| Egress control | Restrict outbound destinations and protocols |

## A safe assessment approach

1. Translate the approved network design into expected flows.
2. Identify each control point and its owner.
3. Establish a benign baseline request.
4. Change one protocol, path, or request property at a time.
5. Observe both enforcement and defender telemetry.
6. Stop when a rule gap is demonstrated.
7. Record the shortest verified path and recommend a durable control.

The aim is not to become invisible. The aim is to determine whether policy is
applied consistently and whether defenders receive enough reliable context to
respond.

## Common mistakes

- Treating "blocked" as proof that every alternate path is protected.
- Running high-volume tests without explicit approval.
- Testing only from one network location.
- Ignoring outbound controls.
- Reporting a bypass without confirming the intended policy.
- Failing to coordinate with the monitoring team.

## Defender view

Useful defenses include default-deny segmentation, consistent rules across
equivalent paths, authenticated proxies, egress filtering, tuned detection,
centralized time, contextual logging, and routine validation after changes.

## Quiz

1. Why must expected network policy be known before testing?
2. What is the difference between detection and prevention?
3. Why should one property be changed at a time?
4. What does egress filtering control?
5. Is a quiet alert stream proof that testing was invisible?

## Answer key

1. Without intended policy, a tester cannot tell whether an allowed or blocked
   flow represents correct behavior.
2. Detection records or alerts on activity; prevention actively blocks or
   changes it.
3. It isolates which difference caused a control or response to change.
4. Traffic leaving a network zone, including permitted destinations and
   protocols.
5. No. Logs may be delayed, unavailable to the reviewer, misconfigured, or not
   connected to an alert.

## Flashcards

**Q:** What is network segmentation?  
**A:** Separating zones and limiting traffic between them according to business need.

**Q:** What is a baseline request?  
**A:** A known, harmless request used for comparison.

**Q:** Why coordinate with defenders?  
**A:** To verify logging, alerts, timing, and deconfliction safely.

**Q:** What proves a control gap?  
**A:** Reproducible evidence that actual behavior differs from approved policy.

**Q:** When should testing stop?  
**A:** When the objective is proven, impact appears, or scope becomes uncertain.

## Safe practical exercise

In an isolated lab, draw two network zones and a gateway between them. Define
five expected allow or deny flows using harmless services. With the lab owner,
compare observed connectivity and logs against the table.

Do not use flooding, destructive payloads, persistence, or attempts to hide from
the lab owner. The deliverable is a policy matrix, an evidence table, and one
defensive improvement.

## Completion checklist

- [ ] I can explain the purpose of common boundary controls.
- [ ] I can compare an intended flow with observed behavior.
- [ ] I can validate both prevention and telemetry.
- [ ] I completed a lab policy matrix.
