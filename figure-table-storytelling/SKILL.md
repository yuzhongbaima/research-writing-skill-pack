---
name: figure-table-storytelling
description: Plan engineering-paper figures, tables, plot choices, and captions. Use when the user needs experimental plot recommendations, architecture diagrams, result tables, figure titles, table titles, or publication-ready captions.
---

# Figure Table Storytelling

Use this skill when the paper has results, a system pipeline, or a method structure that needs to become visual evidence.

This skill is especially useful in engineering domains where plots must communicate operating conditions, uncertainty, and tradeoffs rather than just prettier graphics.

## Main job

Turn raw results or method structure into figures and tables that carry argumentative load.

## Workflow

1. Identify the visual's job:
   - method overview
   - apparatus or system architecture
   - benchmark comparison
   - sensitivity or ablation
   - tradeoff analysis
   - field case or deployment summary
2. Choose the right artifact:
   - line plot for trends over time, distance, speed, load, or horizon
   - scatter or Pareto-style plot for tradeoffs
   - box or violin plot for variability
   - grouped bar only when category comparison is the real story
   - table when exact values or many conditions matter
   - pipeline or block diagram for system structure
3. Write a caption that explains:
   - what is shown
   - under which conditions
   - what the reader should notice
4. Check visual integrity:
   - axis labels
   - units
   - legend clarity
   - uncertainty display
   - color or line-style accessibility
5. If the figure is for a paper, align the wording with the section's argument.

## Output shape

Prefer one or more of:

- `figure_plan.md`
- caption drafts
- table schema
- plot recommendation list
- title options for figures and tables

## Guardrails

- Do not use a bar chart by default when the story is continuous or uncertainty-heavy.
- Do not omit units or operating conditions in engineering plots.
- Avoid captions that only rename the figure; captions should interpret it.
- If exact numeric comparison matters, recommend a table even if a chart looks nicer.
