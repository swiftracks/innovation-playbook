# Cycle Anatomy

**Purpose**: Break the loop into executable checkpoints.

## Who this is for

- Operators who need clear stage-by-stage execution guidance.
- Reviewers who need to diagnose exactly where quality dropped.
- Program teams standardizing checkpoint expectations.

This page is useful when the team understands the loop conceptually but needs a clearer sense of what each stage is actually doing. Each checkpoint exists to reduce a different kind of uncertainty.

## Checkpoint 1: Assumption selection

- Pick the highest-risk assumption.
- Define why it matters now.
- Set a decision deadline.

This is where the cycle gains focus. If this checkpoint is weak, everything downstream gets noisier. The team should leave this step knowing exactly what belief is under pressure and why it matters enough to test now.

## Checkpoint 2: Hypothesis and experiment design

- Convert assumption into one testable hypothesis.
- Define signal criteria before running the test.
- Assign owner and run window.

This is where the team turns uncertainty into a real test. A strong checkpoint here makes the rest of the cycle easier. A weak checkpoint usually creates activity without usable evidence.

## Checkpoint 3: Learning capture

- Document what happened and what evidence supports it.
- Tag confidence level.
- Link the learning to the original assumption.

This is the point where teams either gain clarity or start drifting into interpretation. The discipline here is simple but important: capture what changed in understanding, not just what happened during execution.

## Checkpoint 4: Insight synthesis

- Combine relevant learnings.
- Clarify implications, options, and trade-offs.

This checkpoint gives the learnings meaning. It is where the team steps back and asks, "What does this actually imply for the bet, the roadmap, or the next move?" A synthesis that only restates evidence is still incomplete.

## Checkpoint 5: Decision

- Decide: go, iterate, pivot, or stop.
- Document owner, rationale, and next test.

This is where the loop closes. If the team does not make an explicit decision, the cycle stays open and momentum leaks out. A good decision does not remove uncertainty completely. It creates a responsible next move.

## How the checkpoints connect

Each checkpoint should make the next one easier:

- a sharper assumption creates a stronger hypothesis,
- a stronger hypothesis creates a cleaner experiment,
- a cleaner experiment creates more trustworthy learnings,
- stronger learnings make synthesis easier,
- better synthesis makes decisions faster and more accountable.

If a team is struggling late in the cycle, it is often worth checking whether the breakdown actually happened earlier.

## What good looks like

Good cycle anatomy is visible when a team can move from one checkpoint to the next without re-explaining the whole project every time. The artifacts should carry enough clarity that the work compounds instead of resetting.

## Definition of done

- Each checkpoint has a visible artifact with clear owner.
- Teams can explain why each checkpoint exists before moving on.
- Review conversations use checkpoint quality, not generic status updates.

## Next step

Read [Quality Standards](quality-standards.md).
