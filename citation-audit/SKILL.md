---
name: citation-audit
description: Audit citation support in engineering or applied-technical academic drafts. Use when the user needs unsupported claims identified, citation strength checked, bibliography issues flagged, or claim-to-source alignment improved.
---

# Citation Audit

Use this skill when a draft exists and the question is whether the citations genuinely support it.

## Workflow

1. Mark the claims that carry argumentative weight.
2. For each claim, classify support:
   - directly supported
   - partly supported
   - weak proxy support
   - unsupported
3. Check for common problems:
   - citation absent on non-obvious claim
   - source does not match the strength of the sentence
   - citation stack where all sources say roughly the same thing
   - outdated citation for a fast-moving area
   - standard, report, or manual cited as if it were peer-reviewed evidence
   - bibliography metadata inconsistency
4. Recommend the smallest safe fix:
   - weaken wording
   - add a better citation
   - split one strong claim into two narrower claims
   - remove the claim

## Output shape

Prefer a table with:

- claim snippet
- current citation
- support rating
- issue
- recommended fix

## Guardrails

- Do not invent missing references.
- Distinguish peer-reviewed support, standards support, and background context support.
- Prefer conservative wording over unsupported certainty.
- Separate citation hygiene from conceptual disagreement; a claim can be interesting and still not yet be supported.
