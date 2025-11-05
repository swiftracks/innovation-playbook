# 05 — Planning

**Purpose**: Create a comprehensive plan for your MVP including user stories, PRD, and visual mockups

**Outcome**: Have a complete plan (user stories, PRD, mockups) that guides implementation

**Audience**: PM / Dev / Both

**Time**: 1-2 days

**Prerequisites**: [Decide What to Build](decide/index.md) - Decision to build, key problems identified, innovation aspects defined

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Generate and refine user stories using AI tools
2. Create a comprehensive PRD using AI tools
3. Design complete user journeys and create visual mockups using UX Pilot
4. Export mockups ready for implementation planning

## Jobs-to-Be-Done

- **When**: I have a decision to build and need to create a detailed plan
- **I want**: To generate user stories, create a PRD, and design visual mockups
- **So that**: I have a clear blueprint that guides implementation

## Inputs

- Decision to build from [06 — Synthesize Insights → Decision](decide/06-synthesize-insights-decision.md)
- Key problems identified and innovation aspects defined
- Understanding of target users and value proposition
- Access to AI tools (ChatGPT, Claude, or Cursor)
- Access to UX Pilot for mockup generation

## Activities

### 1. Generate User Stories

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

### 2. Generate Product Requirements Document (PRD)

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

### 3. Design User Flows and Screens

Use UX Pilot to create visual mockups of your application. This is where you **design the complete user journey** that will be implemented later.

**Process**:
1. Review your PRD and identify key user flows
2. In UX Pilot, create flows for each major user journey
3. Generate screens for each step in the flows
4. Iterate on mockups based on UX best practices
5. Ensure all screens referenced in PRD are created
6. Export all mockups to PNG format when satisfied

**Key Flows to Design**:
- Authentication flow (signup/login)
- Primary user journey (core value delivery)
- Secondary user journeys
- Error and edge case states

**Design Principles**:
- **Narrow**: Focus on one complete journey
- **Deep**: Complete end-to-end value
- **Polished**: Works well, not perfect

> 🎯 **Goal**: Create mockups that clearly communicate your vision. These will be used by Cursor to understand the UI structure during implementation.

## Apply It Now

**Task**: Complete planning for your MVP

1. Generate user stories using AI tools (ChatGPT, Claude, or Cursor)
2. Iterate and finalize user stories
3. Generate comprehensive PRD using AI tools
4. Review and refine PRD
5. Create user flows and screens in UX Pilot
6. Iterate on mockups
7. Export all mockups to PNG

**Artifacts**: You'll create:
- Finalized user stories list
- Comprehensive PRD document
- UX Pilot mockups (PNG files for all screens)

## Artifacts

You'll create:
- User stories list (prioritized)
- Product Requirements Document (PRD)
- UX mockups (PNG files for all screens)

## Worked Example

**Situation**: Planning for a B2B AI SaaS MVP

**Planning Process**:
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

**Time**: Planning took 1.5 days total

## Checklist

Before proceeding to the next chapter, verify:
- [ ] User stories generated and finalized
- [ ] PRD created and reviewed
- [ ] UX mockups created in UX Pilot
- [ ] All mockups exported to PNG
- [ ] Complete user journey designed and documented

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

3. **Where do you design the complete user journey?**
   - [ ] During implementation
   - [ ] In the Setup chapter
   - [ ] In UX Pilot during Planning ✓
   - [ ] After deployment

## Exit Criteria

You're ready to proceed when:
- [ ] User stories are finalized
- [ ] PRD is complete and reviewed
- [ ] All mockups are created and exported
- [ ] Complete user journey is designed and documented

## Dependencies & Next Steps

### Prerequisites Completed
- [Decide What to Build](decide/index.md) - Decision to build, key problems identified, innovation aspects defined

### Next Steps
- Proceed to [06 — Setup](06-setup.md) to set up development environment and create implementation plan

### What This Enables

Completing planning enables:
- Clear direction from PRD and user stories
- Visual reference from mockups
- Structured approach to implementation
- Better understanding of scope and requirements

### Related Resources

- [PRD Template](05-setup-prd-template.md) - Template for creating your PRD

---

> 💡 **Tip**: Don't rush the planning phase. A solid PRD and mockups will save significant time during development.
> 📝 **Note**: The journey design happens here in Planning using UX Pilot. Implementation will follow in later chapters.
> ⚠️ **Warning**: Don't skip mockups. They help Cursor understand your vision and generate better UI code during implementation.

