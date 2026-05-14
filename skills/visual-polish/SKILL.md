---
name: visual-polish
description: Improve the visual quality, hierarchy, polish, and product-grade feel of generated Tencent Meeting interface drafts, low-fidelity prototypes, Figma frames, HTML demos, or UI screenshots. Use when the user asks to make a generated interface more beautiful, polished, premium, modern, professional, product-like, less AI-looking, or more consistent with Tencent Meeting/product-design standards. Also use after demo-and-review or figma-handoff when a draft needs a visual refinement pass before review.
---

# Visual Polish

## Goal

Turn a functional but rough UI draft into a clearer, more beautiful, review-ready product interface.

This skill is adapted for Tencent Meeting product/design work. Favor calm, useful, enterprise-grade polish over decorative spectacle.

Reference inspiration: `tristanmanchester/agent-skills@designing-beautiful-websites` from the open skills ecosystem. Do not copy its files verbatim; use the principles as a design-quality baseline.

## When To Use

Use this skill for:

- Low-fidelity or medium-fidelity screen drafts that feel plain, generic, or "AI-generated".
- Figma frames that need hierarchy, spacing, typography, color, and component-state refinement.
- HTML/CSS demos that need better visual quality before showing to product/design partners.
- Design review requests focused on beauty, polish, consistency, or product-grade feel.
- Tencent Meeting flows where the structure is roughly right but the UI lacks credibility.
- Tencent Meeting mobile drafts that should follow the Apple-like mobile design system.

Do not use this as a substitute for `need-framing`, `solution-exploration`, or `solution-convergence`. Visual polish should not hide weak product logic.

## Gate

Before polishing, confirm what artifact exists:

- Screenshot, Figma link, HTML/demo, written page outline, or component list.
- Target fidelity: low-fidelity, medium-fidelity, or closer-to-product.
- Product tone: Tencent Meeting calm professional, lightweight consumer, admin/enterprise dense, AI assistant/trust-sensitive, or exploratory concept.
- Whether the target should follow `tencent-meeting-mobile-design-system`, especially for mobile and Apple-like requests.

If the user only says "美化一下" and gives no artifact, ask for a screenshot/Figma link/demo file or offer to create a visual direction from the current solution outline.

## Polish Pass

Review in this order:

1. Purpose and primary action: can a reviewer tell what this screen is and what to do first within 10 seconds?
2. Layout and grouping: is spacing inside groups smaller than spacing between groups?
3. Hierarchy: are title, key data, primary action, secondary actions, and metadata clearly separated?
4. Typography: is the type scale limited, readable, and matched to the density of the surface?
5. Color: are accents meaningful, restrained, and accessible? Avoid one-note palettes and gratuitous gradients.
6. Components: do buttons, inputs, tabs, cards, menus, tags, and alerts use familiar product patterns?
7. States: normal, empty, loading, error, permission, weak-network, cross-device, and role-specific states.
8. Microcopy: is copy short, concrete, and appropriate for meeting/productivity contexts?
9. Accessibility: contrast, focus states, hit targets, keyboard path, text overflow, and responsive behavior.
10. Tencent Meeting fit: does the UI feel trustworthy, efficient, cross-platform, and respectful of meeting context?
11. Apple-like mobile fit when relevant: does the UI feel content-first, native, safe-area aware, low-interruption, and privacy-explicit without becoming a generic iOS clone?

## Product Design Aesthetic Rules

- For SaaS, meeting, admin, and collaboration tools, prioritize density, scanability, and calm hierarchy over marketing-style decoration.
- Use cards only for repeated items, modals, and genuinely framed tools. Do not put cards inside cards.
- Use 8px radius or less unless matching an existing design system.
- Use icons for clear tools and actions when available; avoid text-only tool controls where symbols are familiar.
- Define stable dimensions for boards, panels, toolbars, counters, and repeated tiles so labels and states do not shift layout.
- Do not use large hero typography inside compact panels or dashboards.
- Do not rely on a single hue family. Use neutral foundations with 1 primary accent and semantic accents.
- Avoid decorative orbs, bokeh blobs, and generic purple-blue gradients for Tencent Meeting product surfaces.
- Make text fit on mobile and desktop; long labels should wrap or be shortened.
- For mobile, respect safe areas, 44 px touch targets, bottom reachability, stable control docks, and explicit recording/AI/external-guest states.
- Use Tencent Meeting blue for primary actions and active states; reserve AI accent color for AI-specific surfaces only.

## Output Modes

### Audit Mode

When the user provides a screenshot, Figma frame, or existing demo, output:

- Visual verdict: ready, needs polish, or structurally blocked.
- Top 5 highest-impact fixes.
- Before/after description by screen area.
- Token adjustments: spacing, typography, color, radius, shadow.
- Component/state fixes.
- Accessibility and responsive risks.
- Next step: update Figma, update code, or create a polished prompt.

### Generation Mode

When the user wants a better prompt or new UI direction, output:

- Visual direction in one sentence.
- Layout structure.
- Token system.
- Component styling rules.
- Key states to include.
- Polished low/medium-fidelity prompt for Figma, HTML, or image generation.

### Implementation Mode

When working in a codebase, inspect existing design tokens and components first. Then make focused edits to:

- spacing and layout,
- typography,
- color and contrast,
- component states,
- empty/loading/error states,
- responsive behavior.

Verify with screenshots when possible.

## Output Contract

End with one of these handoffs:

- To `figma-handoff` if the user wants the polished direction drawn in Figma.
- To `demo-and-review` if the polish should become a low-fidelity demo prompt.
- To `mobile-prototype-artifact` if the polish should become an Open Design, HTML artifact, or Figma generation prompt for Tencent Meeting mobile.
- To `meeting-design-review` before stakeholder review when the mobile draft appears complete.
- To `pd-review-panel` if the polished UI needs multi-perspective critique.
