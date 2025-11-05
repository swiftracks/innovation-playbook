# 05 — Planning: PRD & AI Baseline

**Purpose**: Create a comprehensive Product Requirements Document (PRD) and plan AI Baseline integration for your MVP

**Outcome**: Have a complete PRD that guides implementation and a well-planned AI Baseline integration (if applicable)

**Audience**: PM / Dev / Both

**Time**: 2-4 hours

**Prerequisites**: [05 — Planning: User Stories](05-planning-user-stories.md) - Finalized and prioritized user stories

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Use AI tools to generate a comprehensive PRD from user stories
2. Review and refine PRD sections with AI assistance
3. Ensure all PRD sections are complete and clear
4. Plan AI Baseline integration including service selection, model choice, and prompt design
5. Document AI features and integration points in the PRD

## Jobs-to-Be-Done

- **When**: I have finalized user stories and need to create a detailed PRD
- **I want**: To generate a comprehensive PRD and plan AI Baseline integration
- **So that**: I have a clear blueprint that guides implementation including AI components

## Inputs

- Finalized user stories from [05 — Planning: User Stories](05-planning-user-stories.md)
- Product context and value proposition
- Understanding of target users and problems
- Access to AI tools (ChatGPT, Claude, or Cursor)
- [PRD Template](05-setup-prd-template.md) for reference

## Activities

### 1. Prepare Materials for PRD Generation

Before generating the PRD, gather everything you'll provide to AI:

**What You Need**:
- Finalized and prioritized user stories
- Product description and value proposition
- Target user personas
- Key problems being solved
- Innovation aspects
- MVP scope boundaries

**Context to Provide**:
- Complete list of user stories
- Product vision and purpose
- Target users and personas
- Core problems and solutions
- MVP scope (in-scope vs. out-of-scope)

### 2. Generate Product Requirements Document (PRD)

Use AI tools to generate a comprehensive PRD based on your finalized user stories.

**Process**:
1. Open your AI tool (ChatGPT, Claude, or Cursor)
2. Provide your finalized user stories and product context
3. Reference the [PRD Template](05-setup-prd-template.md) structure
4. Request generation of a PRD following the template structure
5. Specify that all sections should be complete and clear
6. Request specific acceptance criteria for each feature

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

Include:
- Purpose & Vision
- Scope (Release 1) with in-scope and out-of-scope features
- Key Personas
- User Journeys for each major flow
- Functional Requirements with acceptance criteria
- Non-Functional Requirements
- Information Architecture & Data Model
- UX References (mockups will be added later)
- Acceptance Criteria for each feature
- Analytics & Success Metrics
- Content & States (empty states, error states)
- Accessibility & Design System requirements
- Security, Privacy, Compliance requirements
- Glossary of key terms

Make sure all sections are complete and clear.
```

### 3. Review and Refine PRD

**Review Process**:
1. Review the generated PRD section by section
2. Check for completeness and clarity
3. Verify alignment with user stories
4. Ensure acceptance criteria are specific and measurable
5. Refine sections that need improvement

**Refinement Process**:
1. Identify sections that need improvement
2. Use AI to refine specific sections
3. Add missing details or requirements
4. Ensure consistency across sections
5. Verify all user stories are addressed

**Example Refinement Prompt**:
```
Here's my PRD: [PRD content]

Please:
1. Review the Functional Requirements section
2. Ensure all user stories are addressed
3. Add missing acceptance criteria
4. Make acceptance criteria more specific and measurable
5. Ensure consistency with User Journeys section
```

> 📝 **Note**: The PRD serves as the blueprint for your MVP. Spend time getting it right - it will guide all implementation decisions.

### 4. Plan AI Baseline Integration

If your MVP includes AI functionality, plan the AI Baseline integration during the Planning phase. This ensures AI components are designed alongside the rest of your product architecture.

**Process**:

#### Step 1: Select AI Service

Choose your AI provider:

- **OpenAI**: GPT models, embeddings
- **Anthropic**: Claude models (recommended for this stack)
- **Custom**: Build your own (not recommended for MVP)

**Selection Criteria**:
- Quality of responses for your use case
- Cost considerations
- API reliability and rate limits
- Integration complexity

#### Step 2: Choose Model

Select appropriate model for MVP:

- **Claude 3.5 Sonnet**: Best quality, balanced cost
- **Claude 3 Haiku**: Fast responses, lower cost
- **GPT-4**: Alternative option
- **GPT-3.5**: Lower cost option

**Model Selection Criteria**:
- Required response quality
- Response speed needs
- Cost constraints
- Token limits for your use case

#### Step 3: Design AI Integration

Define AI features and integration points:

**Questions to Answer**:
- What will AI do in your product?
- What inputs does it need?
- What outputs does it produce?
- How will users interact with AI features?
- Where in the user journey does AI add value?

**Integration Points to Define**:
- Where AI is triggered (user action, background process, scheduled)
- What data flows to AI (user input, context, history)
- What AI produces (responses, insights, recommendations)
- How users see AI output (inline, modal, notification)

#### Step 4: Design Prompt Templates

Create prompt structures for AI interactions:

**System Prompts**:
- Define AI behavior and role
- Set context and constraints
- Specify output format requirements
- Define error handling approach

**User Prompt Templates**:
- Structure user input for AI
- Include necessary context
- Format data for AI processing
- Handle variable inputs

**Response Formatting**:
- Define expected output structure
- Specify JSON or text format
- Define parsing requirements
- Handle edge cases

**Error Handling and Fallbacks**:
- What happens if AI fails?
- Fallback mechanisms
- User-friendly error messages
- Retry strategies

#### Step 5: Document API Requirements

Define technical requirements:

**API Configuration**:
- API keys and authentication
- Rate limiting considerations
- Error handling strategy
- Response processing requirements
- Token usage and limits

**Integration Requirements**:
- Where API calls are made (frontend, backend, functions)
- Data flow and processing
- Caching strategies
- Security considerations

#### Step 6: Include AI in PRD

Ensure AI Baseline is documented in your PRD:

**PRD Sections to Update**:
- **Functional Requirements**: Add AI features with acceptance criteria
- **User Journeys**: Include AI integration points in flows
- **Acceptance Criteria**: Define criteria for AI features
- **Technical Requirements**: Document AI integration requirements
- **Data Model**: Include AI-related data structures

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

### 5. Finalize PRD

**Final Review Checklist**:
- [ ] All PRD sections are complete
- [ ] User stories are addressed in Functional Requirements
- [ ] Acceptance criteria are specific and measurable
- [ ] User Journeys are complete and include AI integration points (if applicable)
- [ ] AI Baseline planning is documented (if applicable)
- [ ] PRD is ready for mockup creation and implementation

**Documentation Format**:
- Use the PRD template structure
- Save as a markdown or document file
- Include all sections
- Ensure formatting is clear

> 💡 **Tip**: Start simple with AI. You can enhance AI features later. Focus on core value delivery first.
> 📝 **Note**: AI Baseline planning happens here in Planning. Implementation will follow in Build Features where Cursor will build the AI components as part of the comprehensive plan.
> ⚠️ **Warning**: Don't skip AI planning if your product relies on AI. Proper planning ensures AI integration aligns with your product vision.

## Apply It Now

**Task**: Create your PRD and plan AI Baseline integration

1. Prepare user stories and product context
2. Use AI to generate comprehensive PRD following the template structure
3. Review and refine PRD sections
4. Plan AI Baseline integration (if applicable):
   - Select AI service and model
   - Design AI integration points
   - Design prompt templates
   - Document API requirements
5. Include AI features in PRD (if applicable)
6. Finalize PRD document

**Artifacts**: You'll create:
- Comprehensive PRD document
- AI Baseline plan/design (if applicable)
- Documentation of AI integration points

## Artifacts

You'll create:
- Product Requirements Document (PRD)
- AI Baseline plan/design (if applicable)
- Documentation of AI service, model, and prompt design

## Worked Example

**Situation**: Building a B2B AI SaaS retrospective tool

**PRD Process**:
1. **Preparation**: Gathered 8 finalized user stories, product context, and personas

2. **PRD Generation**: Used Claude to generate comprehensive PRD
   - Provided user stories and PRD template structure
   - Generated all sections: purpose, scope, personas, journeys, requirements
   - Included acceptance criteria for each feature
   - Reviewed and refined with AI assistance

3. **AI Baseline Planning**: Planned AI integration
   - **AI Service**: Selected Anthropic Claude 3.5 Sonnet
   - **Use Case**: Generate insights from retrospective feedback
   - **Integration**: After user submits feedback, AI generates insights
   - **Prompt Design**: System prompt defines retrospective facilitator role
   - **Output**: JSON with themes, action items, recognition points

4. **PRD Integration**: Added AI features to PRD
   - Added AI features to Functional Requirements
   - Included AI integration points in User Journeys
   - Defined acceptance criteria for AI features
   - Documented technical requirements for AI integration

5. **Finalization**: Reviewed complete PRD, ensured all sections complete

**Time**: 3 hours total (2 hours PRD, 1 hour AI Baseline planning)

## Checklist

Before proceeding to mockup creation, verify:
- [ ] PRD generated using AI tools
- [ ] PRD reviewed and refined
- [ ] All PRD sections completed (Purpose, Scope, Personas, User Journeys, Requirements, etc.)
- [ ] PRD includes acceptance criteria for each feature
- [ ] PRD finalized and ready for implementation
- [ ] AI Baseline planned and designed (if applicable)
- [ ] AI features documented in PRD (if applicable)
- [ ] AI integration points defined in User Journeys (if applicable)

## Self-Assessment

1. **What should be included in your PRD?** (Select all)
   - [ ] Purpose & Vision ✓
   - [ ] Functional Requirements ✓
   - [ ] User Journeys ✓
   - [ ] Complete product design for all future releases

2. **When should you plan AI Baseline integration?**
   - [ ] During implementation
   - [ ] During Planning phase ✓
   - [ ] After deployment
   - [ ] Only if needed

3. **What should AI Baseline planning include?** (Select all)
   - [ ] AI service and model selection ✓
   - [ ] Prompt design ✓
   - [ ] Integration points in user journey ✓
   - [ ] Implementation code

## Exit Criteria

You're ready to proceed to mockup creation when:
- [ ] PRD is complete and reviewed
- [ ] All PRD sections are filled out
- [ ] Acceptance criteria are defined for each feature
- [ ] AI Baseline planning is complete (if applicable)
- [ ] AI features are documented in PRD (if applicable)
- [ ] PRD is ready for mockup creation and implementation

## Dependencies & Next Steps

### Prerequisites Completed
- [05 — Planning: User Stories](05-planning-user-stories.md) - Finalized and prioritized user stories

### Next Steps
- Proceed to [05 — Planning: Mockups](05-planning-mockups.md) to create visual mockups based on your PRD

### What This Enables

Completing PRD and AI Baseline planning enables:
- Clear blueprint for implementation
- Structured approach to building
- Well-planned AI integration
- Better understanding of scope and requirements

### Related Resources

- [PRD Template](05-setup-prd-template.md) - Template for creating your PRD
- [05 — Planning](05-planning.md) - Return to Planning overview

---

> 💡 **Tip**: Don't rush the PRD phase. A solid PRD will save significant time during development.
> 📝 **Note**: The PRD serves as the blueprint for your MVP. Spend time getting it right.
> ⚠️ **Warning**: Don't skip AI planning if your product relies on AI. Proper planning ensures AI integration aligns with your product vision.

