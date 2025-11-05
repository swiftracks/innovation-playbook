# 06 — Setup: Implementation Planning

**Purpose**: Use Cursor Plan Mode to generate and approve an implementation plan based on your PRD and mockups

**Outcome**: Have an approved implementation plan that breaks down your MVP into manageable tasks ready for building

**Audience**: PM / Dev / Both

**Time**: 1-2 hours

**Prerequisites**: [06 — Setup: .cursorrules](06-setup-cursorrules.md) - `.cursorrules` file configured

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Use Cursor Plan Mode effectively to generate implementation plans
2. Provide PRD, mockups, and tech stack to Cursor
3. Structure requests for clear, actionable plans
4. Review and evaluate implementation plans
5. Approve or refine plans based on MVP scope

## Jobs-to-Be-Done

- **When**: I have PRD, mockups, and `.cursorrules` configured, and need an implementation plan
- **I want**: To generate a comprehensive implementation plan using Cursor Plan Mode
- **So that**: I have a clear roadmap for building features with proper task sequencing

## Inputs

- PRD document from [05 — Planning: PRD & AI Baseline](05-planning-prd.md)
- Mockup PNG files from [05 — Planning: Mockups](05-planning-mockups.md)
- `.cursorrules` file configured from [06 — Setup: .cursorrules](06-setup-cursorrules.md)
- Repository open in Cursor IDE
- Understanding of Foundation Tech Stack (see below)

## Activities

### 1. Prepare Materials for Cursor Plan Mode

Before using Cursor Plan Mode, gather everything you'll provide to Cursor.

**What You Need**:
- **PRD Document**: Complete Product Requirements Document
- **Mockup Files**: All PNG mockup files (exported from UX Pilot)
- **Tech Stack**: Foundation Tech Stack specification (see section below)
- **Repository**: Open repository in Cursor with `.cursorrules` configured

**Preparation Steps**:
1. **Locate PRD**: Ensure your PRD document is accessible
   - Can be a markdown file, document, or text
   - Should be complete with all sections
   - Make sure it's up to date

2. **Gather Mockup Files**: Collect all PNG mockup files
   - Ensure all screens are exported
   - Files should be clearly named
   - Organize files if needed (e.g., in a `mockups/` folder)

3. **Review Tech Stack**: Familiarize yourself with the Foundation Tech Stack
   - Review the tech stack section below
   - Note versions and specific packages
   - Understand key technologies

4. **Verify Setup**: Ensure repository is ready
   - Repository is open in Cursor
   - `.cursorrules` file is configured
   - You're ready to proceed

> 💡 **Tip**: Having all materials ready before starting will make the planning process smoother and more effective.

### 2. Use Cursor Plan Mode

Use Cursor's Plan Mode to generate an implementation plan based on your PRD and mockups.

**Process**:

#### Step 1: Access Plan Mode

1. **Open Cursor**: Ensure your repository is open in Cursor
2. **Access Plan Mode**:
   - Look for "Plan Mode" or "Planning" feature in Cursor
   - This may be in the sidebar, menu, or command palette
   - Use `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac) to open command palette
   - Type "Plan" or "Planning" to find the feature

#### Step 2: Provide PRD Document

1. **Provide PRD**: 
   - Copy and paste your PRD content into Cursor
   - Or upload the PRD file if Cursor supports file upload
   - Ensure the complete PRD is provided

2. **Verify PRD**: 
   - Check that all sections are included
   - Ensure PRD is complete and clear
   - Note any sections you want to emphasize

#### Step 3: Upload Mockup Files

1. **Upload Mockups**: 
   - Upload all PNG mockup files to Cursor
   - Use Cursor's file upload feature (drag-and-drop or file picker)
   - Upload all screens, not just key ones

2. **Organize Mockups**: 
   - If possible, upload in order of user flow
   - Name files clearly if not already named
   - Ensure all screens are included

#### Step 4: Specify Foundation Tech Stack

1. **Provide Tech Stack**: 
   - Copy the Foundation Tech Stack specification (see section below)
   - Paste it into your request to Cursor
   - Ensure all versions and packages are included

2. **Customize if Needed**: 
   - If you're using different versions, update them
   - If you're using different packages, specify them
   - Ensure tech stack matches your actual implementation plan

#### Step 5: Request Implementation Plan

1. **Structure Your Request**: 
   - Use a clear, structured request format
   - Include all materials: PRD, mockups, tech stack
   - Specify what you want in the plan

2. **Example Request**:
```
I'm building an MVP using this PRD:

[Paste PRD content here]

Mockups: [Upload all PNG files]

Tech Stack:
- Core Framework: React 19, TypeScript 5.9.3, Vite 7.7
- Routing & State: React Router DOM 7.4, Zustand 5.8
- UI & Styling: Tailwind CSS 3.3.6, Radix UI (Dialog, Dropdown Menu, Select, Label, Slot, Tabs, Toast), Lucide React 0.546, Heroicons React 2.0
- Utilities: class-variance-authority, clsx
- Backend: Firebase 12.4.0 (Authentication, Cloud Firestore, Firebase Hosting)
- AI Integration: Anthropic SDK 0.67.0 (Claude API)
- Monitoring: LogRocket 10.1.0
- Development Tools: PostCSS, Autoprefixer, ESBuild

Generate a comprehensive implementation plan that:
1. Breaks down the work into logical phases and tasks
2. Prioritizes core MVP features first
3. Identifies dependencies between tasks
4. Follows MVP scope (not over-engineering)
5. Aligns with the mockups provided
6. Uses the specified tech stack
7. Follows the .cursorrules configuration
```

3. **Additional Guidance**: 
   - Specify if you want phases, sprints, or just tasks
   - Request specific formatting if needed
   - Ask for dependency identification
   - Request time estimates if helpful

> 📝 **Note**: The quality of your request will affect the quality of the plan. Be clear and specific about what you need.

### 3. Review Generated Implementation Plan

Review Cursor's generated implementation plan carefully.

**Review Process**:

1. **Read Through Plan**: 
   - Read the entire plan from start to finish
   - Understand the overall structure
   - Note how tasks are organized

2. **Check Completeness**: 
   - Verify all PRD features are covered
   - Check that all mockup screens are addressed
   - Ensure no major features are missing

3. **Evaluate Task Sequencing**: 
   - Review task order and dependencies
   - Verify logical flow (setup → core features → enhancements)
   - Check that dependencies are properly identified

4. **Assess MVP Scope**: 
   - Ensure plan follows MVP scope (not over-engineering)
   - Verify plan doesn't include future features
   - Check that it focuses on core value delivery

5. **Verify Tech Stack Alignment**: 
   - Confirm plan uses specified tech stack
   - Check that packages and versions match
   - Verify no conflicting technologies

6. **Check Mockup Alignment**: 
   - Verify plan addresses all mockup screens
   - Check that UI components match mockups
   - Ensure flow matches mockup sequence

**Review Checklist**:
- [ ] Plan covers all PRD features
- [ ] Tasks are logically sequenced
- [ ] Plan follows MVP scope (not over-engineering)
- [ ] Dependencies are identified
- [ ] Plan aligns with mockups
- [ ] Tech stack matches specification
- [ ] Plan follows `.cursorrules` guidelines
- [ ] Task breakdown is manageable
- [ ] No missing features or screens

### 4. Refine Plan if Needed

If the plan needs adjustments, provide feedback to Cursor and request revisions.

**Refinement Process**:

1. **Identify Issues**: 
   - Note what needs to change
   - Be specific about problems
   - Prioritize critical issues

2. **Provide Feedback**: 
   - Give clear, specific feedback
   - Explain what's wrong and why
   - Suggest improvements

3. **Request Revisions**: 
   - Ask for specific changes
   - Request reordering if needed
   - Ask for additional detail if needed

**Example Refinement Request**:
```
The plan looks good overall, but I need some adjustments:

1. Task sequencing: Move authentication setup before user features
2. Missing feature: The plan doesn't include the dashboard empty state
3. Over-engineering: Task #15 includes features outside MVP scope
4. Dependencies: Task #8 should come before Task #12

Please revise the plan with these changes.
```

4. **Iterate Until Satisfied**: 
   - Review revised plan
   - Check that issues are addressed
   - Request additional changes if needed
   - Continue until plan is acceptable

**Common Issues to Watch For**:
- **Missing Features**: Plan doesn't cover all PRD features
- **Wrong Sequencing**: Tasks are in incorrect order
- **Over-Engineering**: Plan includes non-MVP features
- **Missing Dependencies**: Tasks that depend on others aren't sequenced properly
- **Tech Stack Mismatch**: Plan uses different technologies than specified
- **Mockup Mismatch**: Plan doesn't align with mockup screens

### 5. Approve Implementation Plan

Once the plan meets your requirements, approve it and prepare for building.

**Approval Process**:

1. **Final Review**: 
   - Do a final review of the complete plan
   - Verify all checkpoints are met
   - Ensure you're confident in the plan

2. **Document Plan**: 
   - Save the plan (if Cursor allows)
   - Or copy it to a document/file
   - Keep it accessible for reference

3. **Prepare for Building**: 
   - Ensure repository is ready
   - Verify `.cursorrules` is configured
   - Have PRD and mockups accessible
   - Prepare to start building

**Approval Checklist**:
- [ ] Plan covers all PRD features
- [ ] Tasks are logically sequenced
- [ ] Dependencies are clear
- [ ] Plan follows MVP scope
- [ ] Plan aligns with mockups
- [ ] Tech stack matches specification
- [ ] Plan is documented and saved
- [ ] Ready to proceed to building

> 💡 **Tip**: A good implementation plan will save significant time during development. Don't rush the review process.

## Foundation Tech Stack

This tech stack is optimized for rapid MVP development as of November 2024. Provide this specification to Cursor when generating your implementation plan.

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

**Task**: Generate and approve implementation plan using Cursor Plan Mode

1. Prepare materials
   - Have PRD document ready
   - Gather all mockup PNG files
   - Review Foundation Tech Stack

2. Use Cursor Plan Mode
   - Access Plan Mode in Cursor
   - Provide PRD document
   - Upload all mockup files
   - Specify Foundation Tech Stack
   - Request comprehensive implementation plan

3. Review generated plan
   - Check completeness (all PRD features covered)
   - Verify task sequencing
   - Ensure MVP scope is followed
   - Check dependencies are identified
   - Verify mockup alignment

4. Refine plan if needed
   - Identify issues
   - Provide specific feedback
   - Request revisions
   - Iterate until satisfied

5. Approve plan
   - Final review
   - Document and save plan
   - Prepare for building

**Artifacts**: You'll create:
- Implementation plan generated by Cursor
- Approved plan document
- Task breakdown ready for building

## Artifacts

You'll create:
- Cursor-generated implementation plan
- Approved and refined plan document
- Task breakdown with dependencies identified

## Worked Example

**Situation**: Generating implementation plan for a B2B AI SaaS retrospective tool

**Implementation Planning Process**:
1. **Preparation**: 
   - Gathered complete PRD document
   - Collected 10 PNG mockup files
   - Reviewed Foundation Tech Stack

2. **Cursor Plan Mode**: 
   - Opened Cursor Plan Mode
   - Pasted complete PRD content
   - Uploaded all 10 mockup PNG files
   - Provided Foundation Tech Stack specification
   - Requested comprehensive implementation plan

3. **Generated Plan**: 
   - Cursor generated 15-task implementation plan
   - Organized into 4 phases:
     - Phase 1: Project setup and configuration
     - Phase 2: Authentication and core infrastructure
     - Phase 3: Core MVP features
     - Phase 4: Polish and deployment
   - Identified dependencies between tasks

4. **Review**: 
   - Reviewed plan against PRD: All features covered ✓
   - Checked sequencing: Logical flow ✓
   - Verified MVP scope: No over-engineering ✓
   - Checked dependencies: Properly identified ✓
   - Verified mockup alignment: All screens addressed ✓

5. **Refinement**: 
   - Requested one adjustment: Move dashboard empty state earlier
   - Cursor revised plan
   - Reviewed revised plan: Approved ✓

6. **Approval**: 
   - Documented plan in `IMPLEMENTATION_PLAN.md`
   - Committed to repository
   - Ready to proceed to building

**Time**: 1.5 hours total (1 hour generation and review, 30 min refinement)

## Checklist

Before proceeding to building features, verify:
- [ ] PRD document provided to Cursor
- [ ] All mockup PNG files uploaded
- [ ] Foundation Tech Stack specified
- [ ] Implementation plan generated by Cursor
- [ ] Plan reviewed for completeness
- [ ] Plan reviewed for task sequencing
- [ ] Plan reviewed for MVP scope alignment
- [ ] Dependencies identified in plan
- [ ] Plan aligns with mockups
- [ ] Plan refined if needed
- [ ] Plan approved and documented
- [ ] Ready to proceed to building

## Self-Assessment

1. **What should you provide to Cursor Plan Mode?** (Select all)
   - [ ] PRD document ✓
   - [ ] All mockup PNG files ✓
   - [ ] Foundation Tech Stack specification ✓
   - [ ] Complete codebase

2. **What should you review in the implementation plan?** (Select all)
   - [ ] Plan covers all PRD features ✓
   - [ ] Tasks are logically sequenced ✓
   - [ ] Plan follows MVP scope ✓
   - [ ] Plan includes all future features

3. **What should you do if the plan needs adjustments?**
   - [ ] Accept it as-is
   - [ ] Provide feedback and request revisions ✓
   - [ ] Start building anyway
   - [ ] Skip the plan

## Exit Criteria

You're ready to proceed to building features when:
- [ ] Implementation plan is generated by Cursor
- [ ] Plan is reviewed and approved
- [ ] Plan covers all PRD features
- [ ] Task sequencing is logical
- [ ] Dependencies are identified
- [ ] Plan follows MVP scope
- [ ] Plan is documented and saved
- [ ] Ready to begin building

## Dependencies & Next Steps

### Prerequisites Completed
- [06 — Setup: .cursorrules](06-setup-cursorrules.md) - `.cursorrules` file configured

### Next Steps
- Proceed to [08 — Build Features](08-build-features.md) to build features end-to-end using Cursor collaboration following the approved plan

### What This Enables

Completing implementation planning enables:
- Clear roadmap for building features
- Proper task sequencing and dependencies
- Structured approach to MVP development
- Efficient collaboration with Cursor
- Reduced time on planning during development

### Related Resources

- [06 — Setup](06-setup.md) - Return to Setup overview
- [05 — Planning: PRD & AI Baseline](05-planning-prd.md) - Reference for PRD
- [05 — Planning: Mockups](05-planning-mockups.md) - Reference for mockups

---

> 💡 **Tip**: Take time to review the implementation plan carefully. A good plan will save significant time during development.
> 📝 **Note**: You can refine the plan as you learn more during development. The plan is a guide, not a rigid contract.
> ⚠️ **Warning**: Don't skip the plan review. Ensure it aligns with your PRD and MVP scope before proceeding to building.

