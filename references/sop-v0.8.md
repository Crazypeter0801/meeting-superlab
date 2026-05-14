# AI-Assisted Product Design SOP v0.8

Use this reference when the user wants Meeting Superlab to follow the stronger product/design SOP from the internal PDF.

## Six-Step Flow

1. Problem definition: answer Q1-Q3 before any solution work.
2. Competitor research: study how the market solves the same problem and extract positive and negative lessons.
3. Creative divergence: generate 2-3 meaningfully different candidate solutions without letting AI overwrite product judgment.
4. Solution convergence: use a trade-off matrix to choose one direction and record why the others were not chosen.
5. Prototype demo handoff: turn the chosen direction into key low-fidelity pages for internal review and design discussion.
6. PRD + AI Check: product writes PRD v0.5 first, AI checks it, product accepts/rejects each finding, and PRD v1 records accepted changes.

## Step 1 Problem Definition

The three required questions:

- Q1: Whose specific problem are we solving, in what scenario, and at which stuck point?
- Q2: What happens if we do nothing? Prove the current cost, not the future benefit of a proposed solution.
- Q3: How will we know the problem is solved? Include positive metrics, negative metrics, kill criteria, and qualitative experience standards.

Quality bar:

- Q1 is invalid if it only says "improve experience" or "complete a feature".
- Q2 should describe current loss, risk, missed value, operational cost, or user harm.
- Q3 should include both quantitative and qualitative evidence.
- Kill criteria should eventually become `[time window] + [specific metric] + [trigger action]`.
- After AI challenges the answers, the product owner must mark each challenge as accepted, rejected, or pending.

## Step 2 Competitor Research

Start with constraints:

- User group.
- Interaction pattern.
- Product tone.
- Business or product goal.

Group references:

- A: direct benchmark. Similar users, interaction pattern, tone, and goal. Analyze deeply.
- B: related reference. Not fully comparable, but useful for a specific module or mechanism.
- C: industry benchmark. Mature pattern from a different context; extract principles carefully.

One competitor card should include:

- Basic information: product, function, 1-2 sentence positioning.
- Core mechanism: full user path from entry to completion.
- Key design points: 3-5 design decisions with concrete placement, copy, state, behavior, rationale, and value.
- Data and feedback: adoption, participation, reviews, complaints, incidents, or negative cases when available.
- Implications: mark each point as borrow, localize, or avoid; map it back to the Step 1 problem.

AI may propose and structure competitors, but product/design must verify details manually, especially screenshots and logged-in flows.

## Step 3 Creative Divergence

Recommended discipline:

- Start with 30 minutes of independent thinking before asking AI for ideas when the schedule allows.
- Use 5 Whys and reach at least Why 3.
- Produce rough initial directions before AI challenge.

Divergence prompts:

- Replace: replace a core element of the current solution.
- Reverse: reverse user behavior, incentive target, or process order.
- Borrow: ask how a very different industry, such as games, logistics, or finance, would solve the same problem.

AI challenge should run in three rounds:

- Problem layer: is the understanding of the core problem deep enough?
- Solution layer: what tradeoff feels most uncomfortable, and what can Tencent Meeting do that competitors cannot?
- Risk layer: if the idea fails in three months, what is the most likely cause?

Each challenge needs a clear product decision: keep, drop, or partially adopt.

## Step 4 Solution Convergence

Use a five-dimension trade-off matrix. Do not rely on numeric scores alone; each cell needs a concrete explanation.

Dimensions:

- Simplicity: path length, cognitive cost, implementation path.
- Cost: engineering effort, timing, cross-team dependency.
- Benefit: short-term conversion/revenue/retention effect and long-term value ceiling.
- Extensibility: whether v1 can evolve into the longer-term shape, or whether it becomes a dead end.
- Risk: compliance, complaints, financial loss, trust, brand, or operational risk.

Decision path:

1. Remove candidates with multiple hard red flags.
2. Return to Step 1 Q3 to identify the decisive dimension.
3. If remaining options are close, decide whether extensibility can be preserved with explicit v1 constraints.

Output:

- Trade-off matrix.
- Decision record: why the chosen option beats the alternatives.
- Preserved strengths from rejected options.
- v1 extensibility constraints when choosing a lighter solution.

## Step 5 Prototype Demo Handoff

The prototype is for internal review and product/design discussion. It should prioritize flow, states, and decision points over visual polish.

Minimum useful output:

- Key pages or panels.
- Entry point.
- Happy path.
- Important branches: empty, error, permission, weak-network, role switching, or cross-device states when relevant.
- Short explanation of what reviewers should judge.

## Step 6 PRD + AI Check

Product should write PRD v0.5 first. AI should check, not replace product thinking.

Standard PRD modules:

- Revision record.
- Problem to solve.
- Solution logic.
- Scenario and product-line compatibility.
- Onboarding.
- Metrics.
- Grey release and experiment logic.
- Kill criteria.
- Weak-network behavior.
- Data reporting.
- Security or compliance self-check.

Default AI Check items:

1. Main path simplicity.
2. Branch completeness.
3. Onboarding.
4. Platform compatibility.
5. Multi-language copy.
6. Large font mode.
7. Dark mode.
8. Weak-network behavior.
9. Grey release and A/B experiment logic.
10. Monitoring and data metrics.
11. Kill criteria completeness.

AI Check output has two parts:

- Check report: rating and concrete findings for each item.
- Multi-language copy table: scan all user-visible copy and draft simplified Chinese, English, and traditional Chinese.

Accepted AI Check findings should be written into the PRD revision record. A v0.5 and v1 with no substantive difference usually means the check was not useful enough.

## Review Rhythm

- Self-check and AI Check should happen before leader review.
- AI red findings should go back to product/design for revision before taking leader time.
- Leader review should focus on product judgment, tradeoffs, prioritization, and decision quality.
