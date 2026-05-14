---
name: prd-ai-check
description: Run the Meeting Superlab Step 6 PRD AI Check for Tencent Meeting product/design work. Use when the user provides a PRD v0.5, structured product spec, or wants a PRD checklist after solution convergence/prototype handoff. Checks main path, branches, onboarding, platform compatibility, multilingual copy, large font, dark mode, weak network, grey release/AB experiment, metrics, kill criteria, data reporting, and security; then produces revision-record-ready findings and a simplified Chinese/English/traditional Chinese copy table.
---

# PRD AI Check

## Goal

Help product turn PRD v0.5 into PRD v1. AI checks and challenges; product owns the decisions.

Do not replace product thinking by writing the full PRD from scratch unless the user explicitly asks for a draft. The default is:

`product PRD v0.5 -> AI Check -> product accepts/rejects/pends findings -> PRD v1 revision record`

## Preconditions

Ask for:

- PRD v0.5 or structured product spec.
- Step 1 Q1/Q2/Q3.
- Selected direction and decision record from `solution-convergence`.
- Prototype or key-page outline when available.

If no PRD exists, provide a PRD v0.5 outline and checklist instead of pretending to check a document.

## Standard PRD Modules

Check whether the PRD covers:

- Revision record.
- Problem to solve.
- Solution logic.
- Scenario and product-line compatibility.
- Onboarding.
- Metrics.
- Grey release and experiment logic.
- Kill criteria.
- Weak-network behavior.
- Data reporting.
- Security or compliance self-check.

## Default AI Check Items

For each item, give a rating and concrete findings:

1. Main path simplicity.
2. Branch completeness.
3. Onboarding.
4. Platform compatibility.
5. Multi-language copy.
6. Large font mode.
7. Dark mode.
8. Weak-network behavior.
9. Grey release and A/B experiment logic.
10. Monitoring and data metrics.
11. Kill criteria completeness.

Also check data reporting and security/compliance when the PRD includes user-generated content, AI-generated content, sharing, payment, ads, minors, enterprise admin controls, or sensitive meeting data.

## Rating

Use simple ratings:

- Green: acceptable, only minor notes.
- Yellow: usable but should be revised before leader review.
- Red: must revise before leader review.
- N/A: not applicable, with reason.

For every yellow or red finding, provide:

- Specific issue.
- Why it matters.
- Suggested revision direction.
- Whether it affects product, design, engineering, data, legal/compliance, or operations.

## Multi-Language Copy Table

Scan user-visible copy such as buttons, tips, onboarding, empty states, error messages, notification copy, and permission copy.

Output:

| Copy location | Simplified Chinese | English draft | Traditional Chinese draft | Notes |

Flag terminology, length, culture, legal, or trust-risk concerns. Treat translation as an initial draft for product review, not final localization.

## Revision Record Handoff

End with a table the product owner can paste into the PRD revision record:

| Date | Source | Check item | Rating | Revision content | Owner |

Only accepted findings should become revision records. If the user has not decided yet, label them as proposed revisions.

## Output

Provide:

- PRD module completeness summary.
- AI Check table for the default items.
- Top must-fix issues before leader review.
- Proposed revision-record rows.
- Multi-language copy table.
- Remaining open decisions for product/design/engineering.
- Recommended next skill: `pd-review-panel` for review readiness.
