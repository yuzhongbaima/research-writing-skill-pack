---
name: research-supervision
description: Supervise a human-gated semi-automated research workflow for high-quality papers. Use when the user wants AI to coordinate literature search, hypothesis branching, experiment execution, and drafting while keeping human approval at critical checkpoints.
---

# Research Supervision

Use this skill when the task is larger than one section or one experiment and the user wants AI help coordinating the whole research process without surrendering scientific judgment.

The starting point does not need to be clean. The user may come with partial notes, a draft, an experiment folder, or reviewer comments. This skill should absorb existing materials and establish supervision from the current state forward.

This skill is intentionally not full autonomy. It borrows useful mechanisms from autonomous research systems, but it treats human approval as part of the method rather than as a nuisance.

## Main job

Run a semi-automated research workflow with explicit gates, artifact tracking, and claim discipline.

## Workflow

1. Define the research target:
   - target venue class
   - contribution type
   - evidence level required
   - forbidden shortcuts
   - current stage and inherited materials
2. Create a stage plan:
   - literature search and screening
   - positioning and hypothesis selection
   - experiment or validation design
   - execution and logging
   - results analysis and claim control
   - drafting and reviewer preflight
3. Set mandatory human gates:
   - literature screen approval
   - experiment design approval
   - results interpretation approval
   - final claim and submission approval
4. Track artifacts at each stage:
   - search log
   - inclusion and exclusion note
   - experiment manifest
   - result summary
   - claim ledger
   - risk register
5. If multiple directions exist, branch early at the hypothesis level, not after full drafting.
6. Prefer narrowing the claim over inflating the evidence.
7. If the user already has partial outputs, start with a state diagnosis and retrofit the right gates around the current project state.

## High-stakes rules

- Do not use simulated results in a publishable draft unless the paper is explicitly about simulation or synthetic benchmarking, and even then label it honestly.
- Do not allow AI-generated text to introduce numbers, comparisons, or claims that are not traceable to artifacts.
- Do not let literature relevance scoring replace human reading for the final citation set.
- Do not draft a polished paper before the evidence base and method plan survive human review.
- Do not assume existing drafts are structurally correct; a supervision pass may recommend reframing before more writing.

## Nature Communications mindset

For ambitious journal targets, assume the bar is closer to:

- stronger evidence chains
- tighter claim-evidence alignment
- clearer limitations
- more credible validation
- less tolerance for speculative automation artifacts

When in doubt, downgrade claim strength, add validation, or keep the work at a more modest venue target.

## Output shape

Prefer:

- `state_diagnosis.md`
- `supervision_plan.md`
- `gate_checklist.md`
- `artifact_manifest.md`
- `claim_ledger.md`
- `risk_register.md`

## References

Load [autonomous_research_critique.md](../paper-workflow-suite/references/autonomous_research_critique.md) when the user wants the rationale behind the gates and automation limits.
