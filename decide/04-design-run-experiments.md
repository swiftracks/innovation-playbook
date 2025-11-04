# 04 — Design & Run Experiments

> **Purpose**: Design and execute experiments to test your hypotheses
> **Outcome**: Have validated or invalidated hypotheses with data
> **Audience**: PM / Dev / Both
> **Time**: 1-2 weeks per experiment
> **Prerequisites**: [03 — Form Testable Hypotheses](03-form-testable-hypotheses.md)

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Design experiments that test specific hypotheses
2. Choose appropriate experiment types for different hypotheses
3. Set up experiments with proper controls and metrics
4. Run experiments efficiently with minimal resources
5. Collect reliable data for analysis

## Jobs-to-Be-Done

- **When**: I have testable hypotheses ready
- **I want**: To design and run experiments to test them
- **So that**: I can validate or invalidate assumptions with data

## Inputs

- Testable hypotheses from [03 — Form Testable Hypotheses](03-form-testable-hypotheses.md)
- Success criteria for each hypothesis
- Access to users or test environment
- Time and resources for experimentation

## Activities

### 1. Choose Experiment Types

Select the right experiment type for your hypothesis:

**User Hypotheses** (about user behavior):
- **Landing Page Test**: Measure interest with mockups
- **Concierge Test**: Manual service that mimics product
- **Wizard of Oz**: Fake backend, real experience
- **Smoke Test**: Minimal version to test core assumption

**Technical Hypotheses** (about feasibility):
- **Prototype Test**: Build minimal version to test feasibility
- **Technical Spike**: Proof of concept for specific technology
- **Performance Test**: Test scalability or performance

**Business Hypotheses** (about market):
- **Pricing Test**: Test willingness to pay
- **Market Test**: Test market size or demand
- **Competitive Test**: Test competitive position

> 💡 **Tip**: Start with the cheapest, fastest test that gives you reliable data.

### 2. Design Experiment Plan

For each hypothesis, create an experiment plan:

```
Experiment: [Name]
Hypothesis: [Full hypothesis statement]
Type: [Experiment type]
Method:
  - Setup: [What you'll create]
  - Execution: [How you'll run it]
  - Metrics: [What you'll measure]
  - Timeline: [How long it will take]
Resources Needed:
  - Time: [Hours/days]
  - People: [Who's involved]
  - Tools: [What tools/services]
  - Budget: [Cost if any]
Success Criteria:
  - Metric: [What to measure]
  - Threshold: [Success threshold]
  - Sample Size: [How many needed]
```

### 3. Set Up Experiments

**Minimal Setup** (recommended):
- Use no-code tools when possible
- Create landing pages with mockups
- Use survey tools for feedback
- Leverage existing platforms (Google Forms, Typeform)

**Example Setup**:
- Landing page: Carrd, Webflow, or simple HTML
- Analytics: Google Analytics, Mixpanel
- Forms: Google Forms, Typeform
- Email: Mailchimp, ConvertKit

> 🎯 **Goal**: Set up experiments in hours or days, not weeks.

### 4. Run Experiments

**Execution Steps**:
1. Set up tracking and analytics
2. Launch experiment
3. Drive traffic (if needed)
4. Collect data
5. Monitor for issues

**Driving Traffic**:
- Share with your network
- Post on relevant communities
- Use social media
- Run ads (if budget allows)
- Email potential users

> 💡 **Tip**: Start small. Get 10-20 data points first, then scale if needed.

### 5. Collect Data

Track metrics systematically:

**Quantitative Metrics**:
- Conversion rates
- Signup rates
- Usage metrics
- Time spent
- Completion rates

**Qualitative Metrics**:
- User feedback
- Interview responses
- Survey responses
- Support requests

> 📝 **Note**: Collect both quantitative and qualitative data for richer insights.

## Apply It Now

**Task**: Design and run your first experiment

1. Choose your top priority hypothesis
2. Select an appropriate experiment type
3. Create an experiment plan with method, resources, and success criteria
4. Set up the experiment (use minimal tools)
5. Run the experiment and collect data
6. Document results for analysis

**Artifact**: An experiment plan and results document with:
- Experiment design
- Setup details
- Execution notes
- Data collected
- Initial observations

## Artifacts

You'll create:
- Experiment plans
- Experiment setup documentation
- Data collection logs
- Experiment results
- Initial observations

## Worked Example

**Situation**: Testing hypothesis about teams using AI-powered retrospective tool

**Experiment Plan**:
```
Experiment: Landing Page Interest Test
Hypothesis: We believe teams will use an AI-powered retrospective tool. If we create a landing page with mockups, then at least 30% of visitors will sign up for early access. We'll know this is true when we see 30%+ conversion rate after 100 visitors.

Type: Landing Page Test
Method:
  - Setup: Create landing page with mockups, signup form
  - Execution: Share link, drive traffic, measure signups
  - Metrics: Conversion rate (signups/visitors)
  - Timeline: 1 week
Resources Needed:
  - Time: 4 hours setup, ongoing monitoring
  - People: 1 person (PM)
  - Tools: Carrd (landing page), Google Analytics (tracking)
  - Budget: $0 (using free tools)
Success Criteria:
  - Metric: Signup conversion rate
  - Threshold: 30% or higher
  - Sample Size: 100 visitors minimum
```

**Results**:
- Visitors: 120
- Signups: 28
- Conversion Rate: 23.3%
- Result: **Hypothesis invalidated** (below 30% threshold)

**Observations**:
- Interest is lower than expected
- May need to refine value proposition
- Some users commented: "Looks interesting but not sure I'd use it"
- Need to dig deeper into why conversion is lower

## Checklist

Before proceeding to the next chapter, verify:
- [ ] Experiment is designed with clear method
- [ ] Success criteria are defined
- [ ] Experiment is set up and running
- [ ] Data collection is in place
- [ ] You have enough data points (sample size)
- [ ] Results are documented

## Self-Assessment

1. **What experiment type is best for testing user interest?**
   - [ ] Technical Spike
   - [ ] Landing Page Test ✓
   - [ ] Performance Test

2. **What should you prioritize in experiment setup?**
   - [ ] Perfect design
   - [ ] Speed and simplicity ✓
   - [ ] Complex features

3. **What data should you collect?** (Select all)
   - [ ] Quantitative metrics ✓
   - [ ] Qualitative feedback ✓
   - [ ] Both ✓

## Exit Criteria

You're ready to proceed when:
- [ ] At least one experiment is complete
- [ ] You have reliable data (met sample size)
- [ ] Results are documented
- [ ] You're ready to analyze learnings

## Dependencies & Next Steps

### Prerequisites Completed
- [03 — Form Testable Hypotheses](03-form-testable-hypotheses.md) - Testable hypotheses

### Next Steps
- Proceed to [05 — Extract Key Learnings](05-extract-key-learnings.md) to analyze your experiment results

### What This Enables

Running experiments enables:
- Data-driven validation
- Risk mitigation
- Clear go/no-go decisions
- Learning about users and market

---

> 💡 **Tip**: Start with the cheapest, fastest test. You can always run more sophisticated tests later.
> ⚠️ **Warning**: Don't wait for perfect data. Get enough to make a decision, then move forward.
