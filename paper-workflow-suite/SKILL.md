---
name: paper-workflow-suite
description: Orchestrate an engineering-focused academic writing workflow in Codex. Use when the task spans research supervision, literature review, research positioning, figure or table planning, citation checking, method-section design, reviewer preflight, or chapter polishing and you need the right sub-skill order.
---

# Paper Workflow Suite

Use this skill as the entry point when the user is writing a paper or building a research note set and the work may span multiple stages.

The user does not need to start from zero. This suite supports nonlinear entry from half-finished ideas, rough notes, methods, figures, drafts, or reviewer feedback.

This suite is optimized for engineering-heavy fields such as transportation, energy saving and environmental engineering, ocean engineering, and low-altitude aircraft systems. It can still support computing papers, but it defaults to engineering evidence, validation, and writing norms.

## What this suite covers

- Literature reconnaissance and synthesis
- Human-gated semi-automated research supervision
- Midstream diagnosis and coauthor-style intervention
- Gap framing and research positioning
- Figure, table, and caption planning
- Citation support checks and bibliography hygiene
- Method-section design for conceptual or early-stage empirical papers
- Reviewer-perspective preflight and submission checks
- Chapter-level Markdown polishing and export preparation

## Skill routing

Pick the narrowest skill that fits the task. If the user asks for end-to-end paper help, route through this sequence:

1. `research-supervision` for setting gates, artifacts, and human-approval policy before the workflow accelerates
2. `literature-review` for evidence extraction and structured synthesis
3. `research-positioning` for narrowing the problem, gap, thesis, and contribution claims
4. `method-design` for translating the positioned problem into a defensible method section
5. `figure-table-storytelling` for turning results or system structure into publishable figures, tables, and captions
6. `citation-audit` for checking whether claims are actually supported and whether citations are missing, weak, or duplicated
7. `reviewer-preflight` for reviewer-perspective critique, venue-fit checks, and pre-submission risk discovery
8. `chapter-polisher` for section cleanup, consistency passes, and export-ready Markdown

If the user arrives with partial material, diagnose first, then route to the smallest next skill that can unblock the work.

## Stage detection

Use these cues:

- If the user says "help me automate the whole workflow", "set checkpoints", "I want AI to coordinate the project", or "I want a semi-automatic pipeline with human review", use `research-supervision`.
- If the user provides half-finished notes, a rough method, incomplete figures, or a partial manuscript and wants to improve the underlying research logic, start with diagnosis and coauthor-style discussion before choosing the next narrow skill.
- If the user says "find papers", "summarize related work", or "make a review matrix", start with `literature-review`.
- If the user says "what is the gap", "how do I position this", or "help me make contributions sharper", use `research-positioning`.
- If the user says "how should I draw this result", "write a caption", "what plot fits this experiment", or "turn this result into a table", use `figure-table-storytelling`.
- If the user says "check citations", "which claims are unsupported", or "clean the references", use `citation-audit`.
- If the user says "write Section 3", "turn this idea into a method", or "avoid sounding like a product pitch", use `method-design`.
- If the user says "review this like a reviewer", "help me preflight before submission", or "check venue requirements", use `reviewer-preflight`.
- If the user says "polish this section", "make it submission-ready", or "prepare a PDF/export draft", use `chapter-polisher`.

## Working rules

- Prefer Markdown-first outputs unless the user explicitly asks for TeX.
- Separate evidence-backed statements from speculative framing.
- Keep a clear distinction between: observed literature pattern, inferred gap, and proposed contribution.
- Keep a clear distinction between: supported fact, inference from current materials, and hypothesis needing verification.
- Avoid inventing citations. If evidence is missing, mark the sentence as unsupported instead of smoothing over it.
- For early-stage papers, optimize for defensible structure rather than fake completeness.
- In engineering fields, track units, operating conditions, boundary conditions, and uncertainty as first-class writing constraints rather than editorial afterthoughts.
- Distinguish simulation evidence, bench evidence, and field evidence. Do not let one masquerade as another.
- Default to human-gated automation, not full automation, for publishable research.
- Never treat synthetic or simulated results as publication-grade evidence unless the paper is explicitly about simulation and says so honestly.
- Diagnose before rewriting when the user provides partial or weak materials.
- Act like a serious coauthor: challenge assumptions, suggest alternatives, and improve the research logic rather than only polishing prose.
- Do not force the workflow back to stage one unless a foundational problem truly requires it.

## Shared outputs

Prefer one or more of these artifacts depending on the stage:

- `supervision_plan.md`
- `state_diagnosis.md`
- `next_move.md`
- `review_matrix.md`
- `positioning_note.md`
- `figure_plan.md`
- `citation_audit.md`
- `method_outline.md`
- `reviewer_preflight.md`
- `section_draft.md`

## References

Load [workflow_map.md](references/workflow_map.md) when you need the end-to-end logic or need to explain the suite to the user.
Load [collaboration_methodology.md](references/collaboration_methodology.md) when the user is entering from a partial draft, rough idea, reviewer feedback, or wants deeper research collaboration rather than linear workflow execution.
Load [engineering_adaptation.md](references/engineering_adaptation.md) when the paper is outside core computer science and needs engineering-specific adjustment.
Load [autonomous_research_critique.md](references/autonomous_research_critique.md) when the task involves research automation, stage orchestration, or human gate design.
Load [domain_workflows.md](references/domain_workflows.md) when the paper is specifically in transportation, energy and environment, ocean engineering, or low-altitude aircraft.
Load [domain_input_card.md](references/domain_input_card.md) when the user gives underspecified project context and you need a compact intake structure.
Load [zh_prompt_templates.md](references/zh_prompt_templates.md) when the user wants reusable Chinese prompts or wants to trigger the workflow with copy-ready templates.
