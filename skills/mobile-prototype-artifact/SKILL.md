---
name: mobile-prototype-artifact
description: Convert a Tencent Meeting mobile product direction into reviewable mobile prototype screens, Open Design prompts, HTML artifact specs, or Figma generation prompts. Use after solution convergence or when the user asks for mobile screens, prototype artifact, Open Design prompt, iPhone frames, key states, or Tencent Meeting mobile visual drafts.
---

# Mobile Prototype Artifact

## Goal

Turn a selected Tencent Meeting mobile direction into a concrete, reviewable prototype artifact.

This skill adapts the artifact-first idea from Open Design into Meeting Superlab: define the screen set, states, design system constraints, and output contract before asking an agent or design tool to render UI.

## Preconditions

Confirm the work has:

- User role.
- Meeting stage.
- Core flow.
- Recommended direction.
- Constraints or assumptions.

If these are missing and the user did not request a fast rough draft, route to `need-framing` or `solution-convergence` first.

## Scope Options

Before producing the final prompt, offer 2-3 scope options unless the user already specified scope:

- Tiny mobile demo: entry plus core screen plus one key state. Fastest for discussion.
- Review-ready mobile flow: entry, core path, permission/error/empty state, and role difference. Best default.
- System exploration: 4-6 screens showing component patterns and visual language. Best when validating the new design system.

Recommend review-ready mobile flow for Tencent Meeting product review.

## Design System Gate

If the user mentions Tencent Meeting latest design system, Apple-like style, or iOS-like mobile design, first apply `tencent-meeting-mobile-design-system`.

Use official Tencent Meeting Figma library or screenshots if provided. Otherwise label the token set as provisional.

## Artifact Prompt Contract

Read `references/artifact-contract.md` when generating an Open Design or HTML prompt.

The prompt must specify:

- Output format.
- Viewport and device frame.
- Screen count and names.
- Screen-by-screen content.
- Interaction and state requirements.
- Token and component rules.
- Exclusions.
- Review focus.

## Screen Pattern Selection

Read `references/screen-patterns.md` when choosing screens.

Common Tencent Meeting mobile sets:

- Pre-meeting: home, meeting detail, join lobby, permission prompt.
- In-meeting: video canvas, controls dock, participants, chat, AI summary, captions, share.
- Post-meeting: summary, transcript, action items, sharing, follow-up.
- Admin or enterprise: permissions, policy blocks, recording, guest control.

## Output Modes

### Open Design Prompt

Output a copyable prompt for Open Design:

- Tell the user to choose `mobile-app` or a mobile prototype skill.
- Tell the user to choose the Tencent Meeting design system if available.
- Include the full artifact prompt.

### Figma Prompt

Output a Figma-ready generation prompt:

- Screen inventory.
- Auto layout requirements.
- Component states.
- Token rules.
- Naming conventions.

### HTML Artifact Prompt

Output a single-file HTML prototype prompt:

- Multiple iPhone frames on one canvas.
- CSS tokens.
- Static states only unless motion is requested.
- No external assets unless provided.

## Required Output

Provide:

- Requirement recap.
- Selected scope.
- Screen inventory.
- State inventory.
- Design system assumptions.
- Copyable prototype prompt.
- Review checklist.
- Handoff: Figma, visual polish, or design review.
