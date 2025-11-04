# 02 — Identify Critical Assumptions

> **Purpose**: Find the assumptions that must be true for your solution to succeed
> **Outcome**: Have a prioritized list of critical assumptions that need validation
> **Audience**: PM / Dev / Both
> **Time**: 2-3 hours
> **Prerequisites**: [01 — Idea / Problem](01-idea-problem.md)

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Distinguish between assumptions and facts
2. Identify critical assumptions that must be true for success
3. Prioritize assumptions by risk and impact
4. Categorize assumptions (user, technical, business, etc.)
5. Prepare assumptions for hypothesis formation

## Jobs-to-Be-Done

- **When**: I have a clear problem statement and value proposition
- **I want**: To identify what must be true for my solution to work
- **So that**: I can validate the riskiest assumptions first

## Inputs

- Problem statement from [01 — Idea / Problem](01-idea-problem.md)
- Value proposition
- Jobs-to-Be-Done statements
- Understanding of your proposed solution

## Activities

### 1. List All Assumptions

Start by listing everything you're assuming:

**Categories of Assumptions**:
- **User Assumptions**: About users' needs, behaviors, preferences
- **Technical Assumptions**: About what's possible to build
- **Business Assumptions**: About market, pricing, competition
- **Value Assumptions**: About the value proposition and user willingness to pay

**Example Assumptions**:
- Users will use an AI-powered retrospective tool
- Users will pay $X/month for this tool
- We can build AI that generates useful insights
- Teams will adopt this tool quickly
- Competitors won't copy our approach

> 💡 **Tip**: Don't filter yet. List everything you're assuming, even if it seems obvious.

### 2. Identify Critical Assumptions

An assumption is critical if:
- **If false, the solution fails** (high risk)
- **Uncertainty is high** (we don't know if it's true)
- **Impact is high** (affects the entire value proposition)

**Questions to Ask**:
- If this assumption is false, does the product fail?
- Do we have evidence this is true?
- How confident are we about this assumption?

### 3. Prioritize by Risk

Create a risk matrix:

**High Risk / High Impact** → Critical (test first)
**High Risk / Low Impact** → Test if time allows
**Low Risk / High Impact** → Monitor
**Low Risk / Low Impact** → Track but don't prioritize

> 🎯 **Goal**: Focus on high-risk, high-impact assumptions first.

### 4. Categorize Assumptions

Group assumptions by type:

**User Assumptions**:
- Users have the problem we think they do
- Users will use our solution
- Users will pay for our solution

**Technical Assumptions**:
- We can build the solution
- The solution will perform as expected
- The solution will scale

**Business Assumptions**:
- Market is large enough
- Competition won't block us
- Pricing model works

### 5. Document Assumptions

Create an assumptions list:

```
Assumption: [What you're assuming]
Category: [User/Technical/Business/Value]
Risk Level: [High/Medium/Low]
Impact: [High/Medium/Low]
Evidence: [What evidence do you have?]
Test Needed: [How will you test this?]
```

## Apply It Now

**Task**: Create your critical assumptions list

1. List all assumptions you're making about your solution
2. Identify which are critical (high risk, high impact)
3. Prioritize assumptions by risk and impact
4. Categorize assumptions by type (user, technical, business)
5. Document your top 5-10 critical assumptions

**Artifact**: A critical assumptions list with:
- All assumptions listed
- Critical assumptions identified
- Risk and impact assessment
- Categorization
- Priority ranking

## Artifacts

You'll create:
- Complete assumptions list
- Critical assumptions document
- Risk and impact matrix
- Prioritized assumptions list

## Worked Example

**Situation**: Retrospective tool product idea

**Assumptions List**:
```
1. Assumption: Teams will use an AI-powered retrospective tool
   Category: User
   Risk: High
   Impact: High
   Evidence: None (assumption)
   Test Needed: Landing page with mockups, measure interest

2. Assumption: We can build AI that generates useful insights
   Category: Technical
   Risk: High
   Impact: High
   Evidence: Some AI tools exist, but not for retrospectives
   Test Needed: Build MVP with basic AI, test with real retrospectives

3. Assumption: Users will pay $10/month for this tool
   Category: Business
   Risk: Medium
   Impact: High
   Evidence: Competitors charge $5-15/month
   Test Needed: Pricing page with signup, measure conversion

4. Assumption: Teams will adopt the tool quickly
   Category: User
   Risk: Medium
   Impact: Medium
   Evidence: Teams adopt Slack, Jira quickly
   Test Needed: User interviews about adoption timeline

5. Assumption: Competitors won't copy our approach
   Category: Business
   Risk: Low
   Impact: Medium
   Evidence: Market moves fast, but we have time
   Test Needed: Monitor competitors
```

**Critical Assumptions** (top 3):
1. Teams will use an AI-powered retrospective tool
2. We can build AI that generates useful insights
3. Users will pay $10/month for this tool

## Checklist

Before proceeding to the next chapter, verify:
- [ ] All assumptions are listed
- [ ] Critical assumptions are identified
- [ ] Assumptions are prioritized by risk and impact
- [ ] Assumptions are categorized
- [ ] Top 5-10 critical assumptions are documented

## Self-Assessment

1. **What makes an assumption critical?** (Select all)
   - [ ] If false, the solution fails ✓
   - [ ] Uncertainty is high ✓
   - [ ] Impact is high ✓
   - [ ] It's hard to test

2. **Which assumptions should you test first?**
   - [ ] High risk, high impact ✓
   - [ ] Low risk, high impact
   - [ ] High risk, low impact

3. **What categories should assumptions be grouped into?** (Select all)
   - [ ] User ✓
   - [ ] Technical ✓
   - [ ] Business ✓
   - [ ] Value ✓

## Exit Criteria

You're ready to proceed when:
- [ ] All assumptions are listed
- [ ] Critical assumptions are identified
- [ ] Assumptions are prioritized
- [ ] Top 5-10 critical assumptions are documented
- [ ] You're ready to form hypotheses about these assumptions

## Dependencies & Next Steps

### Prerequisites Completed
- [01 — Idea / Problem](01-idea-problem.md) - Problem statement and value proposition

### Next Steps
- Proceed to [03 — Form Testable Hypotheses](03-form-testable-hypotheses.md) to create testable statements about your critical assumptions

### What This Enables

Identifying critical assumptions enables:
- Focused validation efforts
- Risk mitigation
- Clear hypothesis formation
- Efficient experiment design

---

> 💡 **Tip**: You'll have many assumptions. Focus on the critical ones first.
> ⚠️ **Warning**: Don't assume your assumptions are obvious. Write them down explicitly.
