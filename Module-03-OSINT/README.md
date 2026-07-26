# Module 03: Open Source Intelligence (OSINT)

## Status

**Module status:** Completed  
**Completion date:** 26 July 2026  
**Practical lab:** Completed  
**Evidence screenshots:** Submitted  
**Final quiz:** Passed — 21/25 (84%)  
**Next module:** Module 04

## In plain language

Open Source Intelligence (OSINT) is information collected from lawful,
publicly available sources and analyzed to answer a specific question.
Collection is only half the job; useful OSINT also records source quality,
time, context, and confidence.

## Study material

- [Module 03 OSINT Collection Plan Lab](OSINT-Collection-Plan.md)

## Key ideas

| Term | Beginner-friendly meaning |
| --- | --- |
| Passive collection | Research that does not directly interact with the target system |
| Active collection | Direct interaction that may be visible to the target |
| Source reliability | How trustworthy and authoritative a source is |
| Corroboration | Checking a claim against independent evidence |
| Operational security | Avoiding accidental exposure of the assessment or sensitive data |
| Data minimization | Collecting only what is needed for the agreed objective |

## A simple OSINT workflow

1. Begin with a scoped question, not a tool.
2. Identify suitable public and authoritative sources.
3. Record the source and collection time.
4. Separate facts, claims, and inferences.
5. Corroborate important claims.
6. Rate confidence and note stale or uncertain information.
7. Stop collecting personal data that does not support the objective.
8. Confirm written scope before active validation.

## Important lessons

- Public visibility does not automatically create permission to test.
- A discovered domain or subdomain is a lead, not automatic scope.
- Passive collection avoids directly probing the target.
- Active discovery sends traffic and requires explicit authorization.
- A fact states what the evidence proves; an inference states what it may suggest.
- An open port proves reachability, not vulnerability.
- DNS zone-transfer checks require an approved lab or explicit authorization.
- Automation and AI results require human validation.
- Decommissioning unused or legacy Internet-facing assets reduces external exposure.

## Common mistakes

- Treating a search-result snippet as primary evidence.
- Assuming an email pattern proves that an account exists.
- Copying personal information without a clear need.
- Forgetting that active requests can be logged.
- Reporting an inference as a verified fact.
- Failing to record when a source was collected.
- Treating shared or third-party infrastructure as automatically in scope.

## Defender view

Organizations reduce exposure by maintaining accurate public records, removing
stale services and unnecessary metadata, reviewing public code and documents,
monitoring certificates and lookalike domains, restricting DNS zone transfers,
and maintaining an authoritative external asset inventory.

## Completion checklist

- [x] I can distinguish passive and active collection.
- [x] I can separate data from intelligence.
- [x] I can separate a fact from an inference.
- [x] I can explain source reliability and confidence.
- [x] I understand corroboration using an independent source.
- [x] I understand privacy and data minimization.
- [x] I reviewed DNS, WHOIS, subdomain, archive, metadata, and scanning concepts.
- [x] I completed the fictional-company exercise.
- [x] I completed the attack-surface map.
- [x] I submitted sanitized evidence screenshots.
- [x] I passed the final quiz with 21/25 (84%).

## Final result

```text
Module 03 — Completed
Practical lab — Completed
Evidence — Submitted
Quiz — Passed, 21/25 (84%)
Ready for Module 04 — Yes
```
