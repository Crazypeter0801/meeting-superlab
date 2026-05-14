---
name: competitor-research
description: Competitor and reference-product research for Tencent Meeting product/design exploration. Use before solution exploration when the team needs current competitor evidence, public-source research, A/B/C competitor grouping, five-dimension competitor cards, product pattern comparison, or guidance for hands-on competitor experience and screenshot collection across Zoom, Microsoft Teams, Google Meet, Feishu/Lark, DingTalk, Webex, Slack, Telegram, Discord, and related collaboration products.
---

# Competitor Research

## Goal

Use competitor evidence to inspire better product/design directions without copying surface UI or inventing facts.

This is Step 2 of the SOP. Take the Step 1 Q1-Q3 problem definition into research.

## Step-by-Step Gate

Before doing deep competitor research, offer 2-3 research routes with pros, cons, and a recommendation. Wait for the user to choose unless they already specified the route or asked for a one-pass draft.

Default routes:

- Public scan: search official docs, help centers, release notes, and credible reviews. Pros: fast and citeable. Cons: may miss logged-in or nuanced flows.
- Hands-on screenshot task: tell the user which competitors to experience and what to capture. Pros: strongest visual/flow evidence. Cons: requires user effort and access.
- Hybrid: quick public scan first, then request screenshots only for gaps. Pros: balanced and practical. Cons: takes two passes.

## SOP Setup

Before selecting competitors, ask for or infer with clear assumptions:

- User group.
- Interaction pattern.
- Product tone.
- Product or business goal.

Then group references:

- A direct benchmark: closest user group, pattern, tone, and goal; analyze deeply.
- B related reference: useful for one mechanism or module; analyze selectively.
- C industry benchmark: mature practice from another context; extract principles carefully.

Default quantity: 1-2 A references, 1-2 B references, and 0-1 C references. Prefer fewer references with verified detail over many shallow examples.

## Research Modes

### Public Web Research

When current competitor information matters, browse the web. Prioritize:

- Official product pages.
- Help center and support docs.
- Release notes and changelogs.
- App store listings when relevant.
- Credible reviews or product walkthroughs.

Cite sources. Separate facts from interpretation.

### User-Led Competitor Experience

If public material is shallow, stale, login-gated, or not visual enough, ask the user to experience competitors and provide screenshots, screen recordings, notes, or links.

Suggest competitors based on the need:

- Meeting/video: Zoom, Microsoft Teams, Google Meet, Webex.
- Enterprise collaboration: Feishu/Lark, DingTalk, Slack.
- Community/chat/voice: Discord, Telegram.
- AI meeting workflows: Fireflies, Otter.ai, Read AI, Granola when relevant.

## Competitor Card

For A/B references, produce a concrete card:

- Basic information: competitor, feature, and 1-2 sentence positioning.
- Core mechanism: full user path from entry to completion.
- Key design points: 3-5 decisions, each with what it is, why it exists, and what value or risk it creates.
- Data and feedback: adoption, participation, review signals, complaints, incidents, or negative cases when available.
- Implication: mark each point as borrow, localize, or avoid; map it back to Step 1 P0/P1.

Abstract descriptions do not count. Name placement, copy, state changes, permission rules, notification behavior, and edge states when known.

## Analysis Dimensions

Use `../../references/competitor-dimensions.md` when detail is needed.

Cover:

- Entry point and trigger.
- Core task flow.
- Information architecture.
- Collaboration model, roles, and permissions.
- AI assistance, automation, and trust cues.
- Notification, follow-up, and async handoff.
- Empty, error, permission, and cross-device states.
- Visual density and interaction style.
- Patterns worth borrowing.
- Tencent Meeting differentiation opportunities.

## Output

Provide:

- Sources or screenshot evidence used.
- Constraints and A/B/C grouping.
- Competitor observations table.
- Competitor cards for A/B references when enough evidence exists.
- Pattern summary.
- Implications for the current need.
- Gaps requiring user screenshots or hands-on testing.
- Recommended next skill: `insight-synthesis`.
