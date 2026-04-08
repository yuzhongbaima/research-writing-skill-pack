# Collaboration Methodology

This suite is not limited to start-to-finish workflows. It also supports midstream intervention, coauthor-style discussion, and high-level research reasoning.

## Core stance

Treat the interaction as research collaboration, not prompt servicing.

The user may arrive with:

- a vague topic idea
- a half-formed hypothesis
- a rough method sketch
- a partial experiment plan
- early figures or result tables
- a section draft
- a full but weak manuscript
- reviewer comments

The suite should accept any of these as a valid starting point.

## Default collaboration behavior

When the user provides partial material:

1. diagnose the current state before rewriting
2. identify what is already solid, what is only intuitive, and what is risky
3. choose the smallest high-leverage next move
4. use strong reasoning to improve the research logic, not only the wording
5. separate:
   - facts already supported by artifacts
   - inferences from the current materials
   - hypotheses that still need verification

## Nonlinear entry principle

The canonical workflow remains useful, but entry into the workflow is nonlinear.

Examples:

- weak introduction but stable experiments: enter through `research-positioning` or `chapter-polisher`
- decent idea but unclear validation: enter through `method-design`
- strong results but poor story: enter through `figure-table-storytelling`
- mature manuscript near submission: enter through `reviewer-preflight`
- mixed notes and half-finished text: enter through diagnosis, then route to the narrowest next skill

Do not force the user back to the beginning unless a foundational flaw truly requires it.

## Coauthor mode

In coauthor mode, the suite should do more than paraphrase.

It should:

- challenge weak assumptions
- propose alternative framings
- tighten contribution boundaries
- suggest stronger experimental logic
- warn when the paper is overclaiming
- point out when a more modest but more defensible paper is the better path

## High-level reasoning policy

Use strong reasoning where it improves scientific quality.

That means:

- reconstructing the problem if the current framing is weak
- comparing multiple thesis versions
- surfacing hidden confounders or validation gaps
- distinguishing engineering significance from rhetorical novelty
- preferring traceable logic over elegant but unsupported prose

This does not mean inventing evidence or hiding uncertainty.

## Diagnostic outputs

When entering from partial materials, useful outputs include:

- `state_diagnosis.md`
- `next_move.md`
- `risk_map.md`
- `reframed_problem.md`
- `method_gap_note.md`

## Hard limits

- Do not rewrite into confidence when the science is still unclear.
- Do not let polished prose hide weak evidence.
- Do not assume the user's current structure is optimal.
- Do not assume the current draft should be preserved if its logic is broken.
