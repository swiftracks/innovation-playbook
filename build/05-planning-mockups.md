# 05 — Planning: Mockups

**Purpose**: Design complete user journeys and create visual mockups using UX Pilot

**Outcome**: Have all mockups created and exported as PNG files ready for implementation planning

**Audience**: PM / Dev / Both

**Time**: 2-4 hours

**Prerequisites**: [05 — Planning: PRD & AI Baseline](05-planning-prd.md) - Complete PRD with user journeys defined

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Identify key user flows from your PRD
2. Create user flows in UX Pilot
3. Generate screens for each step in user journeys
4. Iterate on mockups based on UX best practices
5. Export all mockups to PNG format ready for implementation

## Jobs-to-Be-Done

- **When**: I have a complete PRD and need to visualize the user journey
- **I want**: To create visual mockups that communicate my vision
- **So that**: Cursor can understand the UI structure during implementation

## Inputs

- Complete PRD from [05 — Planning: PRD & AI Baseline](05-planning-prd.md)
- User journeys defined in PRD
- Access to UX Pilot for mockup generation
- Understanding of UX best practices

## Activities

### 1. Review PRD and Identify User Flows

Before creating mockups, review your PRD to identify all user flows that need mockups.

**What to Review**:
- User Journeys section in PRD
- Functional Requirements section
- User flows mentioned in the PRD
- Acceptance criteria that reference screens

**Key Flows to Identify**:
- Authentication flow (signup/login)
- Primary user journey (core value delivery)
- Secondary user journeys
- Error and edge case states
- Empty states
- AI interaction flows (if applicable)

**Flow Identification Process**:
1. Read through User Journeys section in PRD
2. Identify each step in the journey
3. Note which steps need screens
4. Identify error states and edge cases
5. List all flows that need mockups

**Example Flow Breakdown**:
- **Authentication Flow**: Login screen → Signup screen → Forgot password screen
- **Primary Journey**: Dashboard → Create action → View results → Share results
- **Error States**: Invalid login → Error message screen
- **Empty States**: Empty dashboard → No data message

### 2. Create User Flows in UX Pilot

Use UX Pilot to create flows for each major user journey.

**Process**:
1. Open UX Pilot
2. Create a new flow for each user journey
3. Name flows descriptively (e.g., "Authentication Flow", "Primary User Journey")
4. Organize flows logically
5. Add flow descriptions if helpful

**Flow Creation Process**:
1. **Start New Flow**: Click "Create Flow" or equivalent
2. **Name Flow**: Use descriptive name from PRD
3. **Add Description**: Brief description of the flow's purpose
4. **Save Flow**: Save flow before adding screens

**Best Practices**:
- Create one flow per major user journey
- Use clear, descriptive flow names
- Organize flows in logical order
- Keep flows focused (one complete journey per flow)

### 3. Generate Screens for Each Flow

Generate screens for each step in your user flows.

**Process**:
1. For each flow, identify all screens needed
2. Generate screens in UX Pilot for each step
3. Ensure screens match the PRD requirements
4. Include all screens referenced in PRD
5. Add screens for error states and edge cases

**Screen Generation Process**:
1. **Select Flow**: Choose the flow you're working on
2. **Add Screen**: Click "Add Screen" or equivalent
3. **Generate Screen**: Use UX Pilot's generation feature
4. **Provide Context**: Describe the screen's purpose and content
5. **Review Screen**: Ensure screen matches PRD requirements
6. **Iterate**: Refine screen if needed

**Screen Generation Tips**:
- Provide clear context about what the screen should show
- Reference the PRD for specific requirements
- Include all elements mentioned in acceptance criteria
- Consider user flow and navigation between screens
- Think about responsive design needs

**Example Screen Generation Prompt**:
```
Create a login screen for a B2B AI SaaS product:
- Email input field
- Password input field
- "Log in" button
- "Forgot password?" link
- Clean, professional design
- Brand colors: [colors]
```

### 4. Iterate on Mockups

Iterate on mockups based on UX best practices and PRD requirements.

**Iteration Process**:
1. Review each screen against PRD requirements
2. Check user flow and navigation
3. Ensure consistency across screens
4. Verify all acceptance criteria are met
5. Refine screens that need improvement

**UX Review Checklist**:
- [ ] Screens match PRD requirements
- [ ] User flow is clear and logical
- [ ] Navigation is intuitive
- [ ] All screens in PRD are created
- [ ] Error states are handled
- [ ] Empty states are designed
- [ ] Consistent design language
- [ ] Responsive design considered

**Iteration Tips**:
- Test the flow mentally by walking through screens
- Ensure transitions between screens make sense
- Check that all user actions have appropriate screens
- Verify error handling is clear
- Ensure empty states are helpful

**Design Principles**:
- **Narrow**: Focus on one complete journey
- **Deep**: Complete end-to-end value
- **Polished**: Works well, not perfect

### 5. Ensure All Screens Are Created

Verify that all screens referenced in your PRD are created.

**Verification Process**:
1. Review PRD User Journeys section
2. Check Functional Requirements section
3. Review Acceptance Criteria for screen references
4. Verify all screens mentioned are created
5. Add any missing screens

**Screen Checklist**:
- [ ] Authentication screens (login, signup, forgot password)
- [ ] Primary user journey screens
- [ ] Secondary user journey screens
- [ ] Dashboard/home screen
- [ ] Error state screens
- [ ] Empty state screens
- [ ] AI interaction screens (if applicable)
- [ ] All screens referenced in PRD

### 6. Export All Mockups to PNG

Export all mockups to PNG format when satisfied with the design.

**Export Process**:
1. Review all flows and screens
2. Ensure all screens are finalized
3. Export each screen to PNG format
4. Organize PNG files logically
5. Name files descriptively

**File Organization**:
- Use descriptive file names (e.g., "01-login.png", "02-dashboard.png")
- Organize files by flow (e.g., "auth-login.png", "auth-signup.png")
- Keep files organized in a folder
- Ensure files are accessible for PRD and implementation

**Export Tips**:
- Export all screens even if they're similar
- Use consistent naming convention
- Keep file sizes reasonable (not too large)
- Ensure PNG quality is good for implementation

> 🎯 **Goal**: Create mockups that clearly communicate your vision. These will be used by Cursor to understand the UI structure during implementation.

## Apply It Now

**Task**: Create all mockups for your MVP

1. Review PRD and identify all user flows
2. Create user flows in UX Pilot
3. Generate screens for each step in flows
4. Iterate on mockups based on UX best practices
5. Ensure all screens referenced in PRD are created
6. Export all mockups to PNG format

**Artifacts**: You'll create:
- User flows in UX Pilot
- All screens for each flow
- PNG files for all screens
- Organized mockup files

## Artifacts

You'll create:
- UX Pilot flows and screens
- PNG mockup files for all screens
- Documentation of user flows

## Worked Example

**Situation**: Building a B2B AI SaaS retrospective tool

**Mockups Process**:
1. **Flow Identification**: Reviewed PRD and identified flows
   - Authentication flow (login, signup)
   - Primary journey (create session, submit feedback, view insights)
   - Dashboard flow
   - Error states

2. **Flow Creation**: Created flows in UX Pilot
   - "Authentication Flow"
   - "Primary User Journey"
   - "Dashboard Flow"
   - "Error States"

3. **Screen Generation**: Generated screens in UX Pilot
   - Authentication flow: Login screen, Signup screen, Forgot password screen
   - Primary journey: Create session screen, Submit feedback screen, View insights screen
   - Dashboard: Dashboard screen, Empty dashboard screen
   - Error states: Invalid login error, Network error

4. **Iteration**: Refined screens
   - Adjusted login screen layout
   - Improved dashboard design
   - Enhanced error messages
   - Ensured consistency across screens

5. **Verification**: Checked all PRD screens were created
   - All screens from PRD were present
   - Added missing empty state screen
   - Verified error states were covered

6. **Export**: Exported all screens to PNG
   - Created 10 PNG files
   - Named files descriptively (e.g., "01-login.png", "02-dashboard.png")
   - Organized files in "mockups" folder

**Time**: 3 hours total

## Checklist

Before proceeding to Setup, verify:
- [ ] User flows created in UX Pilot
- [ ] Screens generated for all key user journeys
- [ ] Mockups iterated on and refined
- [ ] All screens referenced in PRD are created
- [ ] Complete user journey designed
- [ ] All mockups exported to PNG format
- [ ] PNG files organized and accessible
- [ ] Mockups ready for implementation planning

## Self-Assessment

1. **Where do you design the complete user journey?**
   - [ ] During implementation
   - [ ] In the Setup chapter
   - [ ] In UX Pilot during Planning ✓
   - [ ] After deployment

2. **What should you export mockups as?**
   - [ ] PDF files
   - [ ] PNG files ✓
   - [ ] JPG files
   - [ ] Vector files

3. **What should you ensure before exporting mockups?** (Select all)
   - [ ] All screens referenced in PRD are created ✓
   - [ ] Error states are designed ✓
   - [ ] Empty states are designed ✓
   - [ ] All future features are designed

## Exit Criteria

You're ready to proceed to Setup when:
- [ ] All user flows are created in UX Pilot
- [ ] All screens are generated and refined
- [ ] All screens referenced in PRD are created
- [ ] Complete user journey is designed
- [ ] All mockups are exported to PNG format
- [ ] PNG files are organized and accessible
- [ ] Mockups are ready for implementation planning

## Dependencies & Next Steps

### Prerequisites Completed
- [05 — Planning: PRD & AI Baseline](05-planning-prd.md) - Complete PRD with user journeys defined

### Next Steps
- Proceed to [06 — Setup](06-setup.md) to set up development environment and create implementation plan

### What This Enables

Completing mockups enables:
- Visual reference for implementation
- Clear communication of vision to Cursor
- Better UI code generation during implementation
- Structured approach to building features

### Related Resources

- [05 — Planning](05-planning.md) - Return to Planning overview
- [PRD Template](05-setup-prd-template.md) - Reference for PRD structure

---

> 💡 **Tip**: Don't skip mockups. They help Cursor understand your vision and generate better UI code during implementation.
> 📝 **Note**: The journey design happens here in Planning using UX Pilot. Implementation will follow in later chapters.
> ⚠️ **Warning**: Don't rush mockups. Clear mockups lead to better implementation and fewer iterations during development.

