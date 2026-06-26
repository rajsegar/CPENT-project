# Module 03: Open Source Intelligence (OSINT)

## In plain language

Open Source Intelligence (OSINT) is information collected from lawful,
publicly available sources and analyzed to answer a specific question.
Collection is only half the job; useful OSINT also records source quality,
time, context, and confidence.

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
3. Record the source URL and collection time.
4. Separate facts, claims, and your own inference.
5. Corroborate important claims.
6. Rate confidence and note when information may be stale.
7. Stop collecting personal data that does not serve the objective.

Examples of useful categories include official domain records, public company
documents, technology documentation, job advertisements, code repositories,
and metadata intentionally published by the asset owner. Each may be outdated
or misleading, so verify before drawing conclusions.

## Common mistakes

- Treating a search result snippet as primary evidence.
- Assuming an email pattern proves a real account exists.
- Copying personal information without a clear need.
- Forgetting that active requests can be logged.
- Reporting an inference as a verified fact.
- Failing to record when a source was collected.

## Defender view

Organizations reduce exposure by maintaining accurate public records, removing
unnecessary metadata, reviewing public code and documents, monitoring lookalike
domains, and training staff not to publish sensitive operational detail.

## Quiz

1. What makes OSINT different from simply searching the web?
2. Why should collection time be recorded?
3. What is corroboration?
4. Is publicly visible personal information automatically appropriate to collect?
5. What should a report do with an unverified inference?

## Answer key

1. OSINT starts with a defined question and uses documented collection,
   analysis, source evaluation, and confidence.
2. Public information changes; time helps a reviewer judge whether evidence was
   current during the assessment.
3. It is checking an important claim against independent evidence.
4. No. Permission, purpose, privacy, and data minimization still apply.
5. Label it clearly as an inference, state the evidence, and avoid overstating
   confidence.

## Flashcards

**Q:** What should guide OSINT collection?  
**A:** A specific, authorized intelligence question.

**Q:** What is passive OSINT?  
**A:** Collection that avoids direct interaction with target systems.

**Q:** Why can public data still be sensitive?  
**A:** Combining harmless details can reveal people, systems, or business processes.

**Q:** What is source confidence?  
**A:** A reasoned judgment about how strongly the evidence supports a claim.

**Q:** What should every saved source include?  
**A:** Its origin, collection time, relevance, and any reliability limitation.

## Safe practical exercise

Choose a deliberately fictional company. Create a one-page collection plan with:

- Three questions an assessor might need to answer.
- Two public source types for each question.
- A note explaining source reliability.
- A data-minimization rule.
- A table separating facts, possible inferences, and unknowns.

Do not investigate a real person or organization. The goal is to practise
reasoning and evidence structure, not collection volume.

## Completion checklist

- [ ] I can distinguish passive and active collection.
- [ ] I can separate a fact from an inference.
- [ ] I can explain source reliability and confidence.
- [ ] I completed the fictional-company exercise.
