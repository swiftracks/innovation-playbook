# Dependency Map

## Overview

This map shows how chapters relate to each other and different learning paths through the guide.

## Chapter Dependencies

### Getting Started
- **No dependencies** - Start here for all paths
- **Enables**: All subsequent chapters

### Decide What to Build

#### 01 — Idea / Problem
- **Depends on**: Getting Started
- **Enables**: 02 — Identify Critical Assumptions
- **Can be done in parallel with**: None

#### 02 — Identify Critical Assumptions
- **Depends on**: 01 — Idea / Problem
- **Enables**: 03 — Form Testable Hypotheses
- **Can be done in parallel with**: None

#### 03 — Form Testable Hypotheses
- **Depends on**: 02 — Identify Critical Assumptions
- **Enables**: 04 — Design & Run Experiments
- **Can be done in parallel with**: None

#### 04 — Design & Run Experiments
- **Depends on**: 03 — Form Testable Hypotheses
- **Enables**: 05 — Extract Key Learnings
- **Can be done in parallel with**: None

#### 05 — Extract Key Learnings
- **Depends on**: 04 — Design & Run Experiments
- **Enables**: 06 — Synthesize Insights → Decision
- **Can be done in parallel with**: None

#### 06 — Synthesize Insights → Decision
- **Depends on**: 05 — Extract Key Learnings
- **Enables**: Build the MVP (all chapters)
- **Can be done in parallel with**: None

### Build the MVP

#### 05 — Planning
- **Depends on**: 06 — Synthesize Insights → Decision (from Decide)
- **Enables**: 06 — Setup
- **Can be done in parallel with**: None

#### 06 — Setup
- **Depends on**: 05 — Planning
- **Enables**: 08 — Build Features
- **Can be done in parallel with**: None

#### 08 — Build Features
- **Depends on**: 06 — Setup
- **Enables**: 09 — Deploy
- **Can be done in parallel with**: None

#### 09 — Deploy
- **Depends on**: 08 — Build Features
- **Enables**: Launch & Iterate (Coming Soon) (all chapters)
- **Can be done in parallel with**: None

### Launch & Iterate (Coming Soon)

#### 01 — Prepare ICP
- **Depends on**: 09 — Deploy (from Build), Decide What to Build (initial ICP research)
- **Enables**: 02 — Develop Messaging Strategy
- **Can be done in parallel with**: None

#### 02 — Develop Messaging Strategy
- **Depends on**: 01 — Prepare ICP
- **Enables**: 03 — Design Channel Strategy
- **Can be done in parallel with**: None

#### 03 — Design Channel Strategy
- **Depends on**: 02 — Develop Messaging Strategy
- **Enables**: 04 — Build Website V1
- **Can be done in parallel with**: None

#### 04 — Build Website V1
- **Depends on**: 03 — Design Channel Strategy
- **Enables**: 05 — Setup Tool Stack
- **Can be done in parallel with**: None

#### 05 — Setup Tool Stack
- **Depends on**: 04 — Build Website V1
- **Enables**: 06 — Launch Private Beta
- **Can be done in parallel with**: None

#### 06 — Launch Private Beta
- **Depends on**: 05 — Setup Tool Stack
- **Enables**: 07 — Run Experiments, 08 — Synthesize Insights
- **Can be done in parallel with**: None

#### 07 — Run Experiments
- **Depends on**: 06 — Launch Private Beta
- **Enables**: 08 — Synthesize Insights
- **Can be done in parallel with**: 08 — Synthesize Insights (after initial experiments)

#### 08 — Synthesize Insights
- **Depends on**: 06 — Launch Private Beta, 07 — Run Experiments (recommended)
- **Enables**: 09 — Exit to Public Beta
- **Can be done in parallel with**: 07 — Run Experiments (for ongoing synthesis)

#### 09 — Exit to Public Beta
- **Depends on**: 08 — Synthesize Insights
- **Enables**: Iteration back to Decide, Build, or Launch
- **Can be done in parallel with**: None

## Learning Paths

### Path 1: Full Product Innovation Cycle
**Duration**: Complete end-to-end journey
**Path**: Getting Started → Decide (all) → Build (all) → Launch (Coming Soon) (all) → Iterate

### Path 2: Quick Decision Making
**Duration**: Focus on validation before building
**Path**: Getting Started → Decide (all) → [Decision Point: Build or Pivot]

### Path 3: Building an MVP
**Duration**: Focus on execution
**Path**: Getting Started → Build (all) → Launch (Coming Soon) (all)

### Path 4: Optimizing Existing Product
**Duration**: Focus on iteration
**Path**: Getting Started → Launch (Coming Soon) (all) → [Iterate]

### Path 5: Skimmer Path
**Duration**: Overview and templates
**Path**: Getting Started → [Chapter summaries] → Templates → Examples

### Path 6: Deep Dive Path
**Duration**: Comprehensive understanding
**Path**: Getting Started → [All chapters in order] → Worked Examples → Self-Assessments

## Prerequisites Map

### Before Starting "Decide What to Build"
- [ ] Completed "Getting Started"
- [ ] Understand Jobs-to-Be-Done framework
- [ ] Have access to user research or customer insights

### Before Starting "Build the MVP"
- [ ] Completed "Decide What to Build" (all chapters)
- [ ] Have a validated hypothesis or decision to build
- [ ] Have development environment ready (for Dev path)
- [ ] Have design tools ready (for PM path)

### Before Starting "Launch & Iterate (Coming Soon)"
- [ ] Completed "Build the MVP" (all chapters)
- [ ] Have working MVP (at least thin vertical)
- [ ] Have access to deployment infrastructure
- [ ] Have user feedback channels ready

## Parallel Work Opportunities

### Can Work in Parallel
- **07 — Run Experiments** and **08 — Synthesize Insights** (after Launch Private Beta, for ongoing synthesis)

### Must Be Sequential
- All "Decide" chapters (01-06) must be done in order
- Setup must come before Build chapters
- Launch chapters 01-05 must be done in order before launching
- Launch Private Beta (06) must come before post-launch chapters (07-09)

## Dependency Graph

```
Getting Started
    ↓
Decide What to Build
    ├─ 01 → 02 → 03 → 04 → 05 → 06
    ↓
Build the MVP
    ├─ 05 → 06 → 08 → 09
    ↓
Launch & Iterate (Coming Soon)
    ├─ 01 → 02 → 03 → 04 → 05 → 06 → [07, 08] → 09
    ↓
[Iterate back to Decide, Build, or Launch]
```

## Quick Reference

- **Need to validate an idea?** → Start at "Decide What to Build"
- **Ready to build?** → Start at "Build the MVP"
- **Have an MVP to launch?** → Start at "Launch & Iterate (Coming Soon)"
- **Want templates only?** → Go directly to chapter Templates
- **Want examples only?** → Go directly to chapter Examples

