# 11 — Experiments

> **Purpose**: Run experiments to test improvements and optimize
> **Outcome**: Have a process for testing improvements with data
> **Audience**: PM / Dev / Both
> **Time**: 1-2 weeks per experiment
> **Prerequisites**: [09 — Private Beta](09-private-beta.md), [10 — Instrumentation](10-instrumentation.md) (recommended)

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Design experiments to test improvements
2. Set up A/B tests or feature flags
3. Run experiments with real users
4. Analyze experiment results
5. Make data-driven decisions about changes

## Jobs-to-Be-Done

- **When**: I have launched MVP and want to test improvements
- **I want**: To run experiments to test changes
- **So that**: I can make data-driven decisions about what to improve

## Inputs

- Launched MVP from [09 — Private Beta](09-private-beta.md)
- Instrumentation setup (recommended)
- Understanding of what to test
- Access to experiment tools

## Activities

### 1. Design Experiments

**Define Experiment Goals**:
- What do you want to test?
- What hypothesis are you testing?
- What metric will you measure?
- What success looks like?

**Example Experiment**:
```
Goal: Test if improved AI prompts increase insight quality
Hypothesis: If we improve AI prompts, then users will rate insights higher
Metric: Insight quality rating (1-5 scale)
Success: Average rating increases from 3.5 to 4.0+
```

### 2. Set Up Experiment Infrastructure

**Choose Experiment Method**:
- **A/B Test**: Test two versions
- **Feature Flag**: Toggle features
- **Multivariate**: Test multiple variations
- **Simple**: Manual split

**Tools**:
- **LaunchDarkly**: Feature flags
- **Optimizely**: A/B testing
- **Custom**: Build your own
- **Simple**: Manual split

> 💡 **Tip**: Start simple. Use feature flags or manual split for MVP.

### 3. Implement Experiments

**Feature Flag Implementation**:
```javascript
// Check feature flag
if (featureFlag.isEnabled('improved_ai_prompts', userId)) {
  // Use improved prompts
  return generateInsightsWithImprovedPrompts(feedback);
} else {
  // Use original prompts
  return generateInsightsWithOriginalPrompts(feedback);
}
```

**A/B Test Implementation**:
```javascript
// Assign user to variant
const variant = experiment.getVariant(userId, 'ai_prompts_test');
if (variant === 'improved') {
  return generateInsightsWithImprovedPrompts(feedback);
} else {
  return generateInsightsWithOriginalPrompts(feedback);
}
```

### 4. Run Experiments

**Experiment Steps**:
1. Set up experiment
2. Launch to users
3. Monitor results
4. Collect data
5. Analyze results

**Duration**:
- **Short**: 1 week (quick feedback)
- **Medium**: 2 weeks (more data)
- **Long**: 4 weeks (statistical significance)

> 📝 **Note**: Run experiments long enough to get reliable data.

### 5. Analyze Results

**Compare Metrics**:
- Control group vs. treatment group
- Before vs. after
- Variant A vs. variant B

**Statistical Significance**:
- Sample size sufficient?
- Results statistically significant?
- Difference meaningful?

**Example Analysis**:
```
Experiment: Improved AI Prompts
Control: Original prompts (n=50, avg rating=3.5)
Treatment: Improved prompts (n=50, avg rating=4.2)
Result: Statistically significant (p<0.05)
Decision: Roll out improved prompts
```

## Apply It Now

**Task**: Run your first experiment

1. Design experiment (goal, hypothesis, metric)
2. Set up experiment infrastructure (feature flags or A/B test)
3. Implement experiment (code changes)
4. Run experiment (launch to users)
5. Analyze results (compare metrics)
6. Make decision (roll out or roll back)

**Artifact**: An experiment plan with:
- Experiment goal and hypothesis
- Experiment design
- Implementation details
- Results analysis
- Decision and next steps

## Artifacts

You'll create:
- Experiment plans
- Experiment implementations
- Experiment results
- Analysis reports
- Decision documents

## Worked Example

**Situation**: Testing improved AI prompts for retrospective tool

**Experiment Design**:
```
Goal: Test if improved AI prompts increase insight quality
Hypothesis: If we improve AI prompts, then users will rate insights higher
Metric: Insight quality rating (1-5 scale)
Success: Average rating increases from 3.5 to 4.0+
Duration: 2 weeks
```

**Implementation**:
```javascript
// Feature flag implementation
function generateInsights(feedback) {
  const useImprovedPrompts = featureFlag.isEnabled(
    'improved_ai_prompts',
    userId
  );
  
  if (useImprovedPrompts) {
    return generateInsightsWithImprovedPrompts(feedback);
  } else {
    return generateInsightsWithOriginalPrompts(feedback);
  }
}
```

**Results**:
```
Control: Original prompts
- Users: 50
- Average rating: 3.5
- Standard deviation: 0.8

Treatment: Improved prompts
- Users: 50
- Average rating: 4.2
- Standard deviation: 0.7

Statistical test: t-test
- p-value: 0.02 (significant)
- Effect size: 0.7 (medium)
```

**Decision**: Roll out improved prompts to all users

## Checklist

Before proceeding to the next chapter, verify:
- [ ] Experiment is designed
- [ ] Experiment infrastructure is set up
- [ ] Experiment is implemented
- [ ] Experiment is running
- [ ] Results are analyzed
- [ ] Decision is made

## Self-Assessment

1. **What experiment method is good for MVP?**
   - [ ] Complex A/B testing platform
   - [ ] Feature flags or simple split ✓
   - [ ] Manual testing only

2. **What should you analyze?** (Select all)
   - [ ] Metrics ✓
   - [ ] Statistical significance ✓
   - [ ] Effect size ✓
   - [ ] Only positive results

3. **What should you do after experiment?**
   - [ ] Always roll out changes
   - [ ] Make data-driven decision ✓
   - [ ] Ignore results

## Exit Criteria

You're ready to proceed when:
- [ ] Experiment is running
- [ ] Results are analyzed
- [ ] Decision is made
- [ ] You're ready to iterate

## Dependencies & Next Steps

### Prerequisites Completed
- [09 — Private Beta](09-private-beta.md) - Launched MVP
- [10 — Instrumentation](10-instrumentation.md) - Instrumentation setup (recommended)

### Next Steps
- Proceed to [12 — Feedback Ops](12-feedback-ops.md) to establish feedback loops
- OR iterate based on experiment results

### What This Enables

Experiments enable:
- Data-driven improvements
- Risk mitigation
- Optimization
- Continuous learning

---

> 💡 **Tip**: Start simple. Use feature flags or manual split for MVP.
> 📝 **Note**: Experiments are for learning. Don't expect perfect results.
