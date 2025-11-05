# 09 — Deploy

**Purpose**: Conduct thorough QA, set up Firebase infrastructure, and deploy MVP to production

**Outcome**: Have a deployed, tested, and monitored MVP ready for users

**Audience**: PM / Dev / Both

**Time**: 1-2 days

**Prerequisites**: [08 — Build Features](08-build-features.md) - Working MVP features ready for private beta

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Conduct thorough quality assurance testing before deployment
2. Set up Firebase project with Authentication, Hosting, and Functions
3. Configure environment variables and Firebase services
4. Set up Google Analytics and LogRocket for monitoring
5. Build and deploy MVP to production using Firebase

## Jobs-to-Be-Done

- **When**: I have working MVP features and need to deploy to production
- **I want**: To conduct QA, set up Firebase infrastructure, and deploy the MVP
- **So that**: Users can access a tested, monitored, and functional MVP

## Inputs

- Working MVP features from [08 — Build Features](08-build-features.md)
- Firebase account (create if needed)
- Understanding of Firebase services (Authentication, Hosting, Functions)
- Access to Google Analytics (via Firebase)
- LogRocket account (create if needed)

## Activities

### 1. Conduct Quality Assurance

**Before Deployment**: Conduct thorough quality assurance to identify and fix issues before deployment.

**Option 1: Manual Testing**

**Process**:
1. Test the entire application flow manually
2. Navigate through all user journeys
3. Test all features and functionality
4. Test error cases and edge states
5. Document all issues with as much detail as possible:
   - What component or feature has the issue
   - What the expected behavior is
   - What the actual behavior is
   - Steps to reproduce
   - Screenshots or videos if helpful
6. Provide the documented issues to Cursor Planning agent
7. Use Cursor's planning function in a new chat to create a fix plan
8. Review and approve the fix plan
9. Let Cursor implement the fixes
10. Test again after fixes are pushed

**Issue Documentation Example**:
```
Issues Found:
1. Login validation errors don't display properly
   - Expected: Error message appears below input field
   - Actual: No error message appears
   - Steps: Try to login with invalid email format
   - Screenshot: [attach screenshot]

2. Dashboard cards overlap on mobile devices
   - Expected: Cards stack vertically on mobile
   - Actual: Cards overlap each other
   - Steps: View dashboard on mobile device (375px width)
   - Screenshot: [attach screenshot]
```

> 💡 **Tip**: Be thorough with manual testing. Document everything - it helps Cursor fix issues more effectively.

**Option 2: Cursor Agent with Browser (Automated Testing)**

**Process**:
1. Use Cursor Agent with Browser to navigate through the app
2. Cursor will automatically test user flows and record inconsistencies
3. Cursor will identify issues and inconsistencies
4. Once testing completes, Cursor will automatically fix bugs
5. Review the fixes and test again manually
6. Ensure all issues are resolved

> 💡 **Tip**: Cursor Agent with Browser saves significant time and provides comprehensive automated testing. It's extremely helpful for catching issues you might miss.

**After Testing**:
- Ensure you test again after pushing fixes
- Verify all issues are resolved
- Test the complete user journey one more time
- Ensure the application is ready for deployment

> ⚠️ **Warning**: Don't skip QA. Thorough testing before deployment prevents issues that affect real users.

### 2. Set Up Firebase Project

**Create Firebase Account and Project**:
1. Go to [Firebase Console](https://console.firebase.google.com/)
2. Create a Firebase account (if you don't have one)
3. Create a new Firebase project
4. Follow the setup wizard
5. Note your project ID and configuration

**Configure Firebase Services**:
- **Authentication**: Will be enabled in next step
- **Hosting**: Will be configured in next step
- **Functions**: Will be configured if needed
- **Cloud Firestore**: Will be configured if needed

> 📝 **Note**: This playbook focuses on Firebase Authentication, Hosting, and Functions as a base. Configure these services as instructed by Cursor.

### 3. Set Up Environment Variables

**Configure Environment Variables**:
- Set up environment variables for your Firebase project
- Configure API keys and secrets
- Set up Firebase configuration
- Follow Cursor's instructions for environment variable setup

**Environment Variables to Configure**:
- Firebase API keys
- Firebase project configuration
- AI API keys (if applicable)
- Other service API keys
- Environment-specific settings

> 💡 **Tip**: Use `.env` files for local development and Firebase Functions environment configuration for production. Never commit secrets to version control.

### 4. Set Up Firebase Authentication

**Enable Authentication**:
1. Enable Firebase Authentication in Firebase Console
2. Configure authentication methods:
   - **Social Login**: Enable Google, GitHub, or other providers as desired
   - **Email/Password**: Enable email and password authentication if desired
3. Follow Cursor's instructions for setting up authentication
4. Configure authentication providers in your application
5. Test authentication flow

**Authentication Methods**:
- Social login (Google, GitHub, etc.)
- Email and password
- Custom authentication (if needed)

> 📝 **Note**: Enable authentication methods based on your PRD requirements. Social login is recommended for MVP simplicity.

### 5. Add Google Analytics Through Firebase

**Set Up Google Analytics**:
1. Enable Google Analytics in Firebase Console
2. Link Google Analytics to your Firebase project
3. Follow Cursor's instructions for integrating Google Analytics
4. Configure analytics tracking in your application
5. Set up essential events tracking:
   - User signup
   - Core feature usage
   - Journey completion
   - Errors
6. Verify analytics events are firing

**Analytics Events**:
- User signup/login
- Core feature usage
- User journey completion
- Error events
- Custom events as needed

> 💡 **Tip**: Start with essential events. You can add more tracking later based on what you learn.

### 6. Install and Set Up LogRocket

**Set Up LogRocket**:
1. Create a LogRocket account (if you don't have one)
2. Create a new project in LogRocket
3. Install LogRocket SDK in your application
4. Configure LogRocket for session tracking and bug reporting
5. Follow Cursor's instructions for LogRocket setup
6. Test LogRocket integration
7. Verify session replay is working

**LogRocket Features**:
- Session replay
- Bug reporting
- Error tracking
- Performance monitoring

> 📝 **Note**: LogRocket provides session tracking and bug reporting which is essential for understanding user behavior and debugging issues in production.

### 7. Build and Deploy

**Final Steps Before Launch**:
1. Ensure all QA issues are resolved
2. Verify Firebase services are configured
3. Verify environment variables are set
4. Verify authentication is working
5. Verify Google Analytics is tracking
6. Verify LogRocket is recording sessions

**Build Production Bundle**:
```bash
npm run build
```

**Deploy to Firebase**:
```bash
firebase deploy
```

**Verify Deployment**:
- Visit your deployed URL
- Test the complete user journey
- Verify all features work in production
- Check that analytics and LogRocket are working
- Verify authentication is working

> 🎉 **Congratulations!** Your MVP is now deployed and ready for users.

## Apply It Now

**Task**: Conduct QA, set up Firebase, and deploy MVP

1. Conduct thorough quality assurance (manual or Cursor Agent)
2. Document issues and get them fixed by Cursor
3. Test again after fixes
4. Create Firebase account and project
5. Set up environment variables
6. Configure Firebase Authentication (social login and/or email/password)
7. Add Google Analytics through Firebase
8. Install and set up LogRocket
9. Build production bundle (`npm run build`)
10. Deploy to Firebase (`firebase deploy`)
11. Verify deployment and test in production

**Artifact**: A deployed MVP with:
- QA issues resolved
- Firebase infrastructure set up
- Authentication configured
- Google Analytics tracking
- LogRocket session tracking
- Production deployment live

## Artifacts

You'll create:
- QA issue documentation and fixes
- Firebase project configuration
- Environment variables setup
- Firebase Authentication configuration
- Google Analytics integration
- LogRocket integration
- Production deployment

## Worked Example

**Situation**: Deploying retrospective tool MVP

**QA Process**:
1. **Manual Testing**: Tested entire application flow
   - Found 5 issues: login validation, mobile layout, AI loading state, export button, error handling
   - Documented all issues with details and screenshots
   - Provided to Cursor Planning agent
   - Cursor created fix plan with 8 tasks
   - Approved fix plan
   - Cursor implemented fixes
   - Tested again - all issues resolved

2. **Firebase Setup**: Created Firebase project
   - Project name: "retro-tool-mvp"
   - Project ID: "retro-tool-mvp"
   - Configured Authentication, Hosting, Functions

3. **Environment Variables**: Set up configuration
   - Firebase API keys
   - Anthropic API key
   - Environment-specific settings

4. **Authentication**: Enabled Firebase Auth
   - Enabled Google social login
   - Enabled email/password authentication
   - Configured in application
   - Tested authentication flow

5. **Google Analytics**: Added through Firebase
   - Enabled Google Analytics in Firebase Console
   - Configured essential events: signup, journey completion, errors
   - Verified events are firing

6. **LogRocket**: Installed and configured
   - Created LogRocket project
   - Installed SDK
   - Configured session tracking
   - Verified session replay working

7. **Deployment**: Built and deployed
   - Ran `npm run build` - success
   - Ran `firebase deploy` - success
   - Deployed URL: `https://retro-tool-mvp.web.app`
   - Tested in production - all features working

**Time**: QA and deployment took 1.5 days

## Checklist

Before proceeding to the next chapter, verify:
- [ ] QA testing completed (manual or Cursor Agent)
- [ ] All issues documented and fixed
- [ ] Tested again after fixes
- [ ] Firebase project created and configured
- [ ] Environment variables set up
- [ ] Firebase Authentication enabled and configured
- [ ] Google Analytics added and tracking
- [ ] LogRocket installed and configured
- [ ] Production build successful (`npm run build`)
- [ ] Deployment successful (`firebase deploy`)
- [ ] Production deployment tested and verified
- [ ] All features working in production

## Self-Assessment

1. **What should you do before deploying?**
   - [ ] Deploy immediately
   - [ ] Conduct thorough QA ✓
   - [ ] Skip testing
   - [ ] Test only after deployment

2. **What Firebase services should be set up?** (Select all)
   - [ ] Authentication ✓
   - [ ] Hosting ✓
   - [ ] Functions ✓
   - [ ] All Firebase services

3. **What monitoring tools should be set up?** (Select all)
   - [ ] Google Analytics ✓
   - [ ] LogRocket ✓
   - [ ] Complex monitoring systems
   - [ ] No monitoring needed

## Exit Criteria

You're ready to proceed when:
- [ ] QA testing is complete and all issues are fixed
- [ ] Firebase project is set up and configured
- [ ] Environment variables are configured
- [ ] Firebase Authentication is enabled and working
- [ ] Google Analytics is tracking events
- [ ] LogRocket is recording sessions
- [ ] MVP is built and deployed to production
- [ ] Production deployment is tested and verified
- [ ] MVP is ready for users

## Dependencies & Next Steps

### Prerequisites Completed
- [08 — Build Features](08-build-features.md) - Working MVP features ready for private beta

### Next Steps
- Proceed to [Launch & Iterate](launch/index.md) to launch MVP and gather feedback

### What This Enables

Deployment enables:
- Users can access the MVP
- Real user feedback opportunities
- Learning from actual usage
- Iteration and improvement based on data
- Monitoring and debugging capabilities

---

> 💡 **Tip**: Don't skip QA. Thorough testing before deployment prevents issues that affect real users.
> 📝 **Note**: This playbook focuses on Firebase (Authentication, Hosting, Functions) as the base. Follow Cursor's instructions for setup.
> ⚠️ **Warning**: Test thoroughly before deployment. Production issues affect real users. Ensure all QA issues are resolved.
> 🎉 **Launch**: The final step is `npm run build` followed by `firebase deploy`. Your MVP is now live!
