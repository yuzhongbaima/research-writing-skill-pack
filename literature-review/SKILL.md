---
name: literature-review
description: Run a structured literature review workflow for engineering-focused academic writing. Use when the user needs paper scouting, thematic synthesis, related-work drafting, evidence extraction, or a review matrix in engineering or applied-technical domains.
---

# Literature Review

Use this skill when the task starts with sources, themes, or related work.

This skill is tuned for engineering fields where papers may need to be compared across physical conditions, system scales, validation regimes, and deployment settings.

## Goals

- Identify the most relevant paper clusters
- Identify the most relevant paper clusters and source types
- Extract claims, methods, settings, and limitations
- Distinguish mature consensus from isolated findings
- Produce reusable notes for later positioning and writing

## Workflow

1. Define the review target in one sentence: topic, decision problem, population, and scope.
2. Build a paper set with brief inclusion logic.
3. If the area is engineering-heavy, tag each source by evidence type:
   - analytical
   - simulation
   - lab experiment
   - hardware-in-the-loop
   - field or operational study
3. For each source, capture:
   - core question
   - method or paper type
   - system or application setting
   - operating conditions or scale if relevant
   - main finding
   - limitation or blind spot
   - direct relevance to the user's paper
4. Group sources by theme rather than by publication order.
5. In engineering topics, compare sources on validation strength, not just headline performance.
6. End with synthesis:
   - what the field knows
   - where the field disagrees
   - what is missing for the user's paper

## Output shape

Prefer:

- a review matrix
- an evidence ladder or validation map
- a clustered related-work note
- a short "implications for my paper" section

## Guardrails

- Do not present a bag of summaries as a literature review.
- Do not treat standards, white papers, and peer-reviewed articles as interchangeable evidence.
- Highlight limitations and boundary conditions, not just positive findings.
- Mark uncertain or second-hand claims clearly.
- Save unresolved search gaps for follow-up instead of papering over them.
