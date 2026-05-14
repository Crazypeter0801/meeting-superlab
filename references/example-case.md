# Example Case: Post-Meeting Follow-up SOP

This placeholder case demonstrates the six-step Meeting Superlab SOP. Replace it with a real Tencent Meeting need when available.

## Raw Need

Users finish meetings with many conclusions, decisions, and tasks, but follow-up is fragmented across chat, recordings, notes, documents, and memory. Explore a lighter post-meeting experience that helps users understand what happened and continue work.

## Step 1 Problem Definition

- Q1: Hosts, participants, and task owners cannot quickly find decisions, owners, and next steps after a meeting when evidence is scattered across recordings, chat, notes, files, and memory.
- Q2: If nothing changes, follow-up stays slow, accountability is unclear, and meeting value decays after the call.
- Q3: Positive metrics could include follow-up entry usage, action item confirmation, task handoff rate, and repeat use. Negative metrics could include incorrect summary reports, permission complaints, and manual correction rate. Kill criteria should include a time window, metric threshold, and rollback or review action.

## Step 2 Competitor Questions

- How do Zoom, Teams, Google Meet, and Webex expose recordings, transcripts, summaries, and action items?
- How do Slack, Lark, DingTalk, Telegram, and Discord connect live discussion to async follow-up?
- Which products show source trace, edit controls, sharing permissions, or task handoff?
- What happens when there is no recording, no transcript, no permission, or an external guest?

## Step 3 Creative Divergence

### A. Conservative Optimization

Add a compact post-meeting summary and action-item module to the existing meeting details page.

### B. Experience Restructuring

Create a meeting follow-up workspace that combines summary, actions, recording, chat highlights, files, and next meeting suggestions.

### C. Exploratory AI Direction

Introduce an AI meeting follow-up assistant that lets users ask about decisions, assign tasks, and trace answers back to transcript moments.

## Step 4 Convergence Sketch

Use the five-dimension matrix:

- Simplicity: A is shortest, B is moderate, C has the highest learning cost.
- Cost: A is lowest, B needs cross-module integration, C depends on AI quality and trust.
- Benefit: B and C have higher long-term value; A is faster for v1 validation.
- Extensibility: B can evolve into C if source trace and permissions are designed well.
- Risk: C has the highest AI trust and privacy risk.

Recommended v1: B if the team wants a stronger product narrative; A if the goal is quick validation.

## Step 5 Demo Prompt Sketch

```text
Generate a black-and-white low-fidelity demo for a post-meeting follow-up workspace.
Include: summary, action items, source trace, recording/chat/file entry points, no-summary empty state, permission-limited external guest state.
Focus on structure and reviewability, not visual polish.
```

## Step 6 PRD Check Focus

- Branch completeness: no recording, no transcript, external guest, permission-limited view, AI unavailable.
- Multi-language copy: summary, action item, source trace, share, and permission messages.
- Weak-network behavior: delayed transcript or summary generation.
- Metrics: entry exposure, summary open, action item confirmation, correction rate, permission complaint rate.
- Kill criteria: incorrect summary complaints or permission incidents within a defined time window.
