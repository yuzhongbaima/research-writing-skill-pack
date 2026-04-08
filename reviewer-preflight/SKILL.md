---
name: reviewer-preflight
description: Review an engineering or applied-technical paper draft from the perspective of a skeptical reviewer before submission. Use when the user wants reviewer-style criticism, submission readiness checks, venue-fit checks, or a prioritized risk list.
---

# Reviewer Preflight

Use this skill when the draft is mature enough that the next high-value step is criticism rather than more drafting.

## Main job

Simulate a strong but fair reviewer and surface the issues most likely to hurt acceptance or credibility.

## Workflow

1. Identify the target venue or the closest venue class:
   - engineering journal
   - engineering conference
   - interdisciplinary systems venue
2. Read the draft as a reviewer would:
   - contribution clarity
   - adequacy of validation
   - fairness of comparison
   - limitations and boundary conditions
   - writing clarity
3. Prioritize findings by risk:
   - major validity threat
   - likely reviewer objection
   - fixable presentation weakness
4. If the venue is known, check visible requirements:
   - format or page pressure
   - anonymous review requirements
   - ethics, safety, or broader-impact sections
   - data or code availability expectations

## Engineering-specific checks

- Are units, operating conditions, and assumptions stated clearly enough?
- Is the validation regime appropriate for the claim strength?
- Are simulation results being overgeneralized to real deployment?
- Are safety, energy, environment, reliability, or cost implications addressed when central to the topic?
- Are comparisons fair in terms of conditions, hardware, and baselines?

## Output shape

Prefer:

- top 5 reviewer concerns
- severity labels
- fix suggestions
- short submission checklist

## Guardrails

- Do not nitpick style while missing core validity problems.
- Do not demand unrealistic scope expansion if a narrower framing would solve the issue.
- Keep criticism specific and actionable.
