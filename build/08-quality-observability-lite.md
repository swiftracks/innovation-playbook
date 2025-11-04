# 08 — Quality & Observability (Lite)

> **Purpose**: Implement essential quality and observability features
> **Outcome**: Have error tracking, logging, and basic analytics in place
> **Audience**: PM / Dev / Both
> **Time**: 1-2 days
> **Prerequisites**: [06 — AI Baseline](06-ai-baseline.md) OR [07 — UX Thin Vertical](07-ux-thin-vertical.md)

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Set up error tracking and monitoring
2. Implement basic logging
3. Add analytics tracking
4. Monitor application health
5. Debug issues effectively

## Jobs-to-Be-Done

- **When**: I have working MVP features and need to monitor quality
- **I want**: To track errors, monitor performance, and understand usage
- **So that**: I can debug issues and learn from user behavior

## Inputs

- Working MVP features from [06 — AI Baseline](06-ai-baseline.md) or [07 — UX Thin Vertical](07-ux-thin-vertical.md)
- Understanding of what to monitor
- Access to monitoring tools

## Activities

### 1. Set Up Error Tracking

**Choose Error Tracking Tool**:
- **Sentry**: Comprehensive error tracking
- **Rollbar**: Error tracking and monitoring
- **LogRocket**: Session replay and errors
- **Simple logging**: Basic error logging

**Implementation**:
- Install SDK
- Configure error tracking
- Set up alerts
- Test error reporting

> 💡 **Tip**: Start with Sentry. It's free for small projects and easy to set up.

### 2. Implement Logging

**Set Up Logging**:
- **Backend**: Structured logging
- **Frontend**: Error logging
- **Format**: JSON or structured format
- **Levels**: Error, Warning, Info

**Tools**:
- **Winston** (Node.js)
- **Python logging** (Python)
- **Console logging** (Simple)

**Example**:
```javascript
// Simple logging example
logger.error('AI API call failed', { error, userId });
logger.info('User completed journey', { userId, journey });
```

### 3. Add Analytics Tracking

**Choose Analytics Tool**:
- **Google Analytics**: Web analytics
- **Mixpanel**: Product analytics
- **Amplitude**: Product analytics
- **Simple custom**: Basic tracking

**Track Essential Events**:
- User signup
- Core feature usage
- Journey completion
- Errors

**Example**:
```javascript
// Track user event
analytics.track('User Completed Journey', {
  userId,
  journeyId,
  duration
});
```

### 4. Monitor Application Health

**Set Up Health Checks**:
- **API health**: Check API status
- **Database health**: Check database connection
- **External services**: Check AI API, etc.

**Monitoring**:
- **Uptime monitoring**: UptimeRobot, Pingdom
- **Application monitoring**: Simple health endpoints
- **Alerts**: Email or Slack notifications

### 5. Set Up Basic Dashboards

**Create Dashboards**:
- **Error dashboard**: Error rates, types
- **Usage dashboard**: User activity, feature usage
- **Performance dashboard**: Response times, API calls

**Tools**:
- **Grafana**: Dashboards
- **Simple dashboards**: Custom or tool-provided
- **Email reports**: Weekly summaries

## Apply It Now

**Task**: Set up quality and observability for your MVP

1. Set up error tracking (e.g., Sentry)
2. Implement logging (backend and frontend)
3. Add analytics tracking (essential events)
4. Set up health monitoring
5. Create basic dashboards
6. Test monitoring and alerts

**Artifact**: A quality and observability setup with:
- Error tracking
- Logging
- Analytics
- Health monitoring
- Dashboards

## Artifacts

You'll create:
- Error tracking configuration
- Logging setup
- Analytics tracking
- Health monitoring
- Dashboards

## Worked Example

**Situation**: Setting up quality and observability for retrospective tool

**Error Tracking**:
- Tool: Sentry
- Setup: Installed SDK, configured error tracking
- Alerts: Email notifications for errors

**Logging**:
- Backend: Winston for structured logging
- Frontend: Error logging to Sentry
- Format: JSON structured logs

**Analytics**:
- Tool: Mixpanel
- Events tracked:
  - User signup
  - Retrospective created
  - Insights generated
  - Journey completed

**Health Monitoring**:
- Health endpoint: `/health`
- Checks: API, database, AI API
- Monitoring: UptimeRobot
- Alerts: Email for downtime

**Dashboards**:
- Error dashboard: Error rates, types
- Usage dashboard: User activity, feature usage
- Performance dashboard: Response times

## Checklist

Before proceeding to the next chapter, verify:
- [ ] Error tracking is set up
- [ ] Logging is implemented
- [ ] Analytics tracking is added
- [ ] Health monitoring is in place
- [ ] Dashboards are created
- [ ] Alerts are configured

## Self-Assessment

1. **What should you set up for MVP?** (Select all)
   - [ ] Error tracking ✓
   - [ ] Basic logging ✓
   - [ ] Analytics ✓
   - [ ] Complex monitoring systems

2. **What analytics events should you track?** (Select all)
   - [ ] User signup ✓
   - [ ] Core feature usage ✓
   - [ ] Journey completion ✓
   - [ ] Every click

3. **What should you monitor?** (Select all)
   - [ ] Errors ✓
   - [ ] Usage ✓
   - [ ] Performance ✓
   - [ ] Every detail

## Exit Criteria

You're ready to proceed when:
- [ ] Error tracking is set up and working
- [ ] Logging is implemented
- [ ] Analytics tracking is added
- [ ] Health monitoring is in place
- [ ] You can debug issues and understand usage

## Dependencies & Next Steps

### Prerequisites Completed
- [06 — AI Baseline](06-ai-baseline.md) OR [07 — UX Thin Vertical](07-ux-thin-vertical.md) - Working MVP features

### Next Steps
- Proceed to [Launch & Iterate](launch/index.md) to launch MVP and gather feedback

### What This Enables

Quality and observability enable:
- Error debugging
- Usage understanding
- Performance monitoring
- Data-driven decisions

---

> 💡 **Tip**: Start simple. You can enhance monitoring later.
> 📝 **Note**: Don't skip quality essentials. They're critical for MVP.
