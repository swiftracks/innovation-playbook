# 10 — Instrumentation

> **Purpose**: Set up comprehensive tracking for usage and behavior
> **Outcome**: Have detailed analytics and understanding of user behavior
> **Audience**: PM / Dev / Both
> **Time**: 1-2 days
> **Prerequisites**: [09 — Private Beta](09-private-beta.md)

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Set up comprehensive analytics tracking
2. Track user behavior and journeys
3. Monitor feature usage
4. Set up event tracking
5. Create analytics dashboards

## Jobs-to-Be-Done

- **When**: I have launched MVP to beta users and need to understand usage
- **I want**: To track user behavior and feature usage
- **So that**: I can make data-driven decisions about improvements

## Inputs

- Launched MVP from [09 — Private Beta](09-private-beta.md)
- Understanding of what to track
- Access to analytics tools

## Activities

### 1. Set Up Analytics Tracking

**Choose Analytics Tool**:
- **Mixpanel**: Product analytics
- **Amplitude**: Product analytics
- **Google Analytics**: Web analytics
- **Custom**: Build your own

**Installation**:
- Install SDK
- Configure tracking
- Set up events
- Test tracking

> 💡 **Tip**: Start with Mixpanel or Amplitude. They're designed for product analytics.

### 2. Define Events to Track

**Essential Events**:
- User signup
- User login
- Core feature usage
- Journey completion
- Errors and issues

**User Journey Events**:
- Journey start
- Journey steps
- Journey completion
- Journey abandonment

**Feature Events**:
- Feature viewed
- Feature used
- Feature completed
- Feature errors

**Example Events**:
```javascript
// Track user signup
analytics.track('User Signed Up', {
  userId,
  method: 'email'
});

// Track feature usage
analytics.track('AI Insights Generated', {
  userId,
  retrospectiveId,
  duration
});

// Track journey completion
analytics.track('Journey Completed', {
  userId,
  journeyId,
  duration
});
```

### 3. Implement Event Tracking

**Frontend Tracking**:
- Track user actions
- Track page views
- Track feature usage
- Track errors

**Backend Tracking**:
- Track API calls
- Track processing times
- Track errors
- Track usage

**Example Implementation**:
```javascript
// Frontend tracking
function generateInsights(feedback) {
  analytics.track('Generate Insights Started', { userId });
  
  try {
    const insights = await api.generateInsights(feedback);
    analytics.track('Generate Insights Completed', {
      userId,
      duration: Date.now() - startTime
    });
    return insights;
  } catch (error) {
    analytics.track('Generate Insights Error', {
      userId,
      error: error.message
    });
    throw error;
  }
}
```

### 4. Set Up User Tracking

**User Identification**:
- Identify users consistently
- Track user properties
- Track user segments
- Track user journeys

**User Properties**:
- User ID
- User type
- User segment
- User cohort

**Example**:
```javascript
// Identify user
analytics.identify(userId, {
  email: user.email,
  type: 'beta_user',
  segment: 'engineering_team'
});
```

### 5. Create Analytics Dashboards

**Essential Dashboards**:
- **User Activity**: Active users, signups, usage
- **Feature Usage**: Feature views, usage, completion
- **Journey Analytics**: Journey completion, drop-off points
- **Error Tracking**: Errors, types, frequency

**Tools**:
- **Analytics Tool Dashboards**: Mixpanel, Amplitude
- **Custom Dashboards**: Grafana, Metabase
- **Simple Dashboards**: Excel, Google Sheets

## Apply It Now

**Task**: Set up instrumentation for your MVP

1. Choose and set up analytics tool
2. Define events to track (essential events)
3. Implement event tracking (frontend and backend)
4. Set up user tracking (identification and properties)
5. Create analytics dashboards
6. Test tracking and verify data collection

**Artifact**: An instrumentation setup with:
- Analytics tool configuration
- Event definitions
- Tracking implementation
- User tracking
- Analytics dashboards

## Artifacts

You'll create:
- Analytics tool configuration
- Event definitions
- Tracking implementation
- User tracking setup
- Analytics dashboards

## Worked Example

**Situation**: Setting up instrumentation for retrospective tool

**Analytics Tool**: Mixpanel

**Events Tracked**:
```
1. User Signed Up
   - userId, method

2. User Logged In
   - userId

3. Retrospective Created
   - userId, retrospectiveId

4. Feedback Added
   - userId, retrospectiveId, itemCount

5. AI Insights Generated
   - userId, retrospectiveId, duration

6. Insights Viewed
   - userId, retrospectiveId

7. Journey Completed
   - userId, retrospectiveId, duration

8. Error Occurred
   - userId, errorType, errorMessage
```

**User Tracking**:
```javascript
analytics.identify(userId, {
  email: user.email,
  type: 'beta_user',
  teamSize: user.teamSize,
  createdAt: user.createdAt
});
```

**Dashboards**:
- User Activity: Active users, signups, logins
- Feature Usage: Retrospectives created, insights generated
- Journey Analytics: Journey completion, drop-off points
- Error Tracking: Errors by type, frequency

## Checklist

Before proceeding to the next chapter, verify:
- [ ] Analytics tool is set up
- [ ] Events are defined
- [ ] Event tracking is implemented
- [ ] User tracking is set up
- [ ] Analytics dashboards are created
- [ ] Tracking is tested and working

## Self-Assessment

1. **What analytics tool is good for product analytics?**
   - [ ] Google Analytics
   - [ ] Mixpanel ✓
   - [ ] Excel

2. **What events should you track?** (Select all)
   - [ ] User signup ✓
   - [ ] Core feature usage ✓
   - [ ] Journey completion ✓
   - [ ] Every click

3. **What should dashboards include?** (Select all)
   - [ ] User activity ✓
   - [ ] Feature usage ✓
   - [ ] Journey analytics ✓
   - [ ] Every metric

## Exit Criteria

You're ready to proceed when:
- [ ] Analytics tool is set up
- [ ] Events are tracked
- [ ] User tracking is working
- [ ] Analytics dashboards are created
- [ ] You can understand user behavior

## Dependencies & Next Steps

### Prerequisites Completed
- [09 — Private Beta](09-private-beta.md) - Launched MVP

### Next Steps
- Proceed to [11 — Experiments](11-experiments.md) to start testing improvements
- OR proceed to [12 — Feedback Ops](12-feedback-ops.md) to establish feedback loops
- These can be done in parallel

### What This Enables

Instrumentation enables:
- Data-driven decisions
- User behavior understanding
- Feature usage insights
- Iteration planning

---

> 💡 **Tip**: Track what matters. Don't over-instrument. Focus on essential events.
> 📝 **Note**: Analytics are for learning, not just metrics. Use them to understand users.
