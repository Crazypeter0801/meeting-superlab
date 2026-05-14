# Tencent Meeting Mobile Components

## Navigation

- Use a native-feeling top bar with clear title, back affordance, and one primary trailing action at most.
- During a meeting, minimize top chrome. Prefer status chips and compact overlays.
- Bottom tabs are appropriate for home-level areas, not active meeting surfaces.

## Meeting Lobby

Required elements:

- Meeting name or join target.
- User identity and device status.
- Camera preview when relevant.
- Mic/camera toggles before join.
- Primary join action.
- Permission or privacy explanation before requesting sensitive access.

## In-Meeting Canvas

Required elements:

- Active speaker or shared content should dominate.
- Participant count, duration, network state, and recording or AI status must be glanceable.
- Controls dock should be stable and not resize when labels change.
- End meeting or leave action must be visually distinct from neutral controls.

## Control Dock

Common controls:

- Mic, camera, share, participants, chat, more.
- AI summary, captions, recording, reactions when relevant.

Rules:

- Use familiar icons plus accessible labels in generated specs.
- Keep destructive actions red.
- Avoid burying privacy-sensitive controls in ambiguous "more" menus.
- Include disabled, active, muted, permission-blocked, and loading states.

## Bottom Sheets

Use bottom sheets for:

- Participants.
- Chat.
- AI summary.
- Captions or transcript.
- Device settings.
- More actions.

Rules:

- First row should summarize current state.
- Primary action should stay reachable.
- Support half and full height when content grows.
- Keep the meeting visible or easily restorable.

## AI Meeting Surfaces

AI surfaces must show:

- What AI is doing.
- Who can see the result.
- Source or confidence caveat when useful.
- User control to dismiss, pause, view detail, or report issue.

Avoid making AI feel like an interrupting assistant during active speaking.

## Trust And Privacy States

Always design explicit states for:

- Recording on or paused.
- AI summary on or off.
- External guest present.
- Screen sharing active.
- Camera or mic permission missing.
- Captions or transcript visible.
- Sensitive content warning when necessary.

## Failure States

Include when relevant:

- Weak network.
- Reconnecting.
- Device switch in progress.
- Host permission denied.
- Room capacity or waiting room.
- AI summary delayed or unavailable.
- Recording permission blocked by enterprise policy.
