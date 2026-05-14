---
name: pd-review-panel
description: Multi-perspective product/design review for Meeting Superlab outputs. Use when a need frame, competitor analysis, insight synthesis, candidate solution, tradeoff matrix, prototype prompt, PRD AI Check, or review package needs critique from product, user, design, competitor, technical/platform, business, risk, and AI-trust perspectives. Supports parallel subagents when available, or sequential simulated review when subagents are unavailable.
---

# Product Design Review Panel

## Goal

Stress-test product/design exploration from multiple angles before sharing it with the team.

## Step-by-Step Gate

Before running the review, offer 2-3 review modes with pros, cons, and a recommendation. Wait for selection unless the user already specified a mode.

Default modes:

- Lightweight review: product, user, and design perspectives. Pros: fast. Cons: may miss platform or risk issues.
- Full panel: product, user, design, competitor, platform, business, and risk/AI-trust perspectives. Pros: strongest before team review. Cons: longer.
- Visual polish review: hierarchy, spacing, typography, color, component states, responsive quality, and product-grade feel. Pros: best after a draft exists. Cons: does not validate product strategy.
- Evidence audit: focus only on missing evidence, weak assumptions, and next research inputs. Pros: useful before deeper solution work. Cons: less help polishing the proposal.
- SOP gate review: check whether Step 1-6 artifacts are ready for leader review. Pros: best before sharing upward. Cons: less creative.

## When Subagents Are Available

Dispatch independent reviewers with narrow instructions and the same artifact:

- Product reviewer: goal clarity, scope, assumptions, priority, decision points.
- User reviewer: role fit, scenario realism, task flow, friction, accessibility of the idea.
- Design reviewer: information architecture, states, hierarchy, interaction clarity, demo readiness.
- Visual polish reviewer: aesthetic coherence, spacing rhythm, type scale, color discipline, depth, states, responsive fit, and whether the UI looks product-grade rather than generic.
- Competitor reviewer: missing references, weak evidence, copied patterns, differentiation.
- Platform reviewer: permissions, privacy, cross-device, AI, recording, IM, notification, enterprise constraints.
- Business reviewer: value, adoption, retention, growth, enterprise admin or paid-feature implications.
- Risk/AI-trust reviewer: hallucination risk, trust cues, source traceability, user control, compliance concerns.
- SOP reviewer: Q1/Q2/Q3 quality, A/B/C competitor coverage, divergence quality, trade-off decision record, prototype readiness, and PRD AI Check completeness.

Ask each reviewer for:

- Top 3 concerns.
- What is strong.
- What evidence is missing.
- Concrete changes before the next review.

Synthesize reviewer outputs into a single decision-oriented summary.

## When Subagents Are Unavailable

Run the same perspectives sequentially in one response. Clearly label the perspectives.

## Output

Provide:

- Review verdict: ready for discussion, needs another iteration, or blocked by missing evidence.
- SOP gate verdict: whether self-check and AI Check are ready before leader review when relevant.
- Cross-perspective findings.
- Highest-risk assumptions.
- Suggested edits to the proposal/demo prompt.
- Questions to bring to product/design/engineering.

Do not rewrite the full proposal unless the user asks. Focus on critique and next actions.
