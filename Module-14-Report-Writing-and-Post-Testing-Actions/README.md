# Module 14: Report Writing and Post-Testing Actions

## In plain language

A penetration test creates value only when evidence becomes a clear decision:
what happened, why it matters, how confident the tester is, what should be
fixed, and how the fix will be verified. Post-testing actions also return the
environment and sensitive data to the agreed state.

## From evidence to action

| Report element | Question it answers |
| --- | --- |
| Observation | What did the tester see? |
| Reproduction | How can an authorized reviewer verify it? |
| Impact | What technical and business outcome was demonstrated? |
| Likelihood | How realistic is the required access and effort? |
| Severity | How urgently should this be prioritized in context? |
| Remediation | What durable change addresses the root cause? |
| Retest | What evidence would show the issue is resolved? |
| Limitation | What was not tested or remains uncertain? |

## A reliable reporting workflow

1. Index evidence while testing, with timestamps and assets.
2. Separate confirmed facts from hypotheses and untested impact.
3. Group evidence by root cause rather than tool alert.
4. Write a concise title, summary, impact, reproduction, and remediation.
5. Calibrate severity using technical and business context.
6. Write the executive summary after the findings are stable.
7. Perform a consistency and sensitive-data review.
8. Complete cleanup, evidence transfer, debriefing, and retest planning.

The technical section should be reproducible by an authorized specialist. The
executive section should be useful to a decision-maker without requiring them
to interpret tool output.

## Common mistakes

- Copying raw scanner output into the report.
- Claiming data access or takeover that was not demonstrated.
- Hiding limitations in an appendix.
- Giving vague remediation such as "improve security."
- Using severity as a substitute for explaining impact.
- Leaving credentials, tokens, or personal data in evidence.
- Marking a finding fixed without a focused retest.

## Useful templates

- [Single finding](../Reports/Finding-Report-Template.md)
- [Full penetration test report](../Reports/Penetration-Test-Report-Template.md)
- [Executive summary](../Reports/Executive-Summary-Template.md)
- [Evidence log](../Reports/Evidence-Log-Template.md)
- [Retest report](../Reports/Retest-Report-Template.md)

## Quiz

1. What is the difference between an observation and impact?
2. Why should facts and hypotheses be labeled separately?
3. What makes remediation actionable?
4. Why is severity context-dependent?
5. What must happen after technical testing ends?

## Answer key

1. An observation is what the evidence directly shows; impact is the verified
   or carefully qualified consequence of that condition.
2. Readers need to know what is proven, what is inferred, and where uncertainty
   remains.
3. It identifies the root cause, responsible control, concrete change, priority,
   and validation method.
4. Exposure, data, business process, existing controls, exploitability, and
   organizational tolerance change the practical risk.
5. Cleanup, evidence handling, urgent notification where needed, reporting,
   debriefing, remediation planning, and retest agreement.

## Flashcards

**Q:** What is evidence?  
**A:** Recorded information that supports a reproducible claim.

**Q:** What belongs in a finding title?  
**A:** The affected control or condition and its meaningful consequence.

**Q:** What is residual risk?  
**A:** Risk that remains after a control or remediation is applied.

**Q:** When is a finding fixed?  
**A:** When focused retesting shows the original condition is gone and the intended control works.

**Q:** Why report positive observations?  
**A:** They add context, recognize effective controls, and support practical prioritization.

## Safe practical exercise

Use this fictional evidence:

- A lab user could view another lab user's invoice.
- The server returned the invoice after only its numeric identifier changed.
- No administrative access or bulk data access was tested.
- Both test users and invoices were synthetic.

Write a complete finding with a factual title, scope, reproduction, sanitized
evidence, demonstrated impact, untested impact, severity rationale, root-cause
remediation, and retest plan. Then write a three-sentence executive summary.

Finish by completing a cleanup checklist and marking synthetic accounts and
evidence for disposal.

## Completion checklist

- [ ] I can turn evidence into a precise, qualified claim.
- [ ] I can write for both technical and executive readers.
- [ ] I can recommend a root-cause fix and a retest method.
- [ ] I completed cleanup and evidence-handling notes.
