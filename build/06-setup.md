# 06 — Setup

**Purpose**: Set up development environment and create implementation plan

**Outcome**: Have a working development environment and an approved implementation plan ready for building

**Audience**: PM / Dev / Both

**Time**: 4-8 hours

**Prerequisites**: [05 — Planning](05-planning) - User stories, PRD, and mockups complete

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Set up Git repository and clone in Cursor
2. Configure `.cursorrules` for rapid MVP development
3. Use Cursor's plan mode to generate implementation plans
4. Review and approve implementation plans
5. Prepare development environment for building

## Jobs-to-Be-Done

- **When**: I have a complete plan (user stories, PRD, mockups) and need to set up development
- **I want**: To set up development environment and create an implementation plan
- **So that**: I can build efficiently with clear direction and proper tooling

## Inputs

- User stories, PRD, and mockups from [05 — Planning](05-planning)
- GitLab or GitHub account for version control
- Cursor IDE installed
- Understanding of foundation tech stack

## Activities

### 1. Create Git Repository

Create a new GitLab or GitHub project for your MVP.

**Steps**:
1. Create a new repository in GitLab or GitHub
2. Initialize with a README (optional)
3. Note the repository URL

> 💡 **Tip**: Choose a repository name that reflects your MVP. Keep it simple and descriptive.

### 2. Clone Repository in Cursor

Open Cursor and clone your Git repository.

**Steps**:
1. Open Cursor IDE
2. Use File → Open Folder or Clone Repository
3. Enter your Git repository URL
4. Clone the repository to your local machine
5. Open the cloned folder in Cursor

### 3. Set Up .cursorrules

Create a `.cursorrules` file in your project root with strong rules for rapid MVP development.

**Process**:
1. Create a `.cursorrules` file in the project root
2. Use the [.cursorrules template](05-setup-cursorrules-template) as a starting point
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

### 4. Use Cursor Plan Mode

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

### 5. Review and Approve Implementation Plan

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

**Task**: Set up development environment and create implementation plan

1. Create GitLab or GitHub repository
2. Clone repository in Cursor
3. Set up `.cursorrules` file with development rules
4. Use Cursor plan mode with PRD, mockups, and tech stack
5. Review and approve implementation plan

**Artifacts**: You'll create:
- Git repository with `.cursorrules`
- Cursor implementation plan
- Initial project structure ready for building

## Artifacts

You'll create:
- Git repository configuration
- `.cursorrules` file
- Cursor implementation plan
- Initial project structure

## Worked Example

**Situation**: Setting up for a B2B AI SaaS MVP

**Setup Process**:
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
5. **Ready to Build**: Project structure ready for implementation

**Time**: Setup took 6 hours

## Checklist

Before proceeding to the next chapter, verify:
- [ ] Git repository created
- [ ] Repository cloned in Cursor
- [ ] `.cursorrules` file created and customized
- [ ] Cursor plan mode used with PRD and mockups
- [ ] Implementation plan reviewed and approved
- [ ] Initial project structure ready

## Self-Assessment

1. **When should you set up `.cursorrules`?**
   - [ ] After building the first feature
   - [ ] Before using Cursor plan mode ✓
   - [ ] After deployment
   - [ ] It's optional

2. **What should you provide to Cursor plan mode?** (Select all)
   - [ ] PRD document ✓
   - [ ] All mockup PNG files ✓
   - [ ] Tech stack specification ✓
   - [ ] Complete codebase

3. **What should you review in the implementation plan?** (Select all)
   - [ ] Plan covers all PRD features ✓
   - [ ] Tasks are logically sequenced ✓
   - [ ] Plan follows MVP scope ✓
   - [ ] Plan includes all future features

## Exit Criteria

You're ready to proceed when:
- [ ] Git repository is set up and cloned
- [ ] `.cursorrules` file is configured
- [ ] Cursor implementation plan is approved
- [ ] You're ready to begin building

## Dependencies & Next Steps

### Prerequisites Completed
- [05 — Planning](05-planning) - User stories, PRD, and mockups complete

### Next Steps
- Proceed to [07 — AI Baseline](07-ai-baseline) to build core AI functionality
- OR proceed to [08 — Build Features](08-build-features) to implement UI based on mockups
- These can be done in parallel after setup, following your implementation plan

### What This Enables

Completing setup enables:
- Efficient development with Cursor and `.cursorrules`
- Structured implementation following the plan
- Quality code through established rules
- Clear direction from approved plan

### Related Resources

- [.cursorrules Template](05-setup-cursorrules-template) - Template for Cursor development rules

---

> 💡 **Tip**: The `.cursorrules` file is critical for maintaining code quality. Take time to customize it for your needs.
> 📝 **Note**: Review Cursor's implementation plan carefully. A good plan will save significant time during development.
> ⚠️ **Warning**: Don't skip the implementation plan review. Ensure it aligns with your PRD and MVP scope.

