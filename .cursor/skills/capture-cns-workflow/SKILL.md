---
name: capture-cns-workflow
description: Capture real SwiftCNS app workflows step-by-step with screenshots for documentation. Use when a user asks for platform tutorials, walkthrough docs, or screenshot-based workflow guides from app.dev.swiftcns.ai.
---

# Capture CNS Workflow

Use this skill to capture real product workflows from the CNS app and produce reliable capture artifacts for tutorial writing.

## Core Principle

Capture only what is actually executed in the app.
Do not fabricate steps, UI labels, outcomes, or screenshots.

## Target App

- Production/dev app URL: `https://app.dev.swiftcns.ai`

## Authentication Handoff

If the app requires login:

1. Stop and request user takeover for authentication.
2. Wait for user confirmation that auth is complete.
3. Resume capture only after confirmation.

Do not attempt to bypass login flows or fake authenticated state.

## Capture Workflow

1. Define scope
   - Confirm the target workflow (for example full learning cycle).
   - Confirm target audience (Innovation Hubs, Program Managers, Startups).

2. Navigate and execute
   - Perform one deliberate action at a time.
   - After each action, verify visible outcome before continuing.

3. Capture evidence for each step
   - Step number
   - Current URL/page context
   - Action taken
   - Expected outcome
   - Actual observed outcome
   - Screenshot asset path

4. Record edge cases
   - Missing permissions
   - Empty-state blockers
   - Data prerequisites
   - Workflow deviations

## Screenshot Naming Convention

Use deterministic names:

- `learning-cycle-step-01-<slug>.png`
- `learning-cycle-step-02-<slug>.png`
- `learning-cycle-step-03-<slug>.png`

Use zero-padded step numbers and short descriptive slugs.

## Output Artifact Format

Return a structured capture log that can be transformed into tutorial pages:

- workflow title
- audience
- prerequisites discovered during run
- ordered steps with screenshot references
- blockers and recovery notes
- completion state

## Quality Checks

- Every documented step has an observed result.
- Every screenshot maps to exactly one step.
- No undocumented jumps between steps.
- Any uncertainty is explicitly marked.
