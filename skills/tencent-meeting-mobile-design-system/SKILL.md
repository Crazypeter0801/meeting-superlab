---
name: tencent-meeting-mobile-design-system
description: Apply or define the Tencent Meeting mobile design system for iOS-like, Apple-inspired product UI. Use when the user mentions Tencent Meeting latest design system, Apple-like style, mobile UI tokens, iOS visual language, meeting components, privacy states, Figma prompts, or visual rules for Tencent Meeting mobile screens.
---

# Tencent Meeting Mobile Design System

## Goal

Translate Tencent Meeting mobile product work into a calm, Apple-like design language without copying iOS blindly.

Apple-like means content first, low chrome, semantic color, clear hierarchy, system-native motion, strong accessibility, and privacy-respecting interaction. Tencent Meeting still needs its own meeting-product identity: trustworthy, efficient, low-interruption, enterprise-ready, and cross-platform.

If an official Tencent Meeting design system, Figma library, screenshot set, or token file is available, use that as source of truth. Otherwise use the provisional rules below and label them as assumptions.

## When To Use

Use this skill for:

- Tencent Meeting mobile screens, iOS screens, Android screens, and cross-platform mobile flows.
- Requests for the latest Tencent Meeting design system, Apple-like UI, or HIG-style polish.
- Building prompts for Open Design, Figma, HTML prototypes, image generation, or visual review.
- Defining mobile tokens, meeting components, permission states, AI meeting surfaces, and in-meeting controls.

Do not use this skill to skip product framing. If the user need is vague, route through `need-framing` first.

## Design Stance

1. Content over decoration: meeting content, people, status, and next action should beat brand ornament.
2. Calm hierarchy: use neutrals, subtle separators, and a single meaningful blue accent.
3. Low interruption: in-meeting prompts should be compact, deferrable, and reversible.
4. Trust by design: recording, AI summary, transcript, camera, mic, and external-guest states must be explicit.
5. Native feeling: respect safe areas, Dynamic Type, hit targets, platform materials, and familiar navigation.
6. Enterprise clarity: copy should be short, precise, and confidence-building.

## Provisional Token Direction

Read `references/mobile-tokens.md` when generating or auditing concrete UI.

Core defaults:

- Canvas: iPhone 15/16 class frame, 393 x 852 or 390 x 844, with safe areas.
- Font stack: PingFang SC, SF Pro, system UI. Use tabular numbers for durations and counters.
- Main accent: Tencent meeting blue as the primary action and active state.
- Radius: restrained for list items and cards, larger only for sheets and system-like panels.
- Shadows: very soft; prefer separators and materials over heavy elevation.
- Motion: small spatial transitions, no decorative motion during active meetings.

## Component Coverage

Read `references/meeting-components.md` when the output includes specific screens.

Always consider:

- Meeting lobby, joining, waiting room, and permission priming.
- In-meeting video canvas, participant strip, active speaker, subtitle/transcript, controls dock.
- Bottom sheets for people, chat, share, AI summary, captions, settings, and reactions.
- Privacy and trust banners for recording, AI, external guests, camera, mic, screen sharing.
- Weak network, reconnecting, device switch, role change, no permission, and host controls.

## Output Modes

### Token Mode

When the user asks for a design system or token guidance, output:

- Design stance.
- Token table: color, typography, spacing, radius, shadow, materials, motion.
- Component rules.
- Accessibility rules.
- Assumptions and missing official inputs.

### Prompt Mode

When the user wants Open Design, Figma, HTML, or image-generation prompts, output:

- A short visual direction.
- Required viewport and frame rules.
- Token rules.
- Component/state rules.
- A copyable prompt.

### Audit Mode

When the user provides a screenshot, Figma frame, or generated UI, output:

- Verdict: aligned, partially aligned, or off-system.
- Top fixes by impact.
- Token corrections.
- Component and state corrections.
- Accessibility and trust risks.

## Handoffs

- Use `mobile-prototype-artifact` when this design system should become mobile screens or an Open Design prompt.
- Use `visual-polish` when an existing draft needs better hierarchy and product-grade finish.
- Use `meeting-design-review` when the draft needs a structured QA pass before review.
