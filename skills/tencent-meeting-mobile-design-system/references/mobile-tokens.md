# Tencent Meeting Mobile Tokens

These are provisional tokens for Apple-like Tencent Meeting mobile design. Replace with official tokens when available.

## Viewport

- Primary iPhone canvas: 393 x 852.
- Alternate compact canvas: 390 x 844.
- Safe areas: top 54, bottom 34.
- Minimum touch target: 44 x 44.
- In-meeting control hit target: 48 x 48 preferred.

## Color

- Background: #F7F8FA.
- Elevated surface: #FFFFFF.
- Secondary surface: #F2F4F7.
- Separator: #E5E8EF.
- Primary text: #111827.
- Secondary text: #5B6472.
- Tertiary text: #8A93A3.
- Primary blue: #2F80FF.
- Primary blue pressed: #1F6FE5.
- Success: #20A464.
- Warning: #F59E0B.
- Danger: #E5484D.
- AI accent: #6D5DF6, used sparingly for AI-only affordances.

Use semantic intent first. Do not make the whole product blue or purple.

## Typography

Use PingFang SC, SF Pro, system UI.

- Large title: 28 / 34, semibold.
- Page title: 20 / 26, semibold.
- Navigation title: 17 / 22, semibold.
- Body: 16 / 22, regular or medium.
- Secondary: 14 / 20, regular.
- Caption: 12 / 16, regular or medium.
- Numeric timer: 15 / 20, medium, tabular numbers.

Limit each screen to 3-4 text styles. Support text expansion and truncation.

## Spacing

- Screen horizontal margin: 16.
- Dense meeting margin: 12.
- Group gap: 16.
- Related item gap: 8.
- List row vertical padding: 12.
- Bottom sheet content padding: 20.
- Control dock gap: 10-12.

Spacing inside a group should be smaller than spacing between groups.

## Radius

- Small controls and chips: 8.
- List tiles and compact cards: 10-12.
- Floating controls: 14-16.
- Bottom sheets and modal panels: 20-24.
- Full circular controls for mic, camera, share, and end call.

Avoid oversized radius on dense enterprise screens.

## Elevation And Materials

- Prefer subtle separators on flat surfaces.
- Use very soft shadow only for floating docks, sheets, and transient overlays.
- Use translucent material only when it helps preserve meeting context behind the layer.
- Do not use decorative gradients, blobs, or heavy glass effects.

## Motion

- Use 160-240ms transitions for sheets, toasts, and control expansion.
- Use spring only for direct manipulation, not for status changes.
- Honor reduced motion with fade or instant alternatives.
- Avoid decorative animation during active meetings.
