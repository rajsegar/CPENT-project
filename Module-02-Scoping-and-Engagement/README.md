# Module 02: Penetration Testing Scoping and Engagement

## Status

**Module status:** Completed  
**Completion date:** 14 July 2026  
**Closed-book review score:** 91/100  
**Practical lab:** Completed  
**Rules of Engagement:** Completed  
**Test plan:** Completed  
**Evidence:** Submitted by the student and recorded in the completion record  
**Next module:** Module 03 — OSINT

## In plain language

Scoping decides what may be tested, why it is being tested, when testing may
happen, and which actions are prohibited. It turns a vague request such as
"test our network" into a safe and measurable engagement.

## Study material

- [Rules of Engagement and Test Plan](Rules-of-Engagement-and-Test-Plan.md)
- [Module 02 Lab Completion Record](Lab-Completion-Record.md)
- [Module 02 Closed-Book Review](Closed-Book-Review.md)

## Key ideas

| Term | Beginner-friendly meaning |
| --- | --- |
| Scope | The assets, people, locations, and techniques included in the test |
| Rules of engagement | The operational rules the tester must follow |
| Assumption | Something believed to be true but not yet verified |
| Constraint | A limit such as time, access, safety, or unavailable systems |
| Success criterion | Evidence that shows the assessment objective was met |
| Stop condition | An event that requires testing to pause immediately |

## A simple engagement flow

1. Understand the business reason for the test.
2. Identify asset owners and decision-makers.
3. List in-scope and out-of-scope targets precisely.
4. Agree on permitted and prohibited techniques.
5. Define the test window, contacts, and escalation process.
6. Agree on evidence handling, reporting, and cleanup.
7. Resolve contradictions before testing begins.

An IP range alone is not a complete scope. Cloud resources, third-party
services, shared infrastructure, user accounts, physical locations, and
sensitive data may need separate approval.

## Common mistakes

- Starting reconnaissance before written authorization is complete.
- Treating an ambiguous hostname as permission to test every related system.
- Forgetting time zones in the testing window.
- Failing to define what happens if production becomes unstable.
- Assuming social engineering or denial of service is allowed.
- Failing to record test accounts and cleanup responsibilities.

## Defender and client view

The client needs to know what business process could be affected, how to reach
the tester, what evidence will be collected, and how urgent findings will be
communicated. Clear rules protect both the organization and the tester.

## Quiz

Try these before reading the answer key.

1. Why is a list of IP addresses not always a complete scope?
2. What is the difference between a constraint and a stop condition?
3. Who should confirm that a third-party hosted system may be tested?
4. What should a tester do when two scope documents disagree?
5. Name three items that belong in rules of engagement.

## Answer key

1. It may not explain ownership, shared services, data boundaries, techniques,
   or business systems behind those addresses.
2. A constraint limits planned work; a stop condition requires work to pause
   because a defined risk or event has occurred.
3. The relevant asset owner and authorized representatives must confirm it,
   including the third party when its terms or ownership require approval.
4. Pause and obtain written clarification before testing the disputed area.
5. Examples include testing windows, allowed techniques, prohibited actions,
   emergency contacts, evidence handling, and notification rules.

## Flashcards

**Q:** What comes before technical testing?  
**A:** Written authorization, agreed scope, and rules of engagement.

**Q:** What makes a scope measurable?  
**A:** Precise assets, objectives, boundaries, and success criteria.

**Q:** Is social engineering automatically included?  
**A:** No. It requires explicit approval and detailed boundaries.

**Q:** What should happen when ownership is uncertain?  
**A:** Treat the target as out of scope until ownership and permission are clear.

**Q:** Why record a testing time zone?  
**A:** It prevents confusion during monitoring, incident response, and evidence review.

## Safe practical exercise

The student completed a rules-of-engagement and test-plan exercise for a single
intentionally vulnerable local lab target. The exercise documented:

- One target address and owner.
- A two-hour window with time zone.
- Allowed reconnaissance and validation.
- Prohibited denial of service, persistence, and unrelated network access.
- An emergency stop condition.
- Evidence handling and cleanup.

No public or third-party systems were included.

## Completion checklist

- [x] I can turn a business objective into a precise test objective.
- [x] I can find ambiguity in a scope.
- [x] I know when to pause and ask for written clarification.
- [x] I completed the safe practical exercise.
- [x] I completed the Rules of Engagement document.
- [x] I completed the test plan.
- [x] I submitted evidence for the practical exercise.
- [x] I completed the closed-book review with at least 80%.
- [x] I can explain why third-party systems require separate authorization.
