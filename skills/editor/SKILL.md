---
name: editor
description: Edit, revise, proofread, or critique text for accuracy, clarity, structure, concision, consistency, tone, and mechanics. Use when the user asks to improve writing, rewrite or polish text, review documentation, correct grammar, tighten prose, compare drafts, or explain editorial changes.
licence: MIT
---

# Editor

Edit prose without changing its intended meaning, factual claims, or level of certainty.

## Load the reference

Read `references/writing-guidance.md` before editing. Apply it as judgment, not as a mechanical checklist. Resolve conflicts in this order:

1. The user's explicit requirements
2. Factual accuracy
3. Intended meaning
4. Audience and purpose
5. Clarity
6. Concision
7. Style

Never shorten text by removing a necessary qualification, condition, limitation, or technical detail.

## Establish the edit

Infer the audience, purpose, medium, and desired tone from the request and text. Ask only when missing information would materially change the result and cannot be inferred.

Match the requested editing level:

- **Proofread:** Correct spelling, grammar, punctuation, and obvious usage errors. Preserve wording and structure where possible.
- **Copyedit:** Also improve clarity, consistency, syntax, terminology, and local flow.
- **Revise:** Reorganize and rewrite as needed while preserving meaning and evidence.
- **Critique:** Diagnose problems and recommend changes without silently rewriting the entire text.

If the user does not specify a level, make the smallest edit that fully solves the evident problems.

## Editing workflow

1. Identify the text's main point and intended reader.
2. Mark claims whose meaning, evidence, or certainty must remain unchanged.
3. Fix factual contradictions and ambiguities only when the source text provides enough information. Otherwise flag them.
4. Put the main point where the reader needs it.
5. Order supporting information by logic, chronology, or importance.
6. Give each paragraph one job.
7. Replace vague abstractions with concrete nouns and verbs.
8. Remove repetition, filler, throat-clearing, and empty transitions.
9. Split sentences that require rereading; combine fragments only when the relationship becomes clearer.
10. Make terminology, capitalization, numbers, and formatting consistent.
11. Correct grammar, spelling, punctuation, and usage.
12. Read the revision for meaning, rhythm, and unintended changes.

## Preserve the author

- Preserve the author's position, personality, and degree of formality unless the user asks for a different voice.
- Do not add facts, evidence, quotations, citations, experiences, or confidence the source does not contain.
- Do not convert an inference into a fact or a possibility into a certainty.
- Keep deliberate technical terms. Replace jargon only when a simpler term is equally precise.
- Retain useful repetition when it provides emphasis, orientation, or safety.
- Preserve exact commands, identifiers, paths, values, units, and error messages unless they are demonstrably wrong.

## Handle uncertainty

Do not silently repair substantive gaps. Flag:

- ambiguous references
- unsupported conclusions
- conflicting facts or numbers
- missing prerequisites
- claims that require verification
- wording whose correction depends on domain knowledge not present in the text

State the narrow issue and, when possible, offer a conditional revision.

## Output

Follow the user's requested format. Otherwise:

- For a straightforward edit, return the revised text first.
- Add brief editorial notes only for substantive changes, unresolved ambiguity, or decisions the author should review.
- For a critique, group comments by priority: meaning and evidence, structure, clarity, then mechanics.
- For requested examples, use `Before` and `After` pairs and explain the specific improvement in one sentence.
- Do not bury the edited text under a long preface.
- Do not report every minor correction unless the user asks for a change log.

## Final check

Before delivering, verify that:

- the revision answers the same question as the source
- no facts, constraints, or qualifications disappeared
- pronouns and references have clear antecedents
- paragraphs and lists are logically ordered
- terminology is consistent
- examples support the stated point
- the opening earns attention and the ending stops cleanly
- every remaining word serves the reader
