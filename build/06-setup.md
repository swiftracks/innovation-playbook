# 06 — Setup

**Purpose**: Set up development environment and create implementation plan

**Outcome**: Have a working development environment and an approved implementation plan ready for building

**Audience**: PM / Dev / Both

**Time**: 4-8 hours

**Prerequisites**: [05 — Planning](05-planning.md) - User stories, PRD, and mockups complete

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

- User stories, PRD, and mockups from [05 — Planning](05-planning.md)
- GitLab or GitHub account for version control
- Cursor IDE installed
- Understanding of foundation tech stack (see [06 — Setup: Implementation Planning](06-setup-implementation-planning.md))

## Setup Workflow

Setup follows a sequential workflow with three main activities:

1. **[Git & Cursor Setup](06-setup-git-cursor.md)**: Create Git repository and clone in Cursor IDE
2. **[.cursorrules Configuration](06-setup-cursorrules.md)**: Configure development rules for rapid MVP development
3. **[Implementation Planning](06-setup-implementation-planning.md)**: Use Cursor Plan Mode to generate and approve implementation plan

> 💡 **Tip**: Follow the activities in order. Each builds on the previous one.

## Activities Overview

### 1. Git & Cursor Setup

**Purpose**: Create Git repository and clone it in Cursor IDE

**Key Steps**:
- Create a new repository in GitLab or GitHub
- Clone the repository in Cursor
- Verify the setup is correct

**Time**: 15-30 minutes

**Detailed Guide**: [06 — Setup: Git & Cursor](06-setup-git-cursor.md)

### 2. .cursorrules Configuration

**Purpose**: Configure `.cursorrules` file with development rules for rapid MVP development

**Key Steps**:
- Review the `.cursorrules` template
- Create `.cursorrules` file in project root
- Customize rules based on your specific needs
- Test configuration with Cursor

**Time**: 30-60 minutes

**Detailed Guide**: [06 — Setup: .cursorrules](06-setup-cursorrules.md)

### 3. Implementation Planning

**Purpose**: Use Cursor Plan Mode to generate and approve an implementation plan

**Key Steps**:
- Prepare PRD, mockups, and tech stack
- Use Cursor Plan Mode to generate implementation plan
- Review and refine the plan
- Approve the plan for building

**Time**: 1-2 hours

**Detailed Guide**: [06 — Setup: Implementation Planning](06-setup-implementation-planning.md)

## Apply It Now

**Task**: Set up development environment and create implementation plan

Follow the sequential workflow:

1. **Git & Cursor Setup**: Complete [06 — Setup: Git & Cursor](06-setup-git-cursor.md)
   - Create GitLab or GitHub repository
   - Clone repository in Cursor
   - Verify setup

2. **.cursorrules Configuration**: Complete [06 — Setup: .cursorrules](06-setup-cursorrules.md)
   - Review template
   - Create and customize `.cursorrules` file
   - Test configuration

3. **Implementation Planning**: Complete [06 — Setup: Implementation Planning](06-setup-implementation-planning.md)
   - Prepare PRD, mockups, and tech stack
   - Use Cursor Plan Mode
   - Review and approve implementation plan

**Artifacts**: You'll create:
- Git repository with `.cursorrules`
- Cursor implementation plan
- Initial project structure ready for building

## Artifacts

You'll create throughout setup:
- Git repository configuration
- `.cursorrules` file
- Cursor implementation plan
- Initial project structure

## Worked Example

**Situation**: Setting up for a B2B AI SaaS MVP

**Setup Process**:
1. **Git & Cursor Setup** ([06 — Setup: Git & Cursor](06-setup-git-cursor.md)): Created GitHub repository `mvp-product-name`
   - Cloned repository in Cursor
   - Verified setup
   - Time: 15 minutes

2. **.cursorrules Configuration** ([06 — Setup: .cursorrules](06-setup-cursorrules.md)): Created `.cursorrules` with rules for:
   - TypeScript strict mode
   - React best practices
   - Component organization
   - Error handling standards
   - MVP-specific guidelines
   - Customized for retrospective tool
   - Time: 45 minutes

3. **Implementation Planning** ([06 — Setup: Implementation Planning](06-setup-implementation-planning.md)): Provided PRD, 10 mockup PNGs, and tech stack
   - Cursor generated 15-task implementation plan
   - Reviewed and approved plan (1 adjustment requested)
   - Time: 1.5 hours

**Time**: Setup took 2.5 hours total

## Checklist

Before proceeding to the next chapter, verify:

**Git & Cursor Setup** ([06 — Setup: Git & Cursor](06-setup-git-cursor.md)):
- [ ] Git repository created
- [ ] Repository cloned in Cursor
- [ ] Setup verified

**.cursorrules Configuration** ([06 — Setup: .cursorrules](06-setup-cursorrules.md)):
- [ ] `.cursorrules` file created in project root
- [ ] Rules customized for your MVP
- [ ] Configuration tested with Cursor
- [ ] File committed to repository

**Implementation Planning** ([06 — Setup: Implementation Planning](06-setup-implementation-planning.md)):
- [ ] Cursor Plan Mode used with PRD and mockups
- [ ] Implementation plan generated
- [ ] Plan reviewed and approved
- [ ] Plan documented and saved

## Self-Assessment

1. **What should you do first in the setup phase?**
   - [ ] Configure `.cursorrules`
   - [ ] Create Git repository and clone in Cursor ✓
   - [ ] Generate implementation plan
   - [ ] Start building features

2. **When should you set up `.cursorrules`?**
   - [ ] After building the first feature
   - [ ] Before using Cursor Plan Mode ✓
   - [ ] After deployment
   - [ ] It's optional

3. **What should you provide to Cursor Plan Mode?** (Select all)
   - [ ] PRD document ✓
   - [ ] All mockup PNG files ✓
   - [ ] Tech stack specification ✓
   - [ ] Complete codebase

4. **What should you review in the implementation plan?** (Select all)
   - [ ] Plan covers all PRD features ✓
   - [ ] Tasks are logically sequenced ✓
   - [ ] Plan follows MVP scope ✓
   - [ ] Plan includes all future features

## Exit Criteria

You're ready to proceed to [08 — Build Features](08-build-features.md) when:
- [ ] Git repository is set up and cloned
- [ ] `.cursorrules` file is configured
- [ ] Cursor implementation plan is approved
- [ ] You're ready to begin building

## Dependencies & Next Steps

### Prerequisites Completed
- [05 — Planning](05-planning.md) - User stories, PRD, and mockups complete

### Next Steps

Follow the sequential workflow:

1. **Start with**: [06 — Setup: Git & Cursor](06-setup-git-cursor.md) - Create Git repository and clone in Cursor
2. **Then**: [06 — Setup: .cursorrules](06-setup-cursorrules.md) - Configure development rules
3. **Then**: [06 — Setup: Implementation Planning](06-setup-implementation-planning.md) - Generate and approve implementation plan
4. **Finally**: Proceed to [08 — Build Features](08-build-features.md) - Build features end-to-end using Cursor collaboration

### What This Enables

Completing setup enables:
- Efficient development with Cursor and `.cursorrules`
- Structured implementation following the plan
- Quality code through established rules
- Clear direction from approved plan

### Related Resources

- [06 — Setup: Git & Cursor](06-setup-git-cursor.md) - Detailed Git and Cursor setup guide
- [06 — Setup: .cursorrules](06-setup-cursorrules.md) - Detailed `.cursorrules` configuration guide
- [06 — Setup: Implementation Planning](06-setup-implementation-planning.md) - Detailed implementation planning guide
- [.cursorrules Template](05-setup-cursorrules-template.md) - Template for Cursor development rules

---

> 💡 **Tip**: The `.cursorrules` file is critical for maintaining code quality. Take time to customize it for your needs.
> 📝 **Note**: Review Cursor's implementation plan carefully. A good plan will save significant time during development.
> ⚠️ **Warning**: Don't skip the implementation plan review. Ensure it aligns with your PRD and MVP scope before proceeding to building.
