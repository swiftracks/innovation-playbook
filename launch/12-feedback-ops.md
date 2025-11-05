# 12 — Feedback Ops

**Purpose**: Establish feedback loops for continuous learning

**Outcome**: Have systematic processes for collecting and acting on feedback

**Audience**: PM / Dev / Both

**Time**: Ongoing (continuous process)

**Prerequisites**: [09 — Private Beta](09-private-beta.md)

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Set up feedback collection channels
2. Establish feedback review processes
3. Create feedback prioritization system
4. Build feedback action workflows
5. Close the feedback loop with users

## Jobs-to-Be-Done

- **When**: I have launched MVP and want to continuously improve
- **I want**: To collect and act on user feedback systematically
- **So that**: I can improve based on real user needs

## Inputs

- Launched MVP from [09 — Private Beta](09-private-beta.md)
- Instrumentation setup (if available)
- Understanding of what to learn
- Feedback collection tools

## Activities

### 1. Set Up Feedback Channels

**Feedback Channels**:
- **In-app feedback**: Feedback forms, surveys
- **Email**: Support email, feedback email
- **Interviews**: Regular user interviews
- **Surveys**: Periodic surveys
- **Support**: Support channels (Slack, email)

**Tools**:
- **Typeform**: Surveys and feedback forms
- **Intercom**: In-app messaging
- **Simple**: Email, forms, interviews

**Example Channels**:
```
1. In-app feedback form
   - Quick feedback button
   - Rating and comments

2. Support email
   - feedback@example.com
   - Support requests

3. Weekly user interviews
   - 30-minute sessions
   - 5-10 users per week

4. Monthly surveys
   - NPS survey
   - Feature requests
```

### 2. Establish Feedback Review Process

**Feedback Review Steps**:
1. Collect feedback
2. Review and categorize
3. Prioritize
4. Decide on action
5. Implement changes
6. Close the loop

**Review Frequency**:
- **Daily**: Critical issues
- **Weekly**: Regular review
- **Monthly**: Comprehensive review

**Example Review Process**:
```
Daily: Review critical issues and bugs
Weekly: Review feedback, categorize, prioritize
Monthly: Comprehensive review, trend analysis
```

### 3. Create Feedback Prioritization System

**Prioritization Framework**:
- **Impact**: How much does it matter?
- **Effort**: How hard is it to implement?
- **Frequency**: How often is it mentioned?
- **User Type**: Who is asking for it?

**Priority Levels**:
- **P0**: Critical (bugs, security)
- **P1**: High (major features, improvements)
- **P2**: Medium (nice-to-have features)
- **P3**: Low (future consideration)

**Example Prioritization**:
```
P0: Critical bugs, security issues
P1: High-impact features (mentioned by 5+ users)
P2: Medium-impact features (mentioned by 2-4 users)
P3: Low-impact features (mentioned by 1 user)
```

### 4. Build Feedback Action Workflows

**Action Workflows**:
- **Bug Reports**: Triage → Fix → Test → Deploy
- **Feature Requests**: Validate → Design → Build → Test → Deploy
- **UX Issues**: Analyze → Design → Test → Iterate
- **General Feedback**: Review → Categorize → Prioritize → Act

**Example Workflow**:
```
Feedback: "AI insights are not helpful"
1. Review: User rating low, feedback common
2. Categorize: Feature improvement
3. Prioritize: P1 (high impact, mentioned by 5+ users)
4. Action: Design improved AI prompts
5. Test: Run experiment (see Experiments chapter)
6. Deploy: Roll out if successful
7. Close loop: Notify user of improvement
```

### 5. Close the Feedback Loop

**Closing the Loop**:
- **Acknowledge**: Thank users for feedback
- **Update**: Let users know when changes are made
- **Follow up**: Ask for additional feedback
- **Celebrate**: Share improvements with users

**Example**:
```
User feedback: "AI insights are not helpful"
Response: "Thank you for the feedback. We're working on improving AI prompts and will test with you soon."
Update: "We've improved AI prompts based on your feedback. Please try it and let us know what you think!"
```

## Apply It Now

**Task**: Set up feedback operations for your MVP

1. Set up feedback channels (in-app, email, interviews)
2. Establish feedback review process (daily, weekly, monthly)
3. Create feedback prioritization system (impact, effort, frequency)
4. Build feedback action workflows (bug reports, feature requests)
5. Set up feedback loop closing (acknowledge, update, follow up)
6. Test feedback operations

**Artifact**: A feedback operations plan with:
- Feedback channels
- Review process
- Prioritization system
- Action workflows
- Loop closing process

## Artifacts

You'll create:
- Feedback channels setup
- Feedback review process
- Feedback prioritization system
- Feedback action workflows
- Feedback loop closing process

## Worked Example

**Situation**: Setting up feedback operations for retrospective tool

**Feedback Channels**:
```
1. In-app feedback form
   - Quick feedback button in app
   - Rating (1-5) and comments

2. Support email
   - feedback@example.com
   - Support requests

3. Weekly user interviews
   - 30-minute sessions
   - 5-10 users per week

4. Monthly surveys
   - NPS survey
   - Feature requests
```

**Review Process**:
```
Daily: Review critical issues and bugs
Weekly: Review feedback, categorize, prioritize
Monthly: Comprehensive review, trend analysis
```

**Prioritization System**:
```
P0: Critical bugs, security issues
P1: High-impact features (mentioned by 5+ users)
P2: Medium-impact features (mentioned by 2-4 users)
P3: Low-impact features (mentioned by 1 user)
```

**Action Workflow**:
```
Feedback: "AI insights are not helpful"
1. Review: User rating low, feedback common
2. Categorize: Feature improvement
3. Prioritize: P1
4. Action: Design improved AI prompts
5. Test: Run experiment
6. Deploy: Roll out if successful
7. Close loop: Notify user
```

**Results**:
- 50 feedback items collected in first month
- 15 P1 items prioritized
- 8 items implemented
- 5 items in progress
- User satisfaction increased

## Checklist

Before proceeding, verify:
- [ ] Feedback channels are set up
- [ ] Feedback review process is established
- [ ] Feedback prioritization system is created
- [ ] Feedback action workflows are built
- [ ] Feedback loop closing is set up
- [ ] Feedback operations are tested

## Self-Assessment

1. **What feedback channels should you use?** (Select all)
   - [ ] In-app feedback ✓
   - [ ] Email ✓
   - [ ] Interviews ✓
   - [ ] Surveys ✓

2. **How should you prioritize feedback?** (Select all)
   - [ ] By impact ✓
   - [ ] By effort ✓
   - [ ] By frequency ✓
   - [ ] By user type ✓

3. **What should you do after implementing feedback?**
   - [ ] Ignore users
   - [ ] Close the loop with users ✓
   - [ ] Wait for more feedback

## Exit Criteria

You're ready to proceed when:
- [ ] Feedback channels are set up
- [ ] Feedback review process is established
- [ ] Feedback prioritization system is created
- [ ] Feedback action workflows are built
- [ ] Feedback loop closing is set up
- [ ] You're continuously learning from feedback

## Dependencies & Next Steps

### Prerequisites Completed
- [09 — Private Beta](09-private-beta.md) - Launched MVP

### Next Steps
- Continue iterating based on feedback
- Return to [Decide What to Build](decide/index.md) if you need to pivot
- Return to [Build the MVP](build/index.md) if you need to add features
- Return to [Launch & Iterate](index.md) to continue iterating

### What This Enables

Feedback operations enable:
- Continuous learning
- User-driven improvements
- Product-market fit validation
- Long-term success

---

> 💡 **Tip**: Close the feedback loop. Users appreciate knowing their feedback matters.
> 📝 **Note**: Feedback operations are ongoing. They never really end.
