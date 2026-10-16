---
name: editor
description: Edit, revise, proofread, restructure, or critique text for accuracy, clarity, structure, concision, consistency, tone, and mechanics. Use when the user asks to improve writing, rewrite or polish text, reorganize it for readability, review documentation, correct grammar, tighten prose, compare drafts, or explain editorial changes.
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
- **Restructure:** Focus on organization and presentation for readability: reorder sections, group related ideas, split dense paragraphs, and use headings or lists where useful. Rewrite only as needed to connect the reorganized text.
- **Critique:** Diagnose problems and recommend changes without silently rewriting the entire text.

If the user does not specify a level, make the smallest edit that fully solves the evident wording problems. Preserve the sequence of ideas and the overall structure: do not move later prerequisites to the beginning, reorder sections, or convert prose into a list without permission. Recommend those changes instead.

### Offer restructuring when useful

Editing and restructuring are separate options. A request to edit, polish, or improve readability does not by itself authorize substantial reorganization. An explicit request to revise, restructure, or reorganize does; proceed without asking again.

When the main point is buried, related ideas are scattered, or dense paragraphs obscure the logic, briefly recommend restructuring as an optional next step. Name the specific benefit, such as grouping prerequisites before instructions or separating decisions from background.

Complete the requested edit first, then offer the option in a short note. Do not withhold the edit to ask the user to choose, produce a second restructured version unless requested, or recommend restructuring when local edits are enough. Honor requests to preserve the structure or return only the edited text.

When restructuring is requested, choose the organization that best serves the reader. Preserve every factual claim, qualification, prerequisite, and dependency; do not force prose into headings or lists when paragraphs work better.

## Editing workflow

1. Identify the text's main point and intended reader.
2. Mark claims whose meaning, evidence, or certainty must remain unchanged.
3. Fix factual contradictions and ambiguities only when the source text provides enough information. Otherwise flag them.
4. Within the agreed editing level, put the main point where the reader needs it.
5. When restructuring is authorized, order supporting information by logic, chronology, or importance.
6. Give each paragraph one job; preserve the overall organization unless restructuring is authorized.
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
- paragraphs and lists are clear within the agreed scope; larger ordering problems are flagged when restructuring is not authorized
- terminology is consistent
- examples support the stated point
- the opening earns attention and the ending stops cleanly
- every remaining word serves the reader
