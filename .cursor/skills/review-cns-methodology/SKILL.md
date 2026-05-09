---
name: review-cns-methodology
description: Review CNS playbook content for methodology rigor, evidence quality, and decision-readiness regressions. Use when auditing or reviewing changes to innovation-playbook pages.
---

# Review CNS Methodology

Use this skill to run a focused quality review for playbook content.
Be strict on reasoning quality and evidence discipline, flexible on output form.

## Review Priorities

1. Correctness of methodology
2. Evidence and confidence rigor
3. Decision relevance
4. Runtime alignment (no unsupported capability claims)
5. Contributor readability and clarity

## Review Method

1. Stage integrity
   - Check that stages are correctly represented.
   - Check that assumptions, hypotheses, experiments, learnings, insights, and decisions are not conflated.

2. Evidence rigor
   - Verify criteria are declared before outcomes.
   - Verify evidence expectations are concrete.
   - Flag activity-as-evidence language.

3. Decision readiness
   - Verify the page leads to explicit next decisions.
   - Flag pages that stop at "capture insights" without action path.

4. Contract alignment
   - Verify claims align with `cns-ui`, `csn-backend`, and `cns-prompts`.
   - Mark roadmap-only statements as planned.

5. Contribution quality
   - Ensure changes are scoped and understandable.
   - Ensure links/navigation are updated where needed.

6. Reasoning over format
   - Reject rigid formatting compliance as a quality proxy.
   - Allow adaptive structure if reasoning, evidence, and decision quality are strong.

7. Capture evidence integrity (for workflow tutorials)
   - Verify each procedural step maps to captured app behavior.
   - Verify screenshot references are deterministic and step-linked.
   - Flag any inferred step that has no capture evidence.

## Critical Thinking Scoring Lens

Score each axis from 1 to 5:

1. Argument quality
   - Is the logic coherent and non-circular?
2. Falsifiability
   - Are claims testable and criteria explicit?
3. Evidence interpretation
   - Are conclusions proportional to signal strength?
4. Decision relevance
   - Does content clearly support next decisions?
5. Runtime safety
   - Are functional claims consistent with current CNS contracts?

## Output Format

When reporting findings, use:

- Severity: critical, major, minor
- Issue: concise description
- Why it matters: impact on learning quality or decision quality
- Suggested fix: concrete and minimal

## Pass Criteria

The page passes only when:

- methodology is stage-correct,
- evidence standards are explicit,
- decision path is explicit,
- and claims are runtime-valid.

## Definition of Done

Review is complete when findings are prioritized by impact, mapped to concrete fixes, and sufficient for an editor to resolve issues without interpretation gaps.
