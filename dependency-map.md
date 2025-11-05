# Dependency Map

## Overview

This map shows how chapters relate to each other and different learning paths through the guide.

## Chapter Dependencies

### Start Here
- **No dependencies** - Start here for all paths
- **Enables**: All subsequent chapters

### Decide What to Build

#### 01 — Idea / Problem
- **Depends on**: Start Here
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
- **Enables**: Launch & Iterate (all chapters)
- **Can be done in parallel with**: None

### Launch & Iterate

#### 09 — Private Beta
- **Depends on**: 09 — Deploy
- **Enables**: 10 — Instrumentation, 11 — Experiments
- **Can be done in parallel with**: None

#### 10 — Instrumentation
- **Depends on**: 09 — Private Beta
- **Enables**: 11 — Experiments, 12 — Feedback Ops
- **Can be done in parallel with**: 11 — Experiments (after instrumentation setup)

#### 11 — Experiments
- **Depends on**: 09 — Private Beta, 10 — Instrumentation (recommended)
- **Enables**: 12 — Feedback Ops
- **Can be done in parallel with**: 10 — Instrumentation (for setup)

#### 12 — Feedback Ops
- **Depends on**: 09 — Private Beta, 10 — Instrumentation (recommended)
- **Enables**: Iteration back to Decide, Build, or Launch
- **Can be done in parallel with**: 11 — Experiments

## Learning Paths

### Path 1: Full Product Innovation Cycle
**Duration**: Complete end-to-end journey
**Path**: Start Here → Decide (all) → Build (all) → Launch (all) → Iterate

### Path 2: Quick Decision Making
**Duration**: Focus on validation before building
**Path**: Start Here → Decide (all) → [Decision Point: Build or Pivot]

### Path 3: Building an MVP
**Duration**: Focus on execution
**Path**: Start Here → Build (all) → Launch (all)

### Path 4: Optimizing Existing Product
**Duration**: Focus on iteration
**Path**: Start Here → Launch (all) → [Iterate]

### Path 5: Skimmer Path
**Duration**: Overview and templates
**Path**: Start Here → [Chapter summaries] → Templates → Examples

### Path 6: Deep Dive Path
**Duration**: Comprehensive understanding
**Path**: Start Here → [All chapters in order] → Worked Examples → Self-Assessments

## Prerequisites Map

### Before Starting "Decide What to Build"
- [ ] Completed "Start Here"
- [ ] Understand Jobs-to-Be-Done framework
- [ ] Have access to user research or customer insights

### Before Starting "Build the MVP"
- [ ] Completed "Decide What to Build" (all chapters)
- [ ] Have a validated hypothesis or decision to build
- [ ] Have development environment ready (for Dev path)
- [ ] Have design tools ready (for PM path)

### Before Starting "Launch & Iterate"
- [ ] Completed "Build the MVP" (all chapters)
- [ ] Have working MVP (at least thin vertical)
- [ ] Have access to deployment infrastructure
- [ ] Have user feedback channels ready

## Parallel Work Opportunities

### Can Work in Parallel
- **10 — Instrumentation** and **11 — Experiments** (after Private Beta)
- **11 — Experiments** and **12 — Feedback Ops** (after Private Beta)

### Must Be Sequential
- All "Decide" chapters (01-06) must be done in order
- Setup must come before Build chapters
- Private Beta must come before other Launch chapters

## Dependency Graph

```
Start Here
    ↓
Decide What to Build
    ├─ 01 → 02 → 03 → 04 → 05 → 06
    ↓
Build the MVP
    ├─ 05 → 06 → 08 → 09
    ↓
Launch & Iterate
    ├─ 09 → [10, 11] → 12
    ↓
[Iterate back to Decide, Build, or Launch]
```

## Quick Reference

- **Need to validate an idea?** → Start at "Decide What to Build"
- **Ready to build?** → Start at "Build the MVP"
- **Have an MVP to launch?** → Start at "Launch & Iterate"
- **Want templates only?** → Go directly to chapter Templates
- **Want examples only?** → Go directly to chapter Examples

