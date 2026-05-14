# Mobile Artifact Contract

Use this contract when producing an Open Design or HTML artifact prompt.

## Required Prompt Shape

1. Context
   - Product: Tencent Meeting mobile.
   - Platform: iOS-first mobile, cross-platform aware.
   - User role and meeting stage.
   - Core problem and desired outcome.

2. Output
   - Produce 3-5 mobile screens.
   - Use 393 x 852 iPhone frames.
   - Show each screen as a separate named frame.
   - Include status bar and home indicator placeholders.
   - Keep the output static unless interaction is explicitly requested.

3. Design system
   - Apply Tencent Meeting Apple-like mobile design system.
   - Use calm neutral surfaces, one primary blue, semantic status colors.
   - Use PingFang SC or SF Pro style typography.
   - Respect safe areas and 44 px minimum hit targets.
   - Avoid decorative gradients, blobs, and marketing-style hero layouts.

4. Content
   - Use realistic meeting names, participants, timestamps, and status copy.
   - Keep copy short and product-grade.
   - Make privacy, recording, AI, external guest, and permission states explicit.

5. States
   - Include normal state.
   - Include at least one important edge state: weak network, no permission, external guest, recording, AI unavailable, or role limitation.
   - Include host and participant differences when relevant.

6. Review focus
   - Screen structure.
   - Meeting-context clarity.
   - Low interruption.
   - Trust and privacy.
   - Visual system alignment.

## HTML Artifact Requirements

If asking for an HTML artifact:

- Use a single self-contained HTML file.
- Use CSS variables for tokens.
- Lay out frames in a responsive grid.
- Do not fetch external resources.
- Do not use SVG illustrations as decoration.
- Make text fit inside mobile frames.
- Name frames visibly for review, but keep labels outside the phone frame when possible.

## Figma Requirements

If asking for Figma:

- Use auto layout.
- Name frames with ordered prefixes, such as `01 Lobby`, `02 In Meeting`, `03 AI Summary`.
- Convert repeated controls into components when possible.
- Define variants for active, disabled, loading, and error states.
- Keep tokens documented in a nearby note frame.
