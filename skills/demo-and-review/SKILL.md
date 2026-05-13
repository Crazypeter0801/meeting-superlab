---
name: demo-and-review
description: Prepare low-fidelity demo prompts and review material for Tencent Meeting product/design exploration. Use when a solution direction needs to become a black-and-white prototype prompt, page/state outline, discussion artifact, product/design/engineering review checklist, or next-day working-session material.
---

# Demo And Review

## Goal

Turn a direction into a practical artifact for discussion. The output should help product and design review the idea, not pretend to be final UI.

## Preconditions

Before creating a demo prompt, confirm there is a clear user role, scenario, core flow, and recommended direction. If these are missing, ask clarification questions or return to `need-framing` / `solution-exploration`.

## Step-by-Step Gate

Before producing the final demo prompt, offer 2-3 demo scope options with pros, cons, and a recommendation. Wait for user selection unless they already specified the scope.

Default scope options:

- Tiny flow demo: 1 entry point + 1 core screen + 1 key state. Pros: fastest for discussion. Cons: may miss edge cases.
- Review-ready flow: entry point + core path + empty/error/permission state. Pros: best default for product/design review. Cons: slightly more work.
- Concept demo: broader exploratory flow with AI/collaboration behavior. Pros: good for vision discussion. Cons: easier to drift from feasibility.

## Demo Prompt Defaults

- Black-and-white / low-fidelity first.
- Focus on structure, flow, states, and decision points.
- Avoid polished visual style unless requested.
- Use concise meeting-product copy.
- Include normal, empty, permission/error, and cross-role states when relevant.
- Borrow interaction lessons from competitors without copying visual identity.

## Required Demo Prompt Content

- Goal.
- User role and scenario.
- Entry point.
- Core flow.
- Screens or panels.
- Key controls.
- Important states.
- Data/content examples.
- Constraints and exclusions.
- Review focus.

## Review Package

Provide:

- Requirement understanding.
- Evidence used.
- Recommended direction.
- Demo prompt.
- Figma handoff question: ask whether the user wants this drawn in Figma, and invite them to provide a Figma file or node link.
- Product questions.
- Design questions.
- Engineering/platform questions.
- Evidence still missing.
- Suggested next iteration.

Use `../../references/templates.md` for copyable structures.
