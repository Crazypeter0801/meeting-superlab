---
name: need-framing
description: Frame rough product/design needs for Tencent Meeting or meeting/collaboration experiences using the Meeting Superlab problem-definition gate. Use when the input is a vague feature idea, meeting note, user pain point, PRD excerpt, screenshot, or request that needs clarified Q1/Q2/Q3, users, scenarios, pain points, outcomes, constraints, assumptions, metrics, kill criteria, and missing information before competitor research or solution exploration. Must ask targeted clarification questions when key framing details are missing.
---

# Need Framing

## Goal

Turn a rough need into a clear product-design problem frame without prematurely classifying it into yearly goals or forcing a solution.

This is Step 1 of the SOP. It defines the problem; it does not design the answer.

## Extract

- User roles: host, participant, external guest, enterprise admin, creator, operator, or other.
- Stage: before meeting, during meeting, after meeting, cross-device, admin/management, or asynchronous collaboration.
- Current behavior: what users do today and where friction appears.
- Pain point: what is inefficient, confusing, risky, untrusted, or costly.
- Desired outcome: what should become faster, clearer, safer, more discoverable, or more valuable.
- Current cost if nothing changes: user harm, lost value, operational cost, business risk, trust risk, or missed opportunity.
- Measurement: positive metrics, negative metrics, qualitative success standard, and kill criteria.
- Constraints: platform, permissions, privacy, compliance, audio/video, IM, recording, AI summary, cross-device, release timing, dependency teams.
- Evidence: user feedback, data, support issues, screenshots, competitor examples, internal discussion notes.
- Unknowns: missing details that materially affect solution direction.

## Question Discipline

Ask focused follow-up questions when the answer would change the next step. For a vague need, asking is the deliverable for this step.

Do not silently fill major gaps with assumptions. Only group minor unknowns into "assumptions for now" after user role, stage, pain point, desired outcome, and at least one constraint or evidence source are reasonably clear.

Ask 3-6 questions at a time. Prefer questions that are easy for product/design partners to answer.

## Problem-Definition Gate

Before moving to competitor research or solution exploration, try to answer:

- Q1: Whose specific problem are we solving, in what scenario, and at which stuck point?
- Q2: What happens if we do nothing? Describe current cost, not the benefit of a preferred solution.
- Q3: How will we know the problem is solved? Include positive metrics, negative metrics, kill criteria, and qualitative standards.

If the user cannot answer Q2 or Q3 yet, ask for the best available proxy evidence rather than inventing numbers.

When challenging a draft problem definition, check:

- Is Q1 concrete enough to show person, scenario, and stuck point?
- Does Q2 prove the current cost of inaction?
- Does Q3 contain both quantitative and qualitative standards?
- Do the metrics in Q3 truly validate the problem in Q1?
- Are the kill criteria stated as a time window, specific metric, and trigger action when possible?

For every challenge, ask the user to mark it as accepted, rejected, or pending when the step is being formalized for PRD work.

Good clarification questions include:

- Who is the primary user in this scenario: host, participant, external guest, enterprise admin, or someone else?
- Does the problem happen before, during, after the meeting, or across multiple stages?
- What is the current user path or product behavior today?
- What pain are we solving: efficiency, understanding, trust, control, collaboration, conversion, or something else?
- What would count as a better outcome for the user or team?
- If we do nothing, what cost or risk remains: user loss, complaints, operational burden, lost conversion, trust damage, or missed strategic value?
- What metrics would prove success, and what negative signal would force us to stop or roll back?
- What constraints should we respect: permissions, privacy, AI accuracy, cross-device consistency, enterprise admin rules, release timing, or existing components?
- Do we have screenshots, user feedback, data, PRD notes, or competitor examples?
- What do you want from this round: clarification only, competitor analysis, solution directions, demo prompt, or review material?

Do not ask the user to classify the need as business growth, technical experience, or 2C exploration at the beginning. Add that mapping later only when the user needs alignment material.

If the user asks to proceed despite missing details, clearly label assumptions before continuing.

## Output

Provide:

- One-paragraph need summary.
- Problem frame.
- Q1/Q2/Q3 answer or draft.
- AI challenge points with accepted/rejected/pending status when formalizing the need.
- Primary users and stages.
- Known constraints.
- Assumptions.
- Missing evidence.
- Clarification questions if the need is still vague.
- Recommended next skill, usually `competitor-research` or `screenshot-analysis`.
