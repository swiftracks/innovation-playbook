---
name: write-cns-tutorial-from-capture
description: Convert captured CNS workflow logs and screenshots into GitBook-ready step-by-step tutorials for pilot users. Use after running capture-cns-workflow or when screenshot-backed workflow artifacts are provided.
---

# Write CNS Tutorial From Capture

Use this skill to transform real workflow capture artifacts into publishable documentation.

## Core Principle

Write only from observed capture artifacts.
If capture evidence is missing, call it out and request recapture.

## Inputs

- Workflow capture log
- Step-level screenshot references
- Audience target (Innovation Hubs, Program Managers, Startups)
- Target page(s) to update

## Authoring Workflow

1. Validate capture completeness
   - Ensure each step has action + observed outcome + screenshot.
   - Flag missing evidence before drafting.

2. Choose output depth
   - Brief mode: short task walkthrough.
   - Standard mode: full operational tutorial.
   - Deep mode: includes decision logic, edge cases, and role-specific variations.

3. Draft tutorial content
   - Define who the guide is for.
   - List prerequisites and setup conditions.
   - Document each step with:
     - action,
     - expected result,
     - screenshot callout,
     - common mistake (when relevant).

4. Add completion checks
   - Explicit definition of done.
   - Next step in the learning cycle.

5. Add troubleshooting and recovery
   - Include blockers seen during capture.
   - Include practical recovery actions.

## Recommended Tutorial Sections

Use only sections needed for clarity:

- Audience
- Prerequisites
- Step-by-step tutorial
- Screenshots and outcomes
- Common mistakes
- Troubleshooting
- Definition of done
- Next step

## Screenshot Referencing Rule

Each documented step should reference one deterministic screenshot file name from capture output.
Do not reference screenshots that were not captured.

## Quality Checks

- Tutorial steps match observed app behavior.
- Language is practical and audience-appropriate.
- No fabricated UI claims.
- Decision and workflow intent stay aligned with canonical CNS loop.
