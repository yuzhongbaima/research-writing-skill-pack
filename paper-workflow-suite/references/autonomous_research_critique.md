# Autonomous Research Critique

This reference distills what is worth borrowing from modern autonomous research systems such as AutoResearchClaw, and what should not become the default for serious engineering papers.

Relevant source repository:

- [aiming-lab/AutoResearchClaw](https://github.com/aiming-lab/AutoResearchClaw)

## What to borrow

### 1. Stage-based orchestration

The strongest idea is not "one prompt, one paper". It is explicit decomposition:

- scoping
- literature search
- screening
- synthesis
- hypothesis generation
- experiment design
- execution
- analysis
- drafting
- review
- export

This is useful because it makes failure visible and lets the human intervene before a weak early decision contaminates the whole paper.

### 2. Human-in-the-loop gates

AutoResearchClaw's newer direction is itself evidence that full autonomy is not enough. The project now emphasizes configurable intervention modes and gate stages rather than pure no-touch execution.

For our workflow, the essential gates are:

1. literature screening gate
2. experiment or validation design gate
3. result interpretation gate
4. final claim and submission gate

### 3. Claim verification and anti-fabrication

This is highly worth adopting.

Useful mechanisms:

- extract claims from draft text
- map each claim to evidence artifacts
- flag unsupported numbers
- distinguish direct support from weak proxy support
- kill citations that do not survive verification

### 4. Artifact-first execution

Research automation is much safer when every important output has a file-backed trace:

- search queries
- included papers
- experiment code
- result tables
- charts
- review notes

This should become standard in our workflow.

### 5. Branching before commitment

Branching alternative hypotheses or experimental directions early is useful. It is cheaper and safer than overcommitting to one story and discovering too late that it does not hold.

## What to adapt rather than copy

### 1. Literature retrieval

The idea of multi-source retrieval is good, but retrieval alone is not enough.

We should adapt it into:

- search strategy log
- inclusion and exclusion criteria
- manual reading of the final core paper set
- explicit labeling of source type and evidence tier

For engineering fields, standards, reports, manuals, and peer-reviewed articles must not be merged into one undifferentiated citation pool.

### 2. Automatic execution

Automatic execution is useful for:

- running scripts repeatedly
- collecting metrics
- generating standardized plots
- checking environment reproducibility

But it must be constrained by:

- execution manifests
- fixed baselines
- frozen evaluation settings
- human review of abnormal outputs
- explicit distinction between simulation, experiment, and field validation

### 3. Forced constraints

Forced constraints are valuable when they prevent bad science rather than merely forcing the pipeline to continue.

Good constraints:

- required human gate before expensive execution
- required evidence mapping before strong claims
- required artifact manifest before paper drafting
- required limitation note before final polishing

Bad constraints:

- forcing a paper draft to continue when evidence is immature
- auto-approving weak literature because the stage needs to move on
- treating low-confidence generated results as publication material

## What to reject

### 1. "One topic in, one paper out" as the default mental model

This is good marketing, but not a safe default for high-level research.

For serious journal work, the product is not a paper-shaped artifact. The product is a defensible contribution with traceable evidence.

### 2. Simulated or synthetic results as paper-ready evidence

If a system supports simulated mode for framework debugging, that can be useful operationally. It should not quietly leak into publication-grade claims.

For our workflow:

- simulated mode is allowed for pipeline debugging
- simulated mode is not allowed as hidden support for journal claims
- any simulation-only study must be labeled as such and framed conservatively

### 3. Writing polish before scientific maturity

Autonomous systems often make this tempting because drafting is easy.

We explicitly reject the order:

topic -> draft -> retrofit evidence

We prefer:

topic -> evidence -> gate -> method -> result -> gate -> draft

## Nature Communications standard

If the target is around the level of Nature Communications, the human role becomes even more important.

At that level, the workflow should assume:

- no fully autonomous greenlight to submission
- stronger skepticism toward overgeneralized claims
- higher expectation of methodological and evidential transparency
- tighter integration between results, limitations, and interpretation
- more visible demand for novelty plus credibility, not novelty theater

## Operational policy for our suite

We therefore adopt this policy:

1. use automation to widen search, speed execution, and standardize records
2. use human judgment to approve literature scope, experiment design, claim strength, and venue fit
3. never let the pipeline's convenience overrule scientific defensibility
