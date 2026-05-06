---
name: author-cns-playbook
description: Author CNS-first innovation playbook pages with canonical stage flow, quality gates, and decision-readiness outputs. Use when creating or significantly revising methodology pages in innovation-playbook.
---

# Author CNS Playbook

Use this skill when drafting or heavily editing playbook methodology content.

## Objective

Produce CNS-first pages that are operational, evidence-oriented, and aligned with canonical loop stages.
Be strict on reasoning quality and evidence discipline, flexible on output form.
When available, prefer capture-backed workflow evidence from `capture-cns-workflow`.

## Workflow

1. Define scope
   - Identify target audience.
   - Identify which loop stage(s) the page covers.
   - Define expected artifact and decision impact.

2. Frame the page
   - Add clear purpose and outcome.
   - Define inputs and prerequisites.
   - Describe stage intent in one concise section.

3. Encode quality gates
   - Add pre-declared criteria guidance.
   - Specify what evidence is expected.
   - Specify what confidence shift should be documented.

4. Add execution guidance
   - Provide practical steps.
   - Include weak-vs-strong examples if useful.
   - Keep guidance operational, not abstract.

5. Ensure decision linkage
   - Show how outputs support go/iterate/pivot/stop.
   - Avoid ending with evidence collection only.

6. Cross-link intelligently
   - Link to adjacent stage pages.
   - Link to glossary/concepts only where necessary.

## Required Checks Before Finalizing

- Stage and artifact are explicit.
- Evidence standard is explicit.
- Decision-readiness path is explicit.
- Claims do not exceed known CNS runtime behavior.
- Language uses canonical CNS terms consistently.
- Tutorial workflow claims are screenshot-backed or explicitly marked as unverified.

## Capture-to-Write Integration

- For platform walkthrough pages, use output from `capture-cns-workflow` as primary source.
- If capture artifacts exist, prefer `write-cns-tutorial-from-capture` before manual drafting.
- If capture artifacts are missing, request recapture rather than inventing steps.

## Adaptive Output Modes

Choose a structure based on page intent and depth.
Do not force a fixed template when it weakens clarity.

### Mode A: Brief Note (fast tactical updates)

Use for short guidance or narrow fixes.
Typical sections:

1. Context
2. Recommendation
3. Evidence or rationale
4. Decision or next action

### Mode B: Standard Method (default for stage pages)

Use for most operational playbook content.
Typical sections:

1. Purpose
2. Outcome
3. Inputs
4. Steps in SwiftCNS
5. Quality gates
6. Outputs
7. Definition of done
8. Next step

### Mode C: Deep Methodology (complex or cross-stage topics)

Use when tradeoffs, constraints, or failure patterns require depth.
Typical sections:

1. Context and problem framing
2. Scope and assumptions
3. Method logic
4. Evidence model and quality thresholds
5. Decision model and tradeoffs
6. Failure modes and recovery
7. Handoff implications

## Form Flexibility Rules

- Merge or reorder sections when it improves reasoning flow.
- Omit sections that add no decision value.
- Add sections only when they clarify evidence, logic, or execution.
- Never optimize for format compliance over critical thinking.
