# Research Writing Skill Pack

This pack packages an engineering-oriented research-paper workflow into modular skills plus one router skill.

## Included skills

- `paper-workflow-suite`
- `research-supervision`
- `literature-review`
- `research-positioning`
- `citation-audit`
- `method-design`
- `figure-table-storytelling`
- `reviewer-preflight`
- `chapter-polisher`

## Recommended order

1. `paper-workflow-suite` when the user is unsure where to start
2. `research-supervision` to define checkpoints, artifacts, and automation boundaries
3. `literature-review` to build the evidence base
4. `research-positioning` to sharpen the paper's claim
5. `method-design` to write Section 3 or equivalent
6. `figure-table-storytelling` to shape visuals and captions around the argument
7. `citation-audit` to verify support before overcommitting
8. `reviewer-preflight` to catch reviewer-visible weaknesses
9. `chapter-polisher` to prepare a clean draft for export or submission

## Nonlinear collaboration

The suite does not require a from-scratch starting point.

You can enter with:

- a half-formed idea
- a rough method note
- result figures
- a section draft
- a full but weak manuscript
- reviewer comments

In those cases, the default move is diagnosis first, then routing to the smallest next skill that can unblock the work. The collaboration guide lives in [collaboration_methodology.md](paper-workflow-suite/references/collaboration_methodology.md).

## Domain adaptation

Use the suite with a domain lens:

- transportation engineering: prioritize network scale, time horizon, demand variability, and deployment realism
- energy and environmental engineering: prioritize system boundary, functional unit, accounting method, and scale-up feasibility
- ocean engineering: prioritize sea state, environmental load, coupling assumptions, and validation regime
- low-altitude aircraft systems: prioritize flight envelope, mission profile, safety and regulation, and evidence tier

The domain guide lives in [domain_workflows.md](paper-workflow-suite/references/domain_workflows.md).

## Chinese prompt pack

Copy-ready Chinese prompts live in [zh_prompt_templates.md](paper-workflow-suite/references/zh_prompt_templates.md).
If you want a compact intake sheet before invoking any skill, use [domain_input_card.md](paper-workflow-suite/references/domain_input_card.md).
Automation critique and adoption policy live in [autonomous_research_critique.md](paper-workflow-suite/references/autonomous_research_critique.md).
Nonlinear collaboration guidance lives in [collaboration_methodology.md](paper-workflow-suite/references/collaboration_methodology.md).

## When to skip stages

- If the user already has a mature review matrix, jump directly to `research-positioning`.
- If the user wants AI help coordinating the whole project, start with `research-supervision` before drafting anything serious.
- If the user arrives with partial materials, diagnose first instead of restarting from stage 1.
- If the user already has mature results but weak figures, jump directly to `figure-table-storytelling`.
- If the draft is near submission, run `reviewer-preflight` before final polishing.
- If the user only wants prose cleanup, use `chapter-polisher`, but still surface missing citation risks.
- If the user only wants bibliography cleanup, use `citation-audit` alone.
