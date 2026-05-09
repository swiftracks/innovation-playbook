# Run Learning Cycle Guide (Internal Source)

This document is the canonical internal narrative for the current SwiftCNS UI learning-cycle walkthrough. It is the primary source for expanding playbook pages with screen-level context.

## Audience

- Playbook authors expanding user-facing workflow pages.
- Internal reviewers validating screen sequence and UX claims.

## Workflow objective

Help a team move from first login to reusable insight context through the shipped loop:

`idea/problem -> assumptions -> hypotheses -> experiments -> learnings -> insights`

Artifacts are currently persisted through Insight, then handed off into team decision routines.

## Screenshot naming note

The public runbook uses filenames with `-ems` suffixes for some assets (for example `08.2-experiment-draft-approval-ems.png`). If older aliases appear in draft notes, normalize references to the runbook naming set.

## End-to-end sequence

### 1) Workspace entry and project creation

Primary screenshot: `@innovation-playbook/screenshots/01-workspace-dashboard.png`

- User lands on workspace dashboard after login at `https://swiftcns.ai`.
- User clicks **Create a project**.
- Team should choose a broad, durable project scope so insights can compound over time.

Why this matters: project scope defines the memory boundary of the learning system.

### 2) Project dashboard and conversation start

Primary screenshot: `@innovation-playbook/screenshots/02-project-dashboard.png`

- User enters project dashboard with project-level analytics and tabs.
- User creates first conversation (`Create first conversation` or `New conversation`).
- User names thread clearly for cross-team context.

Why this matters: this thread becomes the anchor for assumption surfacing and hypothesis generation.

### 3) Kickoff context submission

Primary screenshot: `@innovation-playbook/screenshots/03-kickoff-conversation.png`

- User submits high-signal context: problem, target users, constraints, goals.
- User optionally uploads supporting docs (PRD, plans, research notes).

Why this matters: stronger context improves assumption quality and reduces generic outputs.

### 4) Clarifying questions

Primary screenshot: `@innovation-playbook/screenshots/04-clarifying-questions-conversation.png`

- Assumption mapping agent asks clarifying questions as needed.
- User answers with available detail and marks unknowns explicitly.

Why this matters: unknowns are signal; guessing lowers downstream evidence quality.

### 5) Critical assumption selection

Primary screenshot: `@innovation-playbook/screenshots/05-select-assumptions.png`

- Agent presents assumptions mapped by **importance** and **evidence**.
- Team prioritizes high-importance, low-evidence assumptions first.

Why this matters: assumption choice determines whether the cycle resolves meaningful uncertainty.

### 6) Hypothesis selection

Primary screenshot: `@innovation-playbook/screenshots/06-select-hypothesis.png`

- Experiment design agent proposes testable hypotheses.
- Team reviews success/invalidation framing and chooses one.
- Hypotheses are categorized as desirability, feasibility, or viability.

Why this matters: hypothesis precision determines experiment interpretability.

### 7) Experiment option selection in conversation

Primary screenshots:

- `@innovation-playbook/screenshots/07-select-experiment.png`
- `@innovation-playbook/screenshots/07.1-selected-experiment.png`

- Team compares experiment cards by method, criteria, metrics, and tradeoffs.
- Team balances setup complexity, runtime, cost, and data reliability.
- Team selects an experiment and opens it in EMS.

Why this matters: choosing for convenience over reliability causes weak learning quality.

### 8) EMS execution flow (draft -> approval -> tracker -> completion)

Primary screenshots:

- `@innovation-playbook/screenshots/08-experiment-draft-ems.png`
- `@innovation-playbook/screenshots/08.1-experiment-draft-coordination-ems.png`
- `@innovation-playbook/screenshots/08.2-experiment-draft-approval-ems.png`
- `@innovation-playbook/screenshots/08.3-experiment-data-tracker-ems.png`
- `@innovation-playbook/screenshots/08.4-experiment-data-tracker-inputs-ems.png`
- `@innovation-playbook/screenshots/08.5-experiment-data-tracker-lock-ems.png`

State transitions:

1. Experiment opens in **Draft** mode.
2. Team refines scope, criteria, and metrics.
3. Team assigns owner and due date.
4. Team approves/locks experiment.
5. Team captures execution data in tracker (manual schema or Data Tracking Agent).
6. Team may import CSV data when relevant.
7. Team locks tracker and marks experiment completed.

Why this matters: clear state transitions prevent execution drift and missing ownership.

### 9) Learning generation and draft review

Primary screenshots:

- `@innovation-playbook/screenshots/08.6-generate-learning-card-ems.png`
- `@innovation-playbook/screenshots/08.7-generate-learning-card-submit-ems.png`
- `@innovation-playbook/screenshots/09-learning-card-draft-ems.png`

- Team generates learning card from experiment details.
- Team adds optional context before submit.
- Agent synthesizes learning draft from tracker data and context.
- Team edits observations/insights, adds notes/tags, then approves.

Why this matters: draft review is a quality gate; generated output should not be treated as automatic truth.

### 10) Insight library and Sources compounding

Primary screenshots:

- `@innovation-playbook/screenshots/09.1-insights-library-ems.png`
- `@innovation-playbook/screenshots/09.2-conversation-sources.png`

- Approved outputs are available in insights library for team-wide reuse.
- In new conversations, users attach prior artifacts through Sources panel.
- Sources can include documents, assumptions, hypotheses, experiments, learnings, and insights.

Why this matters: this is the compounding mechanism that increases cycle quality over time.

## Common quality risks

- Narrow project naming that fragments long-term insight memory.
- Assumption selection driven by ease rather than decision risk.
- Tracker schema that cannot support synthesis-quality conclusions.
- Learning approval without evidence-interpretation review.
- New cycles started without adding relevant Sources.

## Definition of done (for walkthrough completeness)

- Every documented step has one or more supporting screenshots.
- UI state transitions are explicit (draft, approved, locked, completed).
- Sequence can be executed end-to-end without fabricated behavior claims.