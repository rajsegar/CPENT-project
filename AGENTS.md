# AGENTS.md

## Purpose

This repository is a beginner-friendly CPENT study knowledge base. Help the
student understand concepts, practise safely, and produce clear evidence and
reports.

These instructions apply to the whole repository.

## Non-negotiable rules

- Do not delete, rename, or overwrite existing study material unless the user
  explicitly asks for that exact change.
- Keep all study content in Markdown unless another format is explicitly
  requested.
- Use only synthetic examples, local lab addresses, and obvious placeholders.
- Never add real credentials, tokens, customer data, private targets, or
  unredacted screenshots.
- Put authorization, scope, safety, and cleanup before tooling.
- Do not suggest testing public or third-party systems without written
  permission.
- Avoid destructive actions, denial of service, persistence, or evasion steps
  unless the user explicitly requests a controlled lab exercise and the safety
  context is clear.

## Writing style

- Write for a motivated beginner.
- Define an acronym the first time it appears.
- Start with what a concept means and why it matters.
- Use short sections, small examples, and practical checklists.
- Separate facts from study tips or assumptions.
- Explain business impact as well as technical impact.
- Prefer placeholders such as TARGET_IP, LAB_DOMAIN, and TEST_USER.

## Module convention

Each core module should normally provide:

- Beginner notes and a completion checklist.
- Quiz questions followed by a separate answer-key section.
- An authorized, repeatable practical exercise.
- Focused question-and-answer flashcards.

These may be sections in the module README while a module is concise. Split
them into Notes.md, Quiz.md, Labs.md, and Flashcards/Flashcards.md when the
material grows. Commands.md and Cheatsheet.md are optional when they genuinely
help; do not add commands simply to fill a file.

## Lab convention

Every lab must state:

1. The learning objective.
2. The authorized target type.
3. Preconditions and safety limits.
4. Tasks at a level appropriate for the learner.
5. Evidence to collect.
6. Cleanup or restoration steps.
7. Reflection questions.

Use the shared lab template in Templates/Lab-Template.md.

## Quiz and flashcard convention

- Put answers after all quiz questions so the learner can self-test.
- Include explanations for answers when the reasoning is not obvious.
- Test understanding and decision-making, not only vocabulary.
- Keep each flashcard focused on one idea.

## Report convention

- State observation, evidence, impact, likelihood, severity, and remediation.
- Do not claim impact that the evidence does not support.
- Separate executive language from technical reproduction detail.
- Redact secrets and personal data.
- Record timestamps and time zones for evidence.

## Quality checks

Before finishing a change:

- Confirm relative Markdown links resolve.
- Confirm headings are in a sensible order.
- Confirm no placeholders look like real secrets or production targets.
- Confirm instructions stay within an authorized lab context.
- Confirm no existing files were unintentionally removed.
