---
name: meeting-design-review
description: Run a structured product and UI quality review for Tencent Meeting mobile designs, Open Design artifacts, Figma frames, screenshots, or prototype prompts. Use before presenting a draft, after mobile-prototype-artifact, after visual-polish, or when the user asks whether a Tencent Meeting design is ready for review.
---

# Meeting Design Review

## Goal

Catch product, trust, visual, and delivery problems before a Tencent Meeting mobile design goes into review.

This is a quality gate, not a replacement for product judgment. Be direct about risks and missing evidence.

## When To Use

Use this skill when the user provides or asks to review:

- Mobile screens.
- Figma frames.
- Open Design artifacts.
- HTML prototypes.
- Image drafts.
- Prototype prompts.
- Visual polish output.

If there is no artifact or prompt, ask for one or route to `mobile-prototype-artifact`.

## Review Order

1. Product fit: user, scenario, pain, outcome, and meeting stage are visible.
2. Meeting context: the design respects live meeting pressure, attention limits, and role differences.
3. Trust and privacy: AI, recording, transcript, external guest, camera, mic, and screen sharing are explicit.
4. Visual system: Tencent Meeting Apple-like system is applied without decorative noise.
5. Interaction and states: normal, loading, empty, error, permission, weak-network, and role-limited states exist.
6. Accessibility: hit targets, contrast, text scaling, readable copy, and focus order.
7. Delivery readiness: the output is specific enough for Figma, prototype, PRD, or engineering review.

## Quality Bar

Read `references/quality-checklist.md` for detailed checks.

High-quality Tencent Meeting mobile drafts should feel:

- Calm under time pressure.
- Clear about who can do what.
- Honest about sensitive meeting states.
- Efficient for repeated enterprise use.
- Native enough to feel at home on iOS and Android.
- Distinct enough to remain Tencent Meeting.

## Output

Provide:

- Verdict: ready, revise, or blocked.
- Top 5 findings, ordered by severity.
- Product risks.
- Visual and design-system fixes.
- State and edge-case gaps.
- Accessibility issues.
- Concrete next actions.
- Suggested handoff: revise prompt, update Figma, run visual polish, or run PRD AI Check.

If there are no major issues, say so clearly and name the remaining risks.
