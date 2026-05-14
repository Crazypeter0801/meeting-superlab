---
name: figma-handoff
description: Figma handoff workflow for Meeting Superlab. Use after a product/design solution direction has converged and a low-fidelity demo scope is selected, when the user wants the proposal drawn in Figma, provides a Figma file/node link, or asks to turn Meeting Superlab outputs into Figma frames, wireframes, flows, output images, or review-ready low-fidelity screens. Also use when the user asks 是否可以画出来, 出图, 画到 Figma, 低保真稿, 原型图, or 可视化方案.
---

# Figma Handoff

## Goal

Bridge Meeting Superlab exploration into a Figma draft without making Figma work automatic or premature.

## Gate

Ask whether the user wants the selected direction drawn in Figma after there is:

- a clear user/scenario frame,
- a selected solution direction,
- a decision record or explicit fast-draft exception,
- a demo scope,
- key screens/states,
- and a low-fidelity demo prompt or equivalent outline.

Do not create or modify Figma files before the user confirms and provides a Figma link or asks to create a new file.

When Figma is not yet possible because the user has not provided a link, say so and offer a low-fidelity page structure or demo prompt as the immediate fallback.

## Ask For

If the user wants Figma output, ask for:

- Figma file or node URL.
- Desired target: append new page, add frames near an existing node, or update an existing draft.
- Fidelity: black-white wireframe, structured low-fidelity UI, or closer-to-product visual draft.
- Frame scope: tiny flow, review-ready flow, or concept flow.
- Whether to reuse an existing Tencent Meeting design system/component area in the file.

## Figma Plugin Workflow

When using Figma tools, follow the available Figma plugin/skill requirements in the current environment.

- Load the required Figma-use skill before calling Figma write tools when the environment instructs it.
- If a Figma URL is provided, parse file key and node id according to the Figma workflow.
- Prefer creating low-fidelity frames first: clear layout, labels, states, and flow notes.
- Reuse existing design system components when available; otherwise use simple neutral wireframe primitives.
- Do not over-polish visual style unless the user explicitly requests it.

## Draft Content

For each frame include:

- Frame title.
- User goal.
- Key content blocks.
- Primary action.
- Secondary action or escape path.
- Important state label: normal, empty, permission, error, external guest, cross-device, or AI trust/source state.
- SOP note when useful: which Step 1 problem and Step 4 decision the frame supports.

## Output

Before writing to Figma, summarize:

- Frames to create.
- States included.
- Source solution direction.
- Open assumptions.

After writing to Figma, report:

- Figma file/page/node affected.
- What frames were created or updated.
- Whether a `visual-polish` pass is recommended before stakeholder review.
- What still needs product/design review.
