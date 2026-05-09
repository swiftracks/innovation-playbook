---
name: map-content-to-cns-runtime
description: Map playbook content claims to CNS runtime contracts across cns-ui, csn-backend, and cns-prompts. Use when validating methodology pages against implemented product behavior.
---

# Map Content to CNS Runtime

Use this skill to verify that documentation statements are grounded in current CNS behavior.
Be strict on reasoning quality and evidence discipline, flexible on output form.

## Objective

Prevent methodology docs from drifting away from actual product contracts.
This skill validates claims, not page formatting style.
For walkthrough docs, validate claims against capture artifacts before runtime mapping.

## Mapping Workflow

1. Extract claims
   - Identify all functional claims in the target page.
   - Separate present-tense claims from roadmap intent.
   - Mark any tutorial steps that are not backed by capture outputs.

2. Map each claim to a layer
   - Frontend (`cns-ui`): user flow, tool UI, chat runtime behavior.
   - Backend (`csn-backend`): APIs, entities, orchestration, lineage.
   - Prompts (`cns-prompts`): agent output schema, action semantics, transitions.

3. Assess status
   - Implemented
   - Partially implemented
   - Planned only
   - Unsupported

4. Rewrite where needed
   - Downgrade unsupported present-tense claims to planned language.
   - Replace vague claims with artifact-specific and stage-specific wording.

5. Record traceability
   - For major claims, capture where the contract is anchored.
   - If no anchor exists, open a docs issue or remove the claim.

## Red Flags

- Invented UI controls or automation flows.
- Implied entities not represented in current model.
- Promises of outcomes without evidence/quality conditions.
- Generic AI language that bypasses stage-level rigor.

## Completion Checklist

- Every major claim has a runtime anchor or planned label.
- No unsupported present-tense statements remain.
- Canonical CNS terminology is preserved.

## Definition of Done

Mapping is complete when a reviewer can trace each major functional claim to an explicit runtime layer or see a clear planned qualifier where runtime support is missing.
