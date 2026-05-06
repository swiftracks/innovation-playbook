# Cadence and Stage Gates

**Purpose**: Reduce cycle delays by enforcing clear operating rhythm and quality checkpoints.

Cadence is what keeps learning from becoming sporadic. Stage gates are what keep quality from drifting. Together, they give teams enough structure to move consistently without turning the work into bureaucracy.

## Recommended rhythm

- Weekly cycle planning.
- Mid-cycle evidence check.
- End-cycle decision review.

This rhythm can flex based on context, but the pattern should remain:

- begin with clarity,
- check for signal before the cycle drifts,
- end with a decision or explicit next move.

## Stage gates

1. **Gate A - Assumptions ready**
   - Top assumptions prioritized.
   - Hypothesis candidates defined.
2. **Gate B - Experiments ready**
   - Success criteria and owners confirmed.
   - Timeline and audience defined.
3. **Gate C - Learnings ready**
   - Evidence-backed learnings documented.
   - Confidence and uncertainty stated.
4. **Gate D - Decision ready**
   - Insights synthesized.
   - Decision and owner explicit.

```mermaid
flowchart LR
  gateA[Gate A Assumptions ready] --> step02[Step 02 Identify Critical Assumptions]
  step02 --> gateB[Gate B Experiments ready]
  gateB --> step03[Step 03 Form Testable Hypotheses]
  step03 --> step04[Step 04 Design and Run Experiments]
  step04 --> gateC[Gate C Learnings ready]
  gateC --> step05[Step 05 Extract Key Learnings]
  step05 --> gateD[Gate D Decision ready]
  gateD --> step06[Step 06 Synthesize Insights to Decision]
```

This mapping helps program managers avoid reviewing teams too generically. Each gate should be tied to a real workflow stage and a visible artifact, not just a status update.

## Why stage gates matter

Stage gates are not meant to slow teams down. They are meant to stop weak work from quietly moving downstream.

Without stage gates, teams often progress by momentum alone. A weak assumption turns into a weak hypothesis, then a weak experiment, then a low-confidence decision. By the time the issue is visible, the team has already lost time.

With stage gates, quality becomes visible earlier.

## How to use stage gates well

- Use them as review standards, not as rigid ceremony.
- Keep them focused on decision readiness, not on paperwork.
- Apply them consistently enough that teams know what “ready” means.
- Escalate early when a team repeatedly misses the same kind of gate.

## Escalation triggers

- No cycle progress in one week.
- Repeated low-quality artifacts.
- Decision delayed beyond agreed gate window.

## What good looks like

A healthy program rhythm feels predictable without feeling heavy.

Teams should know:

- when they will be reviewed,
- what quality bar they are being held to,
- what happens if a cycle gets stuck,
- and who helps them recover if that happens.

## Common mistake

The most common program mistake is turning cadence into status reporting. A good operating rhythm is not just about hearing updates. It is about helping teams move from weak signals to stronger decisions with less drift and less delay.

## Next step

Continue to [Mentor Collaboration Model](mentor-collaboration-model.md).
