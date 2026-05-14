---
name: solution-exploration
description: "Generate 2-3 meaningfully different product/design candidate solutions for Tencent Meeting or meeting/collaboration needs after framing and competitor-informed insight synthesis. Use for Step 3 creative divergence: 5 Whys, replace/reverse/borrow prompts, AI challenge rounds, candidate solution cards, early flows, key states, and validation questions before tradeoff convergence."
---

# Solution Exploration

## Goal

Create a small set of useful candidate solutions that product and design can discuss, not a single overconfident answer.

Work step by step. Do not both generate directions and fully develop demo material in the same response unless the user explicitly asks for a one-pass draft.

This is Step 3 of the SOP. It is for divergence, not final decision.

## Preconditions

Before solution exploration, confirm there is at least:

- A need frame.
- Some competitor, screenshot, user, or product context.
- Known assumptions and constraints.

If user role, meeting stage, current pain point, or desired outcome is still unclear, return to `need-framing` and ask clarification questions instead of generating directions.

If competitor context is missing and the decision would benefit from it, run `competitor-research` first.

## Divergence Discipline

When the user is doing a formal SOP run, encourage:

- Independent thinking first: the product/design owner writes rough thoughts before AI expands them.
- 5 Whys: reach at least Why 3 for the core problem.
- 3 divergence prompts: replace, reverse, borrow.
- AI challenge in rounds, with explicit keep/drop/partially-adopt decisions.

If the user asks for a fast pass, you may simulate the structure, but label it as an assumption-driven draft.

## 5 Whys

Ask why the issue happens, why the mechanism produces it, and why the mechanism exists. Why 4 and Why 5 are optional deeper exploration.

The goal is to expose the root mechanism, not to create wordplay.

## 3 Divergence Prompts

- Replace: replace a core element of the current path or mechanism.
- Reverse: reverse user behavior, incentive target, flow order, or responsibility.
- Borrow: ask how a different industry such as games, logistics, finance, education, or creator tools would solve the problem.

## AI Challenge Rounds

Challenge one round at a time when interacting with the user:

- Round 1, problem layer: is the understanding of the core problem deep enough?
- Round 2, solution layer: what is the most uncomfortable tradeoff, and what can Tencent Meeting do that competitors cannot?
- Round 3, risk layer: if this fails in three months, what is the most likely cause?

Ask the user to decide keep, drop, or partially adopt for important challenges.

## Candidate Set

Default to 3 directions:

- Conservative optimization: improve the existing path with minimal structural change.
- Experience restructuring: change flow, hierarchy, or interaction model.
- Exploratory AI/collaboration direction: introduce a more proactive, AI-assisted, or social/collaboration-forward pattern when appropriate.

For each direction include:

- Core mechanism in one sentence.
- 3-5 sentence user flow summary.
- Key screens or states at a high level.
- Borrowed competitor lesson.
- Pros.
- Cons.
- Main tradeoff.
- Source: original thought, replace/reverse/borrow, competitor lesson, or AI challenge.
- Validation questions.

After presenting candidate solutions, ask which candidates should enter `solution-convergence`. Wait before producing detailed flows, demo prompts, or review material.

## Recommendation

Do not make the final recommendation in this skill unless the user explicitly asks for a lightweight one-pass answer. The formal recommendation belongs in `solution-convergence`.

If making a lightweight recommendation, compare:

- Fit to user problem.
- Evidence from competitors or screenshots.
- Complexity and dependencies.
- Risk around privacy, permissions, trust, and cross-device consistency.
- Suitability for low-fidelity prototype discussion.

## Output

End with:

- 5 Whys summary.
- Replace/reverse/borrow divergence.
- AI challenge decisions when available.
- 2-3 candidate solution cards.
- Questions to clarify before convergence.
- Clear handoff to `solution-convergence`.
