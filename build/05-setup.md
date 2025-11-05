# 05 — Setup

**Purpose**: Plan and set up development environment for rapid MVP development

**Outcome**: Have a complete plan (user stories, PRD, mockups) and a working development environment ready for building

**Audience**: PM / Dev / Both

**Time**: Planning: 1-2 days | Setup: 4-8 hours

**Prerequisites**: [Decide What to Build](decide/index.md) - Decision to build, key problems identified, innovation aspects defined

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Generate and refine user stories using AI tools
2. Create a comprehensive PRD using AI tools
3. Design and prototype user flows using UX Pilot
4. Set up development environment with version control and Cursor configuration
5. Use Cursor's plan mode to generate implementation plans

## Jobs-to-Be-Done

- **When**: I have a decision to build and need to plan and set up development
- **I want**: To create a detailed plan and set up development environment
- **So that**: I can build efficiently with clear direction and proper tooling

## Inputs

- Decision to build from [06 — Synthesize Insights → Decision](decide/06-synthesize-insights-decision.md)
- Key problems identified and innovation aspects defined
- Understanding of target users and value proposition
- Access to AI tools (ChatGPT, Claude, or Cursor)
- Access to UX Pilot for mockup generation
- GitLab or GitHub account for version control

## Activities

This chapter is organized into two phases: **Planning** and **Setup & Execution**.

### Phase 1: Planning

Before setting up your development environment, create a comprehensive plan that will guide your implementation.

#### 1. Generate User Stories

Use AI tools (ChatGPT, Claude, or Cursor) to generate an initial set of user stories based on your key problems and innovation aspects.

**Process**:
1. Provide context about your product idea, target users, and key problems
2. Request generation of user stories in the format: "As a [user type], I want [action] so that [benefit]"
3. Review and iterate on the generated stories
4. Refine stories to ensure they align with your MVP scope
5. Finalize a prioritized list of user stories

**Example Prompt**:
```
I'm building a B2B AI SaaS product that helps [target users] solve [problem]. 
Key innovation aspects: [aspect 1], [aspect 2], [aspect 3].
Generate 10-15 user stories for the MVP, prioritizing core functionality.
```

> 💡 **Tip**: Iterate on user stories with AI. Ask for refinements, merge similar stories, and ensure they're specific and measurable.

#### 2. Generate Product Requirements Document (PRD)

Use AI tools to generate a comprehensive PRD based on your finalized user stories.

**Process**:
1. Provide your finalized user stories and product context
2. Request generation of a PRD using the structure in [PRD Template](05-setup-prd-template.md)
3. Review and refine the PRD with AI
4. Ensure all sections are complete and clear
5. Finalize the PRD document

**PRD Structure** (see [template](05-setup-prd-template.md)):
- Purpose & Vision
- Scope (Release 1)
- Key Personas
- User Journeys
- Functional Requirements
- Non-Functional Requirements
- Information Architecture & Data Model
- UX References
- Acceptance Criteria
- Analytics & Success Metrics
- Content & States
- Accessibility & Design System
- Security, Privacy, Compliance
- Glossary

**Example Prompt**:
```
Based on these user stories: [list user stories],
Generate a comprehensive PRD for MVP Release 1 following this structure:
[reference PRD template structure]
Include specific acceptance criteria for each feature.
```

> 📝 **Note**: The PRD serves as the blueprint for your MVP. Spend time getting it right - it will guide all implementation decisions.

#### 3. Design User Flows and Screens

Use UX Pilot to create visual mockups of your application.

**Process**:
1. Review your PRD and identify key user flows
2. In UX Pilot, create flows for each major user journey
3. Generate screens for each step in the flows
4. Iterate on mockups based on UX best practices
5. Ensure all screens referenced in PRD are created
6. Export all mockups to PNG format when satisfied

**Key Flows to Design**:
- Authentication flow
- Primary user journey (core value delivery)
- Secondary user journeys
- Error and edge case states

> 🎯 **Goal**: Create mockups that clearly communicate your vision. These will be used by Cursor to understand the UI structure.

### Phase 2: Setup & Execution

Once planning is complete, set up your development environment and begin implementation planning.

#### 4. Create Git Repository

Create a new GitLab or GitHub project for your MVP.

**Steps**:
1. Create a new repository in GitLab or GitHub
2. Initialize with a README (optional)
3. Note the repository URL

> 💡 **Tip**: Choose a repository name that reflects your MVP. Keep it simple and descriptive.

#### 5. Clone Repository in Cursor

Open Cursor and clone your Git repository.

**Steps**:
1. Open Cursor IDE
2. Use File → Open Folder or Clone Repository
3. Enter your Git repository URL
4. Clone the repository to your local machine
5. Open the cloned folder in Cursor

#### 6. Set Up .cursorrules

Create a `.cursorrules` file in your project root with strong rules for rapid MVP development.

**Process**:
1. Create a `.cursorrules` file in the project root
2. Use the [.cursorrules template](05-setup-cursorrules-template.md) as a starting point
3. Customize rules based on your specific needs
4. Include rules for:
   - Code quality standards
   - TypeScript best practices
   - React patterns
   - Component organization
   - Error handling
   - Testing considerations
   - MVP-specific guidelines

> ⚠️ **Warning**: Strong `.cursorrules` help Cursor generate better code. Don't skip this step - it significantly improves code quality and consistency.

#### 7. Use Cursor Plan Mode

Use Cursor's plan mode to generate an implementation plan based on your PRD and mockups.

**Process**:
1. In Cursor, select "Plan Mode" (or equivalent planning feature)
2. Provide your PRD document
3. Upload all mockup PNG files
4. Specify your foundation tech stack (see Tech Stack section below)
5. Request an implementation plan that breaks down the work into manageable tasks

**Example Request**:
```
I'm building an MVP using this PRD: [PRD content]
Mockups: [upload all PNG files]
Tech Stack: [list tech stack]
Generate a comprehensive implementation plan that breaks down the work into 
logical phases and tasks. Prioritize core MVP features first.
```

**Tech Stack to Specify**:
- Core Framework: React 19, TypeScript 5.9.3, Vite 7.7
- Routing & State: React Router DOM 7.4, Zustand 5.8
- UI & Styling: Tailwind CSS 3.3.6, Radix UI (Dialog, Dropdown Menu, Select, Label, Slot, Tabs, Toast), Lucide React 0.546, Heroicons React 2.0
- Utilities: class-variance-authority, clsx
- Backend: Firebase 12.4.0 (Authentication, Cloud Firestore, Firebase Hosting)
- AI Integration: Anthropic SDK 0.67.0 (Claude API)
- Monitoring: LogRocket 10.1.0
- Development Tools: PostCSS, Autoprefixer, ESBuild

> 📝 **Note**: Review Cursor's plan carefully. Ensure it aligns with your PRD and covers all MVP features. Adjust the plan if needed before proceeding.

#### 8. Review and Approve Implementation Plan

Review Cursor's generated implementation plan.

**Review Checklist**:
- [ ] Plan covers all PRD features
- [ ] Tasks are logically sequenced
- [ ] Plan follows MVP scope (not over-engineering)
- [ ] Dependencies are identified
- [ ] Plan aligns with mockups

**If Plan Needs Adjustment**:
- Provide feedback to Cursor about what to change
- Request revisions to the plan
- Iterate until satisfied

#### 9. Begin Building

Once the plan is approved, begin implementation.

**Workflow**:
1. Start with the first task in the plan
2. Use Cursor to implement features following the plan
3. Test features as you build
4. Use Cursor's browser mode for debugging when needed
5. Continue implementing features in sequence

**Using Cursor for Development**:
- Follow the implementation plan
- Use `.cursorrules` to guide code generation
- Request fixes when encountering bugs
- Ask for enhancements when needed
- Use browser mode for debugging UI issues

**Using Cursor Browser Mode**:
- Navigate to your app in development
- Use browser mode to inspect elements
- Debug styling and layout issues
- Test interactions and flows
- Fix issues directly from browser context

> 💡 **Tip**: Test frequently as you build. Don't wait until the end to test - catch issues early.

## Foundation Tech Stack

This tech stack is optimized for rapid MVP development as of November 2024:

### Core Framework & Language

- **React 19** - UI framework with latest features
- **TypeScript 5.9.3** - Type safety (strict mode)
- **Vite 7.7** - Fast build tool and dev server

### Routing & State Management

- **React Router DOM 7.4** - Client-side routing
- **Zustand 5.8** - Lightweight state management

### UI & Styling

- **Tailwind CSS 3.3.6** - Utility-first CSS framework
- **Radix UI** - Headless, accessible components:
  - Dialog
  - Dropdown Menu
  - Select
  - Label
  - Slot
  - Tabs
  - Toast
- **Lucide React 0.546** - Icon library
- **Heroicons React 2.0** - Icon library
- **class-variance-authority** & **clsx** - ClassName utilities

### Backend & Database

- **Firebase 12.4.0**:
  - Authentication
  - Cloud Firestore (database)
  - Firebase Hosting (deployment)

### AI Integration

- **Anthropic SDK 0.67.0** - Claude API integration

### Monitoring & Observability

- **LogRocket 10.1.0** - Production monitoring and session replay

### Development Tools

- **PostCSS** & **Autoprefixer** - CSS processing
- **ESBuild** - Bundling and minification

### Deployment

- **Firebase Hosting** - Static site hosting with SPA routing support

> 📝 **Note**: This is a modern React/TypeScript stack using Firebase for backend services and Vite for development and building. The stack is optimized for rapid MVP development while maintaining code quality.

## Apply It Now

**Task**: Complete planning and setup for your MVP

### Planning Phase:
1. Generate user stories using AI tools (ChatGPT, Claude, or Cursor)
2. Iterate and finalize user stories
3. Generate comprehensive PRD using AI tools
4. Review and refine PRD
5. Create user flows and screens in UX Pilot
6. Iterate on mockups
7. Export all mockups to PNG

### Setup & Execution Phase:
1. Create GitLab or GitHub repository
2. Clone repository in Cursor
3. Set up `.cursorrules` file with development rules
4. Use Cursor plan mode with PRD, mockups, and tech stack
5. Review and approve implementation plan
6. Begin building following the plan

**Artifacts**: You'll create:
- Finalized user stories list
- Comprehensive PRD document
- UX Pilot mockups (PNG files)
- Git repository with `.cursorrules`
- Cursor implementation plan
- Initial project structure

## Artifacts

You'll create:
- User stories list (prioritized)
- Product Requirements Document (PRD)
- UX mockups (PNG files for all screens)
- Git repository configuration
- `.cursorrules` file
- Cursor implementation plan
- Initial project structure

## Worked Example

**Situation**: Planning and setting up for a B2B AI SaaS MVP

**Planning Phase**:
1. **User Stories**: Used Claude to generate 12 user stories from problem statement
   - Iterated 3 times to refine and prioritize
   - Finalized 8 core MVP stories
2. **PRD**: Generated comprehensive PRD using Claude with PRD template structure
   - Included all sections: purpose, scope, personas, journeys, requirements
   - Defined acceptance criteria for each feature
   - Reviewed and refined with AI assistance
3. **Mockups**: Created flows in UX Pilot
   - Authentication flow (3 screens)
   - Primary user journey (5 screens)
   - Dashboard (2 screens)
   - Exported 10 PNG mockup files

**Setup & Execution Phase**:
1. **Git Repository**: Created GitHub repository `mvp-product-name`
2. **Cursor Setup**: Cloned repository in Cursor
3. **.cursorrules**: Created `.cursorrules` with rules for:
   - TypeScript strict mode
   - React best practices
   - Component organization
   - Error handling standards
   - MVP-specific guidelines
4. **Cursor Plan Mode**: Provided PRD, 10 mockup PNGs, and tech stack
   - Cursor generated 15-task implementation plan
   - Reviewed and approved plan (1 adjustment requested)
5. **Implementation**: Began building following the plan
   - Completed authentication setup (Task 1-2)
   - Started core feature implementation (Task 3-5)

**Time**: Planning took 1.5 days, Setup took 6 hours, Initial implementation in progress

## Checklist

Before proceeding to the next chapter, verify:

**Planning Phase**:
- [ ] User stories generated and finalized
- [ ] PRD created and reviewed
- [ ] UX mockups created in UX Pilot
- [ ] All mockups exported to PNG

**Setup & Execution Phase**:
- [ ] Git repository created
- [ ] Repository cloned in Cursor
- [ ] `.cursorrules` file created and customized
- [ ] Cursor plan mode used with PRD and mockups
- [ ] Implementation plan reviewed and approved
- [ ] Initial project structure created

## Self-Assessment

1. **What should you do first in the planning phase?**
   - [ ] Create mockups
   - [ ] Generate user stories ✓
   - [ ] Set up Git repository
   - [ ] Write code

2. **What should be included in your PRD?** (Select all)
   - [ ] Purpose & Vision ✓
   - [ ] Functional Requirements ✓
   - [ ] User Journeys ✓
   - [ ] Complete product design for all future releases

3. **When should you set up `.cursorrules`?**
   - [ ] After building the first feature
   - [ ] Before using Cursor plan mode ✓
   - [ ] After deployment
   - [ ] It's optional

4. **What should you provide to Cursor plan mode?** (Select all)
   - [ ] PRD document ✓
   - [ ] All mockup PNG files ✓
   - [ ] Tech stack specification ✓
   - [ ] Complete codebase

## Exit Criteria

You're ready to proceed when:
- [ ] User stories are finalized
- [ ] PRD is complete and reviewed
- [ ] All mockups are created and exported
- [ ] Git repository is set up and cloned
- [ ] `.cursorrules` file is configured
- [ ] Cursor implementation plan is approved
- [ ] You're ready to begin building

## Dependencies & Next Steps

### Prerequisites Completed
- [Decide What to Build](decide/index.md) - Decision to build, key problems identified, innovation aspects defined

### Next Steps
- Proceed to [06 — AI Baseline](06-ai-baseline.md) to build core AI functionality
- OR proceed to [07 — UX Thin Vertical](07-ux-thin-vertical.md) to build user experience
- These can be done in parallel after setup, following your implementation plan

### What This Enables

Completing setup enables:
- Clear direction from PRD and user stories
- Visual reference from mockups
- Efficient development with Cursor and `.cursorrules`
- Structured implementation following the plan
- Quality code through established rules

### Related Resources

- [PRD Template](05-setup-prd-template.md) - Template for creating your PRD
- [.cursorrules Template](05-setup-cursorrules-template.md) - Template for Cursor development rules

---

> 💡 **Tip**: Don't rush the planning phase. A solid PRD and mockups will save significant time during development.
> 📝 **Note**: The `.cursorrules` file is critical for maintaining code quality. Take time to customize it for your needs.
> ⚠️ **Warning**: Don't skip mockups. They help Cursor understand your vision and generate better UI code.
