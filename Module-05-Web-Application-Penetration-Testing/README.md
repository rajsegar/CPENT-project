# Module 05: Web Application Penetration Testing

## In plain language

Web application testing checks how a website handles identity, permissions,
input, sessions, data, and business rules. A useful test follows the
application's behavior instead of running a scanner and treating every alert as
proof.

## Key ideas

| Area | Beginner-friendly question |
| --- | --- |
| Attack surface | Which pages, parameters, files, APIs, and roles exist? |
| Authentication | Can the application reliably identify the user? |
| Authorization | May this user perform this action on this object? |
| Session management | Are login sessions created, protected, and ended safely? |
| Input handling | Does the application safely interpret untrusted data? |
| Business logic | Can a valid feature be used in an unintended harmful order? |
| Configuration | Are deployment settings, backups, and errors safely handled? |

## A simple testing workflow

1. Confirm the exact application, accounts, and test data in scope.
2. Map normal workflows for each approved role.
3. Record requests, responses, cookies, and state changes.
4. Change one variable at a time.
5. Verify suspicious behavior manually.
6. Demonstrate the smallest impact needed.
7. Save evidence, clean up test data, and explain remediation.

Start with normal behavior. If you do not understand how a feature is supposed
to work, you cannot confidently explain why an unusual response is a
vulnerability.

## Common mistakes

- Reporting a scanner alert without confirming it.
- Testing only the unauthenticated pages.
- Confusing authentication with authorization.
- Ignoring different user roles and object ownership.
- Changing several inputs at once and losing the cause of a result.
- Capturing session tokens in screenshots or Git.
- Proving more impact than the engagement requires.

## Defender view

Defenders benefit from server-side authorization on every sensitive action,
safe input handling, secure session settings, useful audit logs, dependency
management, minimal error detail, and security tests inside the development
process.

## Quiz

1. Why should a tester learn the normal workflow first?
2. What is the difference between authentication and authorization?
3. Why is a scanner alert not proof of a vulnerability?
4. What does changing one variable at a time achieve?
5. Why should test impact be minimized?

## Answer key

1. The expected behavior provides the baseline needed to identify and explain
   an unsafe difference.
2. Authentication identifies the user; authorization decides what that user is
   allowed to do.
3. Automated tools can misunderstand context and produce false positives or
   incomplete evidence.
4. It makes the cause of a changed response easier to isolate and reproduce.
5. The goal is reliable evidence, not unnecessary access, data exposure, or
   operational risk.

## Flashcards

**Q:** What is a web attack surface?  
**A:** The reachable features, inputs, endpoints, roles, and technologies that may affect security.

**Q:** Where should authorization be enforced?  
**A:** On the server for every sensitive object and action.

**Q:** What makes a finding reproducible?  
**A:** Clear prerequisites, exact actions, expected behavior, actual behavior, and evidence.

**Q:** What is a business-logic flaw?  
**A:** A harmful result caused by using valid features in an unintended sequence or context.

**Q:** Should session tokens appear in a committed screenshot?  
**A:** No. Redact them or capture safer evidence.

## Safe practical exercise

Use OWASP Juice Shop, WebGoat, or a PortSwigger Academy lab covered by its
training terms. Select one feature and create an application map containing:

- Entry point and expected user role.
- Inputs and resulting server response.
- Data object affected.
- Expected authorization rule.
- One harmless test for a boundary condition.
- Evidence and cleanup.

Stop after demonstrating the assigned lab objective. Write the result with
[the finding template](../Reports/Finding-Report-Template.md).

## Completion checklist

- [ ] I can map a feature before testing it.
- [ ] I can distinguish identity, permissions, sessions, and input handling.
- [ ] I can manually validate a suspected issue.
- [ ] I completed an authorized training lab and sanitized its evidence.
