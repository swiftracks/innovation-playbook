# 05 — Extract Key Learnings

> **Purpose**: Analyze experiment results and extract actionable insights
> **Outcome**: Have clear learnings that inform your go/no-go decision
> **Audience**: PM / Dev / Both
> **Time**: 2-4 hours per experiment
> **Prerequisites**: [04 — Design & Run Experiments](04-design-run-experiments.md)

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Analyze quantitative and qualitative data from experiments
2. Identify patterns and insights in results
3. Distinguish between validated and invalidated hypotheses
4. Extract actionable learnings
5. Document learnings for decision-making

## Jobs-to-Be-Done

- **When**: I have completed experiments and collected data
- **I want**: To analyze results and extract insights
- **So that**: I can make informed decisions about what to build

## Inputs

- Experiment results from [04 — Design & Run Experiments](04-design-run-experiments.md)
- Data collected (quantitative and qualitative)
- Success criteria for each hypothesis
- Experiment notes and observations

## Activities

### 1. Analyze Quantitative Data

Review quantitative metrics:

**Compare to Success Criteria**:
- Did the metric meet the threshold?
- Was the sample size sufficient?
- Are there any anomalies?

**Calculate Key Metrics**:
- Conversion rates
- Completion rates
- Time spent
- Usage patterns
- Drop-off points

**Example Analysis**:
```
Hypothesis: 30% conversion rate
Result: 23.3% conversion rate
Sample: 120 visitors
Conclusion: Hypothesis invalidated (below threshold)
```

> 💡 **Tip**: Look for patterns, not just averages. Segment data if possible.

### 2. Analyze Qualitative Data

Review qualitative feedback:

**User Feedback**:
- What did users say?
- What patterns emerge?
- What surprised you?

**Interview Responses**:
- Common themes
- Pain points mentioned
- Positive reactions
- Concerns or objections

**Survey Responses**:
- Open-ended responses
- Rating patterns
- Suggestions

> 📝 **Note**: Qualitative data explains the "why" behind quantitative results.

### 3. Identify Patterns

Look for patterns across data:

**Quantitative Patterns**:
- Trends over time
- Segments with different behavior
- Drop-off points
- Usage patterns

**Qualitative Patterns**:
- Common themes in feedback
- Repeated concerns
- Consistent positive reactions
- Emerging use cases

**Example Patterns**:
- Users who signed up: "Looks useful, would try it"
- Users who didn't sign up: "Not sure I'd use it regularly"
- Pattern: Interest exists but commitment is low

### 4. Determine Hypothesis Status

For each hypothesis, determine:

**Validated**:
- Metric met or exceeded threshold
- Sample size sufficient
- Data is reliable

**Invalidated**:
- Metric below threshold
- Sample size sufficient
- Data is reliable

**Inconclusive**:
- Sample size insufficient
- Data is unreliable
- Need more data

**Example**:
```
Hypothesis 1: Validated (conversion rate: 35%, threshold: 30%)
Hypothesis 2: Invalidated (conversion rate: 23%, threshold: 30%)
Hypothesis 3: Inconclusive (only 20 visitors, need 100)
```

### 5. Extract Learnings

Document key learnings:

**Learning Format**:
```
Learning: [What you learned]
Evidence: [Data that supports it]
Impact: [How it affects your decision]
Action: [What to do next]
```

**Example**:
```
Learning: Users are interested but not committed
Evidence: 23% conversion rate (below 30% threshold), qualitative feedback shows hesitation
Impact: Value proposition needs refinement before building
Action: Refine value proposition, test again, or pivot
```

### 6. Document Learnings

Create a learnings summary:

**Structure**:
- Hypothesis tested
- Result (validated/invalidated/inconclusive)
- Key metrics
- Qualitative insights
- Patterns identified
- Learnings extracted
- Implications for decision

## Apply It Now

**Task**: Analyze your experiment results and extract learnings

1. Analyze quantitative data against success criteria
2. Review qualitative feedback for patterns
3. Identify patterns across data
4. Determine hypothesis status (validated/invalidated/inconclusive)
5. Extract key learnings
6. Document learnings in a summary

**Artifact**: A learnings summary document with:
- Hypothesis results
- Data analysis
- Patterns identified
- Learnings extracted
- Implications for decision

## Artifacts

You'll create:
- Data analysis document
- Patterns analysis
- Learnings summary
- Hypothesis status report
- Implications document

## Worked Example

**Situation**: Analyzing results from retrospective tool experiments

**Hypothesis 1 Analysis**:
```
Hypothesis: Teams will use AI-powered retrospective tool (30% conversion)
Result: 23.3% conversion rate (120 visitors, 28 signups)
Status: Invalidated
Quantitative: Below threshold
Qualitative: "Looks interesting but not sure I'd use it regularly"
Pattern: Interest exists but commitment is low
Learning: Value proposition needs refinement
Impact: Need to clarify ongoing value before building
Action: Refine value proposition, test again
```

**Hypothesis 2 Analysis**:
```
Hypothesis: Can build AI that generates useful insights (70% usefulness)
Result: 75% usefulness rating (8 out of 10 teams)
Status: Validated
Quantitative: Above threshold
Qualitative: "Insights were helpful", "Would use this"
Pattern: Technical feasibility confirmed
Learning: AI approach is viable
Impact: Can proceed with AI-powered features
Action: Proceed with AI development
```

**Overall Learnings**:
- Technical approach is viable (validated)
- User interest needs refinement (invalidated)
- Need to clarify ongoing value proposition
- Consider pivoting to higher-commitment use case

## Checklist

Before proceeding to the next chapter, verify:
- [ ] Quantitative data is analyzed
- [ ] Qualitative feedback is reviewed
- [ ] Patterns are identified
- [ ] Hypothesis status is determined
- [ ] Key learnings are extracted
- [ ] Learnings are documented

## Self-Assessment

1. **What should you compare results to?**
   - [ ] Success criteria ✓
   - [ ] Industry benchmarks
   - [ ] Your intuition

2. **What should you look for in qualitative data?** (Select all)
   - [ ] Patterns ✓
   - [ ] Themes ✓
   - [ ] Surprises ✓
   - [ ] Only positive feedback

3. **What determines if a hypothesis is validated?**
   - [ ] Metric meets threshold ✓
   - [ ] Sample size sufficient ✓
   - [ ] Data is reliable ✓
   - [ ] You like the result

## Exit Criteria

You're ready to proceed when:
- [ ] Experiment results are analyzed
- [ ] Hypothesis status is determined
- [ ] Key learnings are extracted
- [ ] Learnings are documented
- [ ] You're ready to make a decision

## Dependencies & Next Steps

### Prerequisites Completed
- [04 — Design & Run Experiments](04-design-run-experiments.md) - Experiment results

### Next Steps
- Proceed to [06 — Synthesize Insights → Decision](06-synthesize-insights-decision.md) to make a go/no-go decision

### What This Enables

Extracting learnings enables:
- Data-driven decisions
- Clear understanding of what works
- Identification of what needs refinement
- Informed go/no-go decisions

---

> 💡 **Tip**: Look for patterns, not just averages. Patterns reveal insights.
> 📝 **Note**: Invalidated hypotheses are valuable. They tell you what not to build.
