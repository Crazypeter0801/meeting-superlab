---
name: screenshot-analysis
description: Analyze competitor or Tencent Meeting screenshots, screen recordings, captured flows, and user notes for product/design exploration. Use when the user provides screenshots from Zoom, Teams, Google Meet, Feishu/Lark, DingTalk, Webex, Slack, Telegram, Discord, Tencent Meeting, or other collaboration products and wants structured observations, interaction patterns, A/B/C competitor card evidence, risks, and reusable insights.
---

# Screenshot Analysis

## Goal

Turn screenshots or recordings into structured product-design evidence.

## Process

1. Identify product, screen, user role, and task stage if visible.
2. Describe observable facts before interpretation.
3. Extract information architecture, hierarchy, entry points, controls, states, and feedback.
4. Note collaboration mechanics: roles, permissions, visibility, sharing, handoff, notifications.
5. Identify AI/trust mechanics if present: confidence, source trace, editability, approval, privacy cues.
6. Highlight friction, ambiguity, missing states, and opportunities.
7. Capture concrete design points: placement, copy, state changes, timing, permission behavior, and edge cases.
8. Translate observations into implications for Tencent Meeting and map them back to the Step 1 problem.

## Evidence Rules

- Label facts, interpretations, and hypotheses separately.
- Do not infer hidden product behavior from a static screenshot unless clearly marked as a hypothesis.
- Ask for missing states when needed: empty state, permission denied, external guest, no transcript, no network, no recording, mobile/desktop difference.
- Do not treat screenshots as proof of hidden business rules, logged-in behavior, or performance. Mark those as follow-up questions.

## Output

Provide:

- Screenshot inventory.
- Observable facts.
- Product/design patterns.
- Concrete design points that can feed competitor cards.
- Potential user impact.
- Relevance to the current need.
- Follow-up screenshots or flows to collect.
- Recommended next skill: `insight-synthesis`.
