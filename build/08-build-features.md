# 08 — Build Features

**Purpose**: Implement UI components and features based on the designed mockups from Planning

**Outcome**: Have working frontend features that match the designed user journey

**Audience**: PM / Dev / Both

**Time**: 1-2 weeks

**Prerequisites**: [06 — Setup](06-setup) - Implementation plan approved

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Implement UI components based on mockups from Planning
2. Build frontend features following the designed journey
3. Connect frontend to backend and AI baseline
4. Create a functional interface matching the mockups
5. Test the implemented user journey

## Jobs-to-Be-Done

- **When**: I have implementation plan and need to build the UI features
- **I want**: To implement UI components based on the designed mockups
- **So that**: Users can complete the designed journey end-to-end

## Inputs

- Implementation plan from [06 — Setup](06-setup)
- Mockups from [05 — Planning](05-planning) (designed journey)
- PRD from [05 — Planning](05-planning)
- AI baseline from [07 — AI Baseline](07-ai-baseline) (if applicable)
- Development environment configured

## Activities

### 1. Review Mockups and Implementation Plan

**Review Design**:
- Review mockups from Planning phase
- Understand the designed user journey
- Identify components needed
- Review implementation plan tasks

**Journey Reference**:
- The complete user journey was designed in Planning using UX Pilot
- Mockups show the flow: Signup → Core Value → Success
- Your task is to implement these designed screens

> 💡 **Tip**: Keep mockups open as reference while building. Match the design as closely as possible.

### 2. Implement UI Components

**Build Components Based on Mockups**:
- Start with authentication screens (signup/login)
- Build core value screens (main user journey)
- Create success/completion screens
- Implement navigation and layout components

**Component Structure**:
- Create reusable components
- Follow component organization from `.cursorrules`
- Use design system components (Radix UI, Tailwind)
- Match mockup designs

**Implementation Process**:
1. Review mockup for a screen
2. Create component structure
3. Implement UI matching mockup
4. Connect to state management
5. Test component functionality

### 3. Build Core UX Flows

**Implement Essential Flows**:
- **Onboarding**: Signup/login flow
- **Core Value**: Main user journey flow
- **Success**: Completion and value delivery flow

**Flow Implementation**:
- Build flows step by step following the mockups
- Connect screens with routing
- Implement state management between screens
- Ensure flows work end-to-end
- Test each flow

> 📝 **Note**: Focus on functionality over polish. Match the mockup design but prioritize working features.

### 4. Integrate with Backend

**Connect Frontend to Backend**:
- API integration for data fetching
- Connect to Firebase services (Auth, Firestore)
- Integrate with AI baseline (if applicable)
- Implement state management (Zustand)
- Handle loading and error states

**Integration Points**:
- Authentication: Firebase Auth
- Data: Cloud Firestore
- AI Features: API calls to AI baseline
- State: Zustand stores

### 5. Test User Journey

**Testing**:
- Test complete user journey end-to-end
- Verify flows match the designed mockups
- Test error cases and edge states
- Verify backend integration works
- Test with real data

**User Testing**:
- Test with real users (if possible)
- Observe completion rate
- Gather feedback on implementation
- Identify issues and improvements

## Apply It Now

**Task**: Build features based on designed mockups

1. Review mockups and implementation plan
2. Implement UI components matching mockups
3. Build core UX flows (onboarding, core value, success)
4. Integrate with backend and AI baseline
5. Test complete user journey
6. Get user feedback and iterate

**Artifact**: Working frontend features with:
- UI components matching mockups
- Complete user journey implemented
- Backend integration
- User testing results

## Artifacts

You'll create:
- UI components matching mockups
- Implemented user journey
- Backend integration
- Frontend state management
- User testing documentation

## Worked Example

**Situation**: Implementing features for retrospective tool MVP

**Implementation Process**:
1. **Review Mockups**: Reviewed 10 mockup PNGs from Planning
   - Authentication flow (3 screens)
   - Primary journey: Create → Add → View → Export (5 screens)
   - Dashboard (2 screens)

2. **Implement Components**: Built React components
   - Authentication: LoginForm, SignupForm
   - Core: CreateRetroForm, FeedbackList, InsightsView
   - Navigation: Dashboard, ProjectTabs
   - Matched mockup designs using Tailwind CSS

3. **Build Flows**: Implemented complete flows
   - Signup → Login → Dashboard
   - Create Retrospective → Add Feedback → View Insights → Export
   - Connected with React Router

4. **Integrate Backend**: Connected to Firebase
   - Firebase Auth for authentication
   - Firestore for data storage
   - AI baseline API for insights generation

5. **Test**: Tested complete journey
   - 8 out of 10 users completed journey
   - Average time: 5 minutes
   - Feedback: "Matches design", "Easy to use"
   - Issues: Export button needs improvement

**Time**: Implementation took 10 days

## Checklist

Before proceeding to the next chapter, verify:
- [ ] UI components implemented based on mockups
- [ ] Core UX flows are working end-to-end
- [ ] Backend integration is complete
- [ ] User journey matches designed mockups
- [ ] User journey is tested
- [ ] User feedback is collected

## Self-Assessment

1. **Where was the user journey designed?**
   - [ ] During implementation
   - [ ] In the Setup chapter
   - [ ] In UX Pilot during Planning ✓
   - [ ] After deployment

2. **What should you focus on when implementing?** (Select all)
   - [ ] Match mockup designs ✓
   - [ ] Build working features ✓
   - [ ] Perfect design
   - [ ] All features

3. **What should you test?** (Select all)
   - [ ] Complete user journey ✓
   - [ ] Error cases ✓
   - [ ] Backend integration ✓
   - [ ] Perfect design

## Exit Criteria

You're ready to proceed when:
- [ ] UI components match mockups
- [ ] Core UX flows are working
- [ ] Backend integration is complete
- [ ] User journey is tested with real users
- [ ] Features are ready for deployment

## Dependencies & Next Steps

### Prerequisites Completed
- [05 — Planning](05-planning) - Mockups and designed journey
- [06 — Setup](06-setup) - Implementation plan
- [07 — AI Baseline](07-ai-baseline) - AI features (if applicable)

### Next Steps
- Proceed to [09 — Deploy](09-deploy) to deploy MVP with quality & observability

### What This Enables

Implemented features enable:
- Complete user value demonstration
- Real user testing
- Learning about user behavior
- Iteration and improvement

---

> 💡 **Tip**: Keep mockups open as reference. Focus on matching the design while building working features.
> 📝 **Note**: The journey design happened in Planning. Your job here is to implement it accurately.
> ⚠️ **Warning**: Don't redesign during implementation. Stick to the mockups from Planning unless you discover critical issues.

