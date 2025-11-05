# 05 — Planning

**Purpose**: Create a comprehensive plan for your MVP including user stories, PRD, visual mockups, and AI Baseline design

**Outcome**: Have a complete plan (user stories, PRD, mockups, AI Baseline design) that guides implementation

**Audience**: PM / Dev / Both

**Time**: 1-2 days

**Prerequisites**: [Decide What to Build](decide/index.md) - Decision to build, key problems identified, innovation aspects defined

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Generate and refine user stories using AI tools
2. Create a comprehensive PRD using AI tools
3. Design complete user journeys and create visual mockups using UX Pilot
4. Plan AI Baseline integration including service selection, model choice, and prompt design
5. Export mockups ready for implementation planning

## Jobs-to-Be-Done

- **When**: I have a decision to build and need to create a detailed plan
- **I want**: To generate user stories, create a PRD, design visual mockups, and plan AI Baseline integration
- **So that**: I have a clear blueprint that guides implementation including AI components

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

### 4. Plan AI Baseline Integration

If your MVP includes AI functionality, plan the AI Baseline integration during the Planning phase. This ensures AI components are designed alongside the rest of your product architecture.

**Process**:
1. **Select AI Service**: Choose your AI provider
   - **OpenAI**: GPT models, embeddings
   - **Anthropic**: Claude models (recommended for this stack)
   - **Custom**: Build your own (not recommended for MVP)
2. **Choose Model**: Select appropriate model for MVP
   - **Claude 3.5 Sonnet**: Best quality, balanced cost
   - **Claude 3 Haiku**: Fast responses, lower cost
   - **GPT-4**: Alternative option
   - **GPT-3.5**: Lower cost option
3. **Design AI Integration**: Define AI features and integration points
   - What will AI do in your product?
   - What inputs does it need?
   - What outputs does it produce?
   - How will users interact with AI features?
   - Where in the user journey does AI add value?
4. **Design Prompt Templates**: Create prompt structures for AI interactions
   - System prompts that define AI behavior
   - User prompt templates
   - Response formatting requirements
   - Error handling and fallbacks
5. **Document API Requirements**: Define technical requirements
   - API keys and authentication
   - Rate limiting considerations
   - Error handling strategy
   - Response processing requirements
6. **Include in PRD**: Ensure AI Baseline is documented in your PRD
   - AI features in Functional Requirements
   - AI integration points in User Journeys
   - Acceptance criteria for AI features
   - Technical requirements for AI integration

**Example** (Retrospective Tool):
- **AI Service**: Anthropic Claude 3.5 Sonnet
- **Use Case**: Generate insights from retrospective feedback
- **Input**: User feedback from retrospective session
- **Output**: Structured insights with themes, action items, and recognition points
- **Integration Point**: After user submits feedback, AI generates insights
- **Prompt Design**: System prompt defines retrospective facilitator role, user prompt includes feedback data

**Example Prompt Structure**:
```
System: You are a retrospective facilitator. Analyze feedback and provide structured insights.
User: [Retrospective feedback data]
Output Format: JSON with themes, action items, recognition
```

> 💡 **Tip**: Start simple with AI. You can enhance AI features later. Focus on core value delivery first.
> 📝 **Note**: AI Baseline planning happens here in Planning. Implementation will follow in Build Features where Cursor will build the AI components as part of the comprehensive plan.
> ⚠️ **Warning**: Don't skip AI planning if your product relies on AI. Proper planning ensures AI integration aligns with your product vision.

## Apply It Now

**Task**: Complete planning for your MVP

1. Generate user stories using AI tools (ChatGPT, Claude, or Cursor)
2. Iterate and finalize user stories
3. Generate comprehensive PRD using AI tools
4. Review and refine PRD
5. Create user flows and screens in UX Pilot
6. Iterate on mockups
7. Export all mockups to PNG
8. Plan AI Baseline integration (if applicable)
9. Document AI service, model, and prompt design

**Artifacts**: You'll create:
- Finalized user stories list
- Comprehensive PRD document
- UX Pilot mockups (PNG files for all screens)
- AI Baseline plan/design (if applicable)

## Artifacts

You'll create:
- User stories list (prioritized)
- Product Requirements Document (PRD)
- UX mockups (PNG files for all screens)
- AI Baseline plan/design (if applicable)

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
4. **AI Baseline Planning**: Planned AI integration
   - Selected Anthropic Claude 3.5 Sonnet
   - Designed prompt templates for insights generation
   - Documented AI features in PRD
   - Defined integration points in user journeys

**Time**: Planning took 1.5 days total

## Checklist

Before proceeding to the next chapter, verify:
- [ ] User stories generated and finalized
- [ ] PRD created and reviewed
- [ ] UX mockups created in UX Pilot
- [ ] All mockups exported to PNG
- [ ] Complete user journey designed and documented
- [ ] AI Baseline planned and designed (if applicable)

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
- [ ] AI Baseline planning is complete (if applicable)

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

