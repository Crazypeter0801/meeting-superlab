---
name: solution-convergence
description: Converge Tencent Meeting product/design candidate solutions using the Meeting Superlab Step 4 trade-off matrix. Use after creative divergence when the team has 2-3 candidate solutions and needs a five-dimension comparison, decision path, selected v1 direction, preserved rejected-option strengths, v1 extensibility constraints, and a decision record before prototype/demo or PRD work.
---

# Solution Convergence

## Goal

Choose a v1 direction through explicit tradeoffs. This step is decision work, not PRD writing and not visual design.

Use this after `solution-exploration` has produced 2-3 candidate solutions.

## Preconditions

Confirm there is:

- Step 1 problem definition, especially Q3 metrics and kill criteria.
- 2-3 candidate solutions with core mechanisms.
- Known constraints, dependencies, and risk concerns.

If there is only one candidate, ask whether to quickly generate alternatives first. If Q3 is missing, return to `need-framing` before making a confident decision.

## Trade-Off Matrix

Use five dimensions:

- Simplicity: user path length, cognitive cost, implementation path.
- Cost: engineering effort, timing, and cross-team dependency.
- Benefit: short-term effect and long-term value ceiling.
- Extensibility: whether v1 can evolve into the longer-term shape.
- Risk: compliance, complaints, financial loss, trust, brand, operational, privacy, or AI-risk exposure.

Each cell must contain a concrete explanation. Avoid numeric scoring without explanation.

## Decision Path

1. Identify hard red flags. A candidate with multiple hard red flags should usually be removed.
2. Return to Step 1 Q3 and choose the decisive dimension for this iteration.
3. If remaining candidates are close, prefer the one that preserves future extensibility with explicit v1 constraints.

## Output

Provide:

- Five-dimension trade-off matrix.
- Decision path summary.
- Recommended v1 direction.
- Why the chosen direction beats the alternatives.
- Strengths to preserve from rejected directions.
- v1 extensibility constraints if choosing a lighter solution.
- Risks that must be checked in prototype or PRD.
- Recommended next skill: `demo-and-review` or `prd-ai-check`.
