# 09 — Deploy

**Purpose**: Deploy MVP to production and set up quality & observability

**Outcome**: Have a deployed, monitored, functional MVP ready for users

**Audience**: PM / Dev / Both

**Time**: 1-2 days

**Prerequisites**: [07 — AI Baseline](07-ai-baseline.md) OR [08 — Build Features](08-build-features.md)

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Deploy MVP to production
2. Set up error tracking and monitoring
3. Implement logging and analytics
4. Monitor application health
5. Validate deployed MVP

## Jobs-to-Be-Done

- **When**: I have working MVP features and need to deploy to production
- **I want**: To deploy MVP with quality monitoring and observability
- **So that**: Users can access the MVP and I can monitor its performance

## Inputs

- Working MVP features from [07 — AI Baseline](07-ai-baseline.md) or [08 — Build Features](08-build-features.md)
- Understanding of deployment platform
- Access to monitoring tools
- Production environment ready

## Activities

### 1. Deploy to Production

**Choose Deployment Platform**:
- **Firebase Hosting**: Static site hosting with SPA routing (recommended for this stack)
- **Vercel**: Static site hosting with serverless functions
- **Netlify**: Static site hosting with build pipelines
- **Other**: AWS, GCP, Azure (if needed)

**Deployment Process**:
1. Build production bundle
2. Configure deployment settings
3. Set up environment variables
4. Deploy to production
5. Verify deployment success
6. Test deployed application

**Firebase Hosting Example**:
```bash
# Build production bundle
npm run build

# Deploy to Firebase
firebase deploy --only hosting

# Verify deployment
# Visit deployed URL and test
```

> 💡 **Tip**: Test deployment in staging first if available. Verify all features work in production.

### 2. Set Up Error Tracking

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

**Example (Sentry)**:
```javascript
import * as Sentry from "@sentry/react";

Sentry.init({
  dsn: "your-sentry-dsn",
  environment: "production",
});
```

> 💡 **Tip**: Start with Sentry. It's free for small projects and easy to set up.

### 3. Implement Logging

**Set Up Logging**:
- **Backend**: Structured logging
- **Frontend**: Error logging
- **Format**: JSON or structured format
- **Levels**: Error, Warning, Info

**Tools**:
- **Winston** (Node.js)
- **Python logging** (Python)
- **Console logging** (Simple)
- **LogRocket** (Frontend)

**Example**:
```javascript
// Simple logging example
logger.error('AI API call failed', { error, userId });
logger.info('User completed journey', { userId, journey });
```

### 4. Add Analytics Tracking

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

### 5. Monitor Application Health

**Set Up Health Checks**:
- **API health**: Check API status
- **Database health**: Check database connection
- **External services**: Check AI API, etc.

**Monitoring**:
- **Uptime monitoring**: UptimeRobot, Pingdom
- **Application monitoring**: Simple health endpoints
- **Alerts**: Email or Slack notifications

### 6. Set Up Basic Dashboards

**Create Dashboards**:
- **Error dashboard**: Error rates, types
- **Usage dashboard**: User activity, feature usage
- **Performance dashboard**: Response times, API calls

**Tools**:
- **Grafana**: Dashboards
- **Simple dashboards**: Custom or tool-provided
- **Email reports**: Weekly summaries

### 7. Validate Deployed MVP

**Validation Checklist**:
- [ ] All features work in production
- [ ] Error tracking is working
- [ ] Logging is capturing events
- [ ] Analytics is tracking events
- [ ] Health monitoring is active
- [ ] Alerts are configured
- [ ] Performance is acceptable

**Testing**:
- Test complete user journey in production
- Verify error tracking captures errors
- Check analytics events are firing
- Test health monitoring
- Verify alerts work

## Apply It Now

**Task**: Deploy MVP and set up quality & observability

1. Deploy MVP to production
2. Set up error tracking (e.g., Sentry)
3. Implement logging (backend and frontend)
4. Add analytics tracking (essential events)
5. Set up health monitoring
6. Create basic dashboards
7. Validate deployed MVP

**Artifact**: A deployed MVP with:
- Production deployment
- Error tracking
- Logging
- Analytics
- Health monitoring
- Dashboards

## Artifacts

You'll create:
- Production deployment
- Error tracking configuration
- Logging setup
- Analytics tracking
- Health monitoring
- Dashboards

## Worked Example

**Situation**: Deploying retrospective tool MVP

**Deployment**:
- Platform: Firebase Hosting
- Build: `npm run build`
- Deploy: `firebase deploy --only hosting`
- URL: `https://retro-tool.web.app`
- Status: Successfully deployed

**Error Tracking**:
- Tool: Sentry
- Setup: Installed SDK, configured error tracking
- Alerts: Email notifications for errors
- Status: Working, capturing errors

**Logging**:
- Backend: Winston for structured logging
- Frontend: Error logging to Sentry
- Format: JSON structured logs
- Status: Logging successfully

**Analytics**:
- Tool: Mixpanel
- Events tracked:
  - User signup
  - Retrospective created
  - Insights generated
  - Journey completed
- Status: Tracking events successfully

**Health Monitoring**:
- Health endpoint: `/health`
- Checks: API, database, AI API
- Monitoring: UptimeRobot
- Alerts: Email for downtime
- Status: Monitoring active

**Dashboards**:
- Error dashboard: Error rates, types
- Usage dashboard: User activity, feature usage
- Performance dashboard: Response times
- Status: Dashboards created

**Validation**:
- All features working in production
- Error tracking capturing errors
- Analytics tracking events
- Health monitoring active
- MVP ready for users

**Time**: Deployment and setup took 1 day

## Checklist

Before proceeding to the next chapter, verify:
- [ ] MVP deployed to production
- [ ] Error tracking is set up
- [ ] Logging is implemented
- [ ] Analytics tracking is added
- [ ] Health monitoring is in place
- [ ] Dashboards are created
- [ ] Alerts are configured
- [ ] Deployed MVP is validated

## Self-Assessment

1. **What should be set up before deploying?** (Select all)
   - [ ] Error tracking ✓
   - [ ] Analytics tracking ✓
   - [ ] Health monitoring ✓
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
- [ ] MVP is deployed to production
- [ ] Error tracking is set up and working
- [ ] Logging is implemented
- [ ] Analytics tracking is added
- [ ] Health monitoring is in place
- [ ] You can debug issues and understand usage
- [ ] MVP is accessible to users

## Dependencies & Next Steps

### Prerequisites Completed
- [07 — AI Baseline](07-ai-baseline.md) OR [08 — Build Features](08-build-features.md) - Working MVP features

### Next Steps
- Proceed to [Launch & Iterate](launch/index.md) to launch MVP and gather feedback

### What This Enables

Deployment with quality & observability enables:
- Users can access the MVP
- Error debugging and monitoring
- Usage understanding
- Performance monitoring
- Data-driven decisions

---

> 💡 **Tip**: Start simple. You can enhance monitoring later.
> 📝 **Note**: Don't skip quality essentials. They're critical for MVP.
> ⚠️ **Warning**: Test deployment thoroughly. Production issues affect real users.

