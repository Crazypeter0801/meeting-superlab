---
name: superlab-workflow
description: Entry skill for Meeting Superlab. Use when a product manager or designer wants to explore a Tencent Meeting or meeting/collaboration product need with AI, decide which Meeting Superlab skill to use, or run the full product-design workflow from rough input to clarification questions, competitor research, insights, solution directions, demo prompt, and review material. When the need is vague, this skill must ask targeted follow-up questions before doing competitor research or solution work. At major decision points, present 2-3 options with pros, cons, and a recommendation, then wait for the user before continuing.
---

# Superlab Workflow

## Purpose

Guide product and design work through the Meeting Superlab loop:

`need-framing -> competitor-research -> screenshot-analysis -> insight-synthesis -> solution-exploration -> demo-and-review -> figma-handoff -> pd-review-panel`

Use this skill as the router and process owner. Keep the work moving, but do not skip evidence-gathering before proposing confident solutions.

## Interaction Style

Work like a product/design workshop facilitator, not a one-shot answer generator.

- Proceed one stage at a time.
- At each major decision point, present 2-3 options with pros, cons, and your recommendation.
- Ask the user to choose or confirm before doing the next substantial stage.
- Keep each stage output compact enough for discussion.
- If the user explicitly asks for a full pass in one go, you may continue, but still label assumptions and decision points.

Major decision points include:

- Which user/scenario frame to focus on.
- Which competitor research route to use.
- Which insight/opportunity areas to pursue.
- Which solution direction to deepen.
- Which demo scope to prepare.
- Whether to draw the selected direction in Figma.
- Whether to run a multi-perspective review panel.

## Routing

- Use `need-framing` when the need is vague, unstructured, or missing user/scenario/constraint details.
- Use `competitor-research` before solution exploration when the user needs external references or inspiration.
- Use `screenshot-analysis` when the user provides competitor screenshots, recordings, product captures, or notes.
- Use `insight-synthesis` after collecting need details, competitor observations, screenshots, user feedback, or product data.
- Use `solution-exploration` when there is enough context to generate 2-3 product/design directions.
- Use `demo-and-review` when the user needs a low-fidelity demo prompt, review doc, or next-day discussion material.
- Use `figma-handoff` after a solution direction and demo scope are selected, when the user may want the draft drawn into a Figma file or provides a Figma link.
- Use `pd-review-panel` when there is a draft need frame, competitor analysis, solution proposal, or demo prompt that needs multi-perspective critique.

## Hard Gates

- Do not force the need into a business category at the start.
- Do not continue from a vague input directly into research, solution generation, demo prompts, or review material.
- Do not generate final solution recommendations before the need is framed and competitor/context evidence is considered.
- Do not jump from a rough need directly to final review material unless the user explicitly asks for a one-pass draft.
- Do not invent competitor facts. Search current public sources, cite them, or ask the user for screenshots/notes.
- Do not make the early demo visually polished by default. Start low-fidelity and discussion-oriented.

## Clarification Gate

Before doing work, check whether the input contains enough signal for product/design judgment.

Treat the need as vague if it is missing 3 or more of these:

- User role.
- Meeting/collaboration stage.
- Current behavior or pain point.
- Desired outcome.
- Existing product context.
- Constraints or dependencies.
- Evidence or references.

If the need is vague, stop after a short restatement and ask 3-6 targeted questions. The questions should help decide user, scenario, pain point, constraints, evidence, and expected output. Do not answer the questions yourself.

Proceed only when:

- the user answers enough questions,
- the user explicitly says to proceed with assumptions, or
- the task is only to draft a question list/interview guide.

## Default Flow

1. Summarize the raw need in one short paragraph.
2. If the need is vague, ask clarification questions and wait.
3. Present 2-3 framing options if there are multiple plausible users/scenarios; wait for selection.
4. Present 2-3 competitor research routes; wait for selection unless the user already specified one.
5. Build competitor context from web sources or user-provided screenshots/notes.
6. Synthesize opportunity areas instead of listing features.
7. Generate 2-3 solution directions with tradeoffs; wait for the user to pick one to deepen.
8. Present 2-3 demo scope options; wait for selection.
9. Produce a low-fidelity demo prompt and review checklist.
10. Ask whether the user wants the selected direction drawn in Figma; if yes, ask for a Figma file/node link and use `figma-handoff`.
11. Ask whether to run a product/design/competitor/risk review panel.

## Output Contract

End full-flow work with:

- Requirement frame.
- Competitor evidence and implications.
- Key insights/opportunities.
- Solution direction comparison.
- Recommended next direction.
- Low-fidelity demo prompt.
- Figma handoff question or Figma draft plan when requested.
- Review questions and missing evidence.

Use `../../references/templates.md` for reusable output structures and `../../references/example-case.md` for a sample walkthrough.
