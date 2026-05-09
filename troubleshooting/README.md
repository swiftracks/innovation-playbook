# Troubleshooting and Recovery

**Purpose**: Diagnose slow cycles and recover quickly without sacrificing quality.

## Who this is for

- Teams currently stuck in a cycle.
- Program and mentor roles running recovery interventions.

This page exists because no team runs clean cycles all the time. The goal is not to avoid all breakdowns. The goal is to recognize them early enough that they do not keep compounding.

## Common blockers

- Unclear assumptions.
- Weak or non-testable hypotheses.
- Experiments with no usable evidence.
- Learnings captured as opinions.
- Insight reviews without clear next action.

## How to diagnose where the problem really is

When a cycle feels stuck, teams often focus on the most visible symptom. That can be misleading.

```mermaid
flowchart TD
  actionStall[Next action feels stuck] --> weakLearnings[Weak learnings]
  weakLearnings --> poorExperiment[Poor experiment]
  poorExperiment --> fuzzyHypothesis[Fuzzy hypothesis]
  fuzzyHypothesis --> unclearAssumption[Unclear assumption]
```

In other words, if the team cannot pick a clear next action, the real issue may be weak learnings. If the learnings feel weak, the real issue may be a poor experiment. If the experiment feels noisy, the real issue may be a fuzzy hypothesis. And if the hypothesis is fuzzy, the real issue may be an unclear assumption.

That is why recovery should begin by locating the first weak checkpoint, not just the latest visible problem.

## Recovery sequence

1. Identify the failed checkpoint in the cycle.
2. Use the relevant quality standard or rubric.
3. Redefine owner, timeline, and expected output.
4. Re-run only the minimum required step.

## Branching recovery logic

### If the team is unclear about what it is testing

Return to assumption selection and tighten scope.

### If the team is active but not learning

Review the hypothesis and experiment criteria. This is often experiment theater.

### If the team has data but weak conclusions

Rework the learning capture step and use the rubric before moving to synthesis.

### If the team keeps discussing but not deciding

Use the decision checklist and force clarity on confidence, trade-offs, ownership, and next move.

The important point is that each branch sends the team to the smallest meaningful correction. Recovery should tighten the loop, not restart the whole project unless the team truly discovered the original frame was wrong.

## Escalate when

- A team misses two consecutive cycle checkpoints.
- Confidence remains low after repeated tests.
- Decisions are repeatedly deferred.

## Recovery mindset

The best recovery conversations are specific and non-dramatic. Avoid broad statements like “the whole process is broken.” Instead ask:

- What stage weakened first?
- What artifact is not good enough yet?
- What is the smallest correction that would restore clarity?

That keeps recovery practical and helps teams regain momentum faster.

## Definition of done

- Root cause is identified at the first weak checkpoint.
- Recovery action has clear owner and timebox.
- Team re-enters the cycle with explicit quality gates.

## Next step

Return to [Run Learning Cycles in SwiftCNS](../run-learning-cycles/README.md) and apply the smallest fix that restores clarity. For step-specific recovery, jump directly to:

- [02 - Identify Critical Assumptions](../run-learning-cycles/02-identify-critical-assumptions.md)
- [03 - Form Testable Hypotheses](../run-learning-cycles/03-form-testable-hypotheses.md)
- [04 - Design and Run Experiments](../run-learning-cycles/04-design-run-experiments.md)
- [05 - Extract Key Learnings and Insights](../run-learning-cycles/05-extract-key-learnings.md)
