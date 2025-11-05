# 08 — Build Features

**Purpose**: Build features end-to-end using Cursor collaboration, following the approved implementation plan

**Outcome**: Have working features that match the designed user journey, built through iterative Cursor collaboration

**Audience**: PM / Dev / Both

**Time**: 1-2 weeks

**Prerequisites**: [06 — Setup](06-setup.md) - Comprehensive Cursor Plan approved to develop the product end-to-end including AI components

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Collaborate effectively with Cursor to build features following an approved plan
2. Test and iterate using `npm run dev` throughout the development process
3. Use Cursor's planning function to fix issues and enhance features
4. Guide Cursor through questions and approvals during development
5. Refine features iteratively until ready for private beta

## Jobs-to-Be-Done

- **When**: I have an approved Cursor implementation plan and need to build the product
- **I want**: To collaborate with Cursor to build features end-to-end following the plan
- **So that**: I have a working MVP ready for private beta testing

## Inputs

- Approved Cursor implementation plan from [06 — Setup](06-setup.md)
- Mockups from [05 — Planning](05-planning.md) (designed journey)
- PRD from [05 — Planning](05-planning.md) (including AI Baseline design)
- Development environment configured with `.cursorrules`
- Cursor IDE ready for collaboration

## Activities

### 1. Approve and Start Building

**Review Cursor Plan**:
- Review the comprehensive Cursor plan that includes all features and AI components
- Ensure the plan covers all PRD requirements and follows the designed user journey
- The plan should include order of priority and dependencies - Cursor has already determined this in the planning phase

**Start Building**:
- In Cursor, approve the plan and click "Build" (or equivalent action to begin implementation)
- Cursor will begin scaffolding and building features according to the plan
- Trust Cursor's recommended plan and order of priority from the planning phase

> 💡 **Tip**: If you have concerns about the plan, address them before starting. Once building begins, let Cursor follow its plan.

### 2. Collaborate with Cursor During Building

**Cursor's Building Process**:
- Cursor will scaffold the project structure
- Cursor will build features following the approved plan
- Cursor may ask questions or request approvals for certain tasks
- Some tasks may need to be filled manually - follow Cursor's instructions

**Your Role During Building**:
- **Answer Questions**: When Cursor asks questions, provide clear answers based on your PRD and mockups
- **Provide Approvals**: When Cursor requests approval, review the approach and approve if appropriate
- **Use "ASK" Function**: If you're unsure about something, use Cursor's "ASK" function to get clarification
- **Continue Working with Cursor**: Stay engaged - Cursor may need guidance on next steps or clarification on requirements

**Best Practices for Large Plans**:
- If the plan is large, Cursor will break it down into manageable tasks
- Cursor will present the plan and ask for approval before proceeding
- You can approve sections of the plan as Cursor progresses
- Cursor will navigate through the plan systematically, asking questions when needed

> 📝 **Note**: Cursor is designed to handle large plans. Trust its process and provide guidance when asked. Don't try to micromanage the implementation order.

### 3. Test Throughout Development

**Start Development Server**:
- Use `npm run dev` to boot up the development environment
- Test the application as Cursor builds features
- Keep the dev server running throughout the development process

**Iterative Testing**:
- As Cursor builds features, test them in the browser
- Navigate through the user journey as it's implemented
- Verify that features work as expected
- Check that the UI matches the mockups from Planning

> 💡 **Tip**: Test frequently, not just at the end. Early testing helps catch issues before they compound.

### 4. Identify and Fix Issues

**When You Find Issues**:
- As you test, you'll notice some features may not be built perfectly
- Some experiences may not make sense
- Components may not match the mockups exactly
- Features may have bugs or edge cases not handled

**Using Cursor Planning for Fixes**:
- When you find issues, use Cursor's planning function in a new chat
- Provide Cursor with a detailed list of issues and problems:
  - What component or feature has the issue
  - What the expected behavior is
  - What the actual behavior is
  - Any relevant context or screenshots
- Allow Cursor to present a plan to fix, add, or enhance features
- Review and approve the fix plan
- Let Cursor implement the fixes

**Example Issue Report for Cursor**:
```
I've found these issues while testing:
1. Login form doesn't show validation errors
2. Dashboard cards don't match the mockup layout
3. AI insights generation is slow and needs loading state
4. Export button doesn't work on mobile devices

Please create a plan to fix these issues.
```

> 💡 **Tip**: Be specific about issues. The more detail you provide, the better Cursor can plan and fix them.

### 5. Continue Iterative Refinement

**Refinement Cycle**:
1. Cursor builds features
2. You test with `npm run dev`
3. You identify issues or improvements
4. You use Cursor planning to create a fix plan
5. Cursor implements fixes
6. You test again
7. Repeat until satisfied

**Continue Testing**:
- Use `npm run dev` throughout the entire testing process
- Test the complete user journey end-to-end
- Test error cases and edge states
- Test with different data scenarios
- Verify all features work together

**Refinement Criteria**:
- Features work as expected
- UI matches mockups (or improvements are acceptable)
- User journey is smooth and intuitive
- No critical bugs or broken features
- Ready for private beta testing

> 📝 **Note**: Don't aim for perfection. Focus on reaching a point of satisfaction for private beta. You can iterate further based on user feedback.

## Apply It Now

**Task**: Build features using Cursor collaboration

1. Review and approve the Cursor implementation plan
2. Click "Build" in Cursor to begin implementation
3. Answer questions and provide approvals as Cursor builds
4. Use `npm run dev` to test throughout development
5. Document issues and problems as you find them
6. Use Cursor planning function to fix issues
7. Continue iterative testing and refinement
8. Reach satisfaction point for private beta

**Artifact**: Working features with:
- Complete user journey implemented
- All features from PRD built
- AI components integrated (if applicable)
- UI matching mockups
- Ready for private beta

## Artifacts

You'll create:
- Working application with all features built
- Complete user journey implemented
- Backend integration (Firebase, AI, etc.)
- Issue documentation and fixes
- Test results and refinement notes

## Worked Example

**Situation**: Building features for retrospective tool MVP using Cursor

**Building Process**:
1. **Approved Plan**: Reviewed comprehensive Cursor plan covering all features and AI components
   - Plan included 25 tasks with proper dependencies
   - Cursor determined order of priority automatically
   - Approved plan and clicked "Build"

2. **Cursor Building**: Cursor began scaffolding and building
   - Cursor asked 3 questions about authentication flow
   - Provided answers based on PRD
   - Cursor built authentication, dashboard, and core features
   - Cursor requested approval for AI integration approach - approved

3. **Testing**: Started `npm run dev` and tested as features were built
   - Tested authentication flow - worked well
   - Tested dashboard - layout didn't match mockup
   - Tested core journey - AI insights were slow
   - Found 5 issues total

4. **Fixing Issues**: Used Cursor planning in new chat
   - Provided detailed list of 5 issues
   - Cursor created fix plan with 8 tasks
   - Approved fix plan
   - Cursor implemented fixes
   - Tested again - 4 of 5 issues fixed

5. **Iterative Refinement**: Continued cycle
   - Found 2 more minor issues
   - Used Cursor planning again
   - Cursor fixed remaining issues
   - Tested complete journey - satisfied

6. **Ready for Beta**: Reached satisfaction point
   - All features working
   - UI matches mockups
   - User journey smooth
   - Ready for private beta

**Time**: Building took 12 days with iterative refinement

## Checklist

Before proceeding to the next chapter, verify:
- [ ] Cursor implementation plan is approved
- [ ] Cursor has built all features from the plan
- [ ] You've tested with `npm run dev` throughout development
- [ ] All issues have been identified and fixed
- [ ] Complete user journey works end-to-end
- [ ] Features are ready for private beta
- [ ] You've reached a point of satisfaction

## Self-Assessment

1. **When should you start testing?**
   - [ ] After all features are built
   - [ ] Throughout the development process ✓
   - [ ] Only at the end
   - [ ] Before starting to build

2. **What should you do when you find issues?** (Select all)
   - [ ] Fix them manually
   - [ ] Use Cursor planning function to create a fix plan ✓
   - [ ] Provide detailed list of issues to Cursor ✓
   - [ ] Ignore them and move on

3. **How should you handle Cursor's questions during building?**
   - [ ] Ignore them
   - [ ] Answer based on PRD and mockups ✓
   - [ ] Tell Cursor to figure it out
   - [ ] Stop building

## Exit Criteria

You're ready to proceed when:
- [ ] All features from the Cursor plan are built
- [ ] You've tested thoroughly with `npm run dev`
- [ ] All identified issues have been fixed
- [ ] Complete user journey works end-to-end
- [ ] Features match mockups and PRD requirements
- [ ] You've reached satisfaction point for private beta

## Dependencies & Next Steps

### Prerequisites Completed
- [05 — Planning](05-planning.md) - Mockups, PRD, and AI Baseline design
- [06 — Setup](06-setup.md) - Comprehensive Cursor Plan approved

### Next Steps
- Proceed to [09 — Deploy](09-deploy.md) to conduct QA and deploy MVP

### What This Enables

Built features enable:
- Complete user value demonstration
- Private beta testing opportunity
- Learning from real user feedback
- Iteration and improvement based on usage

---

> 💡 **Tip**: Trust Cursor's plan and process. Your role is to guide, test, and provide feedback. Let Cursor do the heavy lifting.
> 📝 **Note**: The order of priority was determined by Cursor in the planning phase. Follow Cursor's recommended plan and order.
> ⚠️ **Warning**: Don't skip testing. Test frequently throughout development to catch issues early. Use `npm run dev` regularly.
