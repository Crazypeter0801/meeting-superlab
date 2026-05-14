---
name: demo-and-review
description: Prepare low-fidelity prototype prompts and review material for Tencent Meeting product/design exploration. Use for Meeting Superlab Step 5 when a converged solution direction needs to become key pages, black-and-white prototype prompts, page/state outlines, discussion artifacts, product/design/engineering review checklists, output images, or next-day working-session material. Also use when the user asks for 出图, 原型图, 低保真图, demo, wireframe, or a visual draft.
---

# Demo And Review

## Goal

Turn a direction into a practical artifact for discussion. The output should help product and design review the idea, not pretend to be final UI.

This is Step 5 of the SOP. It translates the selected direction into reviewable key pages and states.

## Preconditions

Before creating a demo prompt, confirm there is a clear user role, scenario, core flow, and recommended direction. If there is no trade-off decision record, route to `solution-convergence` first unless the user asks for a fast rough draft.

## Step-by-Step Gate

Before producing the final demo prompt, offer 2-3 demo scope options with pros, cons, and a recommendation. Wait for user selection unless they already specified the scope.

If the user says they want "出图" but has not provided a Figma link, offer low-fidelity image/prototype prompt first and ask whether to later hand off to Figma.

Default scope options:

- Tiny flow demo: 1 entry point + 1 core screen + 1 key state. Pros: fastest for discussion. Cons: may miss edge cases.
- Review-ready flow: entry point + core path + empty/error/permission/weak-network state. Pros: best default for product/design review. Cons: slightly more work.
- Concept demo: broader exploratory flow with AI/collaboration behavior. Pros: good for vision discussion. Cons: easier to drift from feasibility.

## Demo Prompt Defaults

- Black-and-white / low-fidelity first.
- Focus on structure, flow, states, and decision points.
- Avoid polished visual style unless requested.
- Use concise meeting-product copy.
- Include normal, empty, permission/error, and cross-role states when relevant.
- Include weak-network, role-switching, reward/entitlement delay, or cross-device states when the scenario can fail there.
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
- Decision record from `solution-convergence` when available.
- Demo prompt.
- Figma handoff question: always ask whether the user wants this drawn in Figma, and invite them to provide a Figma file or node link.
- Product questions.
- Design questions.
- Engineering/platform questions.
- Evidence still missing.
- Suggested next iteration.
- PRD readiness note: whether the prototype has enough structure to support `prd-ai-check`.

Use `../../references/templates.md` for copyable structures.
