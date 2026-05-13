---
name: solution-exploration
description: Generate and compare product/design solution directions for Tencent Meeting or meeting/collaboration needs after framing and competitor-informed insight synthesis. Use when the team needs 2-3 divergent directions, tradeoffs, recommendation logic, user flows, key states, and validation questions before demo creation.
---

# Solution Exploration

## Goal

Create a small set of useful solution directions that product and design can discuss, not a single overconfident answer.

Work step by step. Do not both generate directions and fully develop demo material in the same response unless the user explicitly asks for a one-pass draft.

## Preconditions

Before solution exploration, confirm there is at least:

- A need frame.
- Some competitor, screenshot, user, or product context.
- Known assumptions and constraints.

If user role, meeting stage, current pain point, or desired outcome is still unclear, return to `need-framing` and ask clarification questions instead of generating directions.

If competitor context is missing and the decision would benefit from it, run `competitor-research` first.

## Direction Set

Default to 3 directions:

- Conservative optimization: improve the existing path with minimal structural change.
- Experience restructuring: change flow, hierarchy, or interaction model.
- Exploratory AI/collaboration direction: introduce a more proactive, AI-assisted, or social/collaboration-forward pattern when appropriate.

For each direction include:

- Core idea.
- 3-5 sentence user flow summary.
- Key screens or states at a high level.
- Borrowed competitor lesson.
- Pros.
- Cons.
- Validation questions.

After presenting directions, recommend one and ask the user which direction to deepen. Wait before producing detailed flows, demo prompts, or review material.

## Recommendation

Recommend one direction only after comparing:

- Fit to user problem.
- Evidence from competitors or screenshots.
- Complexity and dependencies.
- Risk around privacy, permissions, trust, and cross-device consistency.
- Suitability for low-fidelity demo discussion.

## Output

End with a direction comparison and a clear handoff to `demo-and-review`.
