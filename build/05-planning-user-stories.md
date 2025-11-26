# 05 — Planning: User Stories

**Purpose**: Generate and refine user stories that define your MVP's core functionality

**Outcome**: Have a prioritized list of user stories that align with your MVP scope and guide PRD creation

**Audience**: PM / Dev / Both

**Time**: 30-60 minutes

**Prerequisites**: [Decide What to Build](/broken/pages/rz5te4UitE8m4DNQogZJ) - Decision to build, key problems identified, innovation aspects defined

## Learning Outcomes

By the end of this chapter, you will be able to:

1. Use AI tools to generate initial user stories from problem statements
2. Refine and iterate on user stories with AI assistance
3. Prioritize user stories based on MVP scope
4. Ensure user stories are specific, measurable, and aligned with value proposition
5. Finalize a comprehensive user stories list ready for PRD creation

## Jobs-to-Be-Done

* **When**: I have identified key problems and innovation aspects, and need to define what users will do
* **I want**: To generate user stories that capture user needs and MVP functionality
* **So that**: I have a clear foundation for creating the PRD and understanding the MVP scope

## Inputs

* Decision to build from [06 — Synthesize Insights → Decision](../decide/06-synthesize-insights-decision.md)
* Key problems identified and innovation aspects defined
* Understanding of target users and value proposition
* Access to AI tools (ChatGPT, Claude, or Cursor)

## Activities

### 1. Prepare Context for AI

Before generating user stories, gather the information you'll provide to AI:

**What You Need**:

* Product idea and target users
* Key problems your product solves
* Innovation aspects that differentiate your solution
* MVP scope boundaries (what's in vs. out)

**Context to Provide**:

* Brief product description
* Target user personas or user types
* Core problems being solved
* Key innovation aspects (what makes your solution unique)
* MVP constraints or scope boundaries

### 2. Generate Initial User Stories

Use AI tools (ChatGPT, Claude, or Cursor) to generate an initial set of user stories based on your key problems and innovation aspects.

**Process**:

1. Open your AI tool (ChatGPT, Claude, or Cursor)
2. Provide context about your product idea, target users, and key problems
3. Request generation of user stories in the format: "As a \[user type], I want \[action] so that \[benefit]"
4. Specify the number of stories needed (typically 10-15 for MVP)
5. Request prioritization of core functionality

**Example Prompt**:

```
I'm building a B2B AI SaaS product that helps [target users] solve [problem]. 
Key innovation aspects: [aspect 1], [aspect 2], [aspect 3].

Generate 10-15 user stories for the MVP, prioritizing core functionality.
Format each story as: "As a [user type], I want [action] so that [benefit]"
```

### 3. Review Generated Stories

**Review Criteria**:

* Are stories specific and actionable?
* Do they align with your MVP scope?
* Do they address the core problems identified?
* Are they measurable (can you verify completion)?
* Do they reflect your innovation aspects?

**Common Issues to Watch For**:

* Vague or generic stories
* Stories that are too large (epics instead of stories)
* Stories outside MVP scope
* Missing core functionality
* Stories that don't connect to user benefits

### 4. Iterate and Refine

Use AI to refine and improve your user stories.

**Refinement Process**:

1. Share the generated stories with AI
2. Request specific improvements:
   * Merge similar stories
   * Split large stories into smaller ones
   * Add missing core functionality
   * Remove stories outside MVP scope
   * Make stories more specific
3. Review the refined stories
4. Repeat until satisfied

**Example Refinement Prompt**:

```
Here are my user stories: [list stories]

Please:
1. Merge any similar stories
2. Split any stories that are too large
3. Ensure all stories are specific and measurable
4. Remove any stories outside MVP scope
5. Add any missing core functionality
```

> 💡 **Tip**: Iterate on user stories with AI. Ask for refinements, merge similar stories, and ensure they're specific and measurable.

### 5. Prioritize User Stories

Organize your user stories by priority for MVP implementation.

**Prioritization Criteria**:

* **Must Have**: Core functionality without which the product doesn't work
* **Should Have**: Important functionality that significantly improves value
* **Could Have**: Nice-to-have features that can wait for later releases

**Prioritization Process**:

1. Review all user stories
2. Categorize each story (Must Have / Should Have / Could Have)
3. Within each category, order by implementation dependency
4. Focus MVP on "Must Have" stories
5. Document "Should Have" and "Could Have" for future releases

### 6. Finalize User Stories List

**Final Review Checklist**:

* [ ] All user stories are specific and measurable
* [ ] Stories align with MVP scope
* [ ] Core functionality is covered
* [ ] Stories are prioritized
* [ ] Stories are documented and ready for PRD creation

**Documentation Format**:

* List format with priority indicators
* Grouped by functional area (optional)
* Include acceptance criteria hints (what "done" looks like)

## Apply It Now

**Task**: Generate and finalize user stories for your MVP

1. Prepare context about your product, users, and problems
2. Use AI to generate initial user stories (10-15 stories)
3. Review generated stories for quality and alignment
4. Iterate with AI to refine stories
5. Prioritize stories for MVP scope
6. Finalize and document your user stories list

**Artifacts**: You'll create:

* Initial user stories (AI-generated)
* Refined and prioritized user stories list
* Documentation of MVP scope boundaries

## Artifacts

You'll create:

* User stories list (prioritized)
* MVP scope documentation
* Notes on user story decisions and rationale

## Worked Example

**Situation**: Building a B2B AI SaaS retrospective tool

**User Stories Process**:

1. **Context Provided**:
   * Product: AI-powered retrospective tool for teams
   * Users: Team leads, project managers
   * Problems: Time-consuming retrospectives, lack of insights
   * Innovation: AI generates actionable insights automatically
2. **AI Generation**: Used Claude to generate 12 initial user stories
   * "As a team lead, I want to create a retrospective session so that I can collect team feedback"
   * "As a team member, I want to submit feedback anonymously so that I feel safe sharing honest opinions"
   * "As a team lead, I want AI to generate insights from feedback so that I save time on analysis"
3. **Refinement**: Iterated 3 times with AI
   * Merged 2 similar feedback submission stories
   * Split "manage retrospective" into separate stories
   * Added missing authentication story
   * Removed "export to PDF" (outside MVP)
4. **Prioritization**:
   * Must Have: 8 core stories (auth, create session, submit feedback, AI insights)
   * Should Have: 3 stories (dashboard, history, notifications)
   * Could Have: 1 story (custom templates)
5. **Finalization**: Documented 8 core MVP stories, saved 4 for future releases

**Time**: 45 minutes total

## Checklist

Before proceeding to PRD creation, verify:

* [ ] User stories generated using AI tools (ChatGPT, Claude, or Cursor)
* [ ] User stories reviewed and iterated on
* [ ] User stories finalized and prioritized
* [ ] User stories align with MVP scope
* [ ] All core functionality is covered in user stories
* [ ] User stories are specific and measurable
* [ ] User stories list is documented

## Self-Assessment

1. **What format should user stories follow?**
   * [ ] "I need \[feature]"
   * [ ] "As a \[user type], I want \[action] so that \[benefit]" ✓
   * [ ] "The system should \[action]"
   * [ ] "Users can \[action]"
2. **How many user stories should you generate for MVP?**
   * [ ] 3-5 stories
   * [ ] 10-15 stories ✓
   * [ ] 20-30 stories
   * [ ] As many as possible
3. **What should you do after generating initial user stories?**
   * [ ] Use them immediately in PRD
   * [ ] Review, refine, and prioritize them ✓
   * [ ] Start building features
   * [ ] Skip to mockups

## Exit Criteria

You're ready to proceed to PRD creation when:

* [ ] User stories are generated and documented
* [ ] User stories are refined and aligned with MVP scope
* [ ] User stories are prioritized (Must Have / Should Have / Could Have)
* [ ] All core functionality is covered in user stories
* [ ] User stories list is finalized and ready for PRD creation

## Dependencies & Next Steps

### Prerequisites Completed

* [Decide What to Build](/broken/pages/rz5te4UitE8m4DNQogZJ) - Decision to build, key problems identified, innovation aspects defined

### Next Steps

* Proceed to [05 — Planning: PRD & AI Baseline](05-planning-prd.md) to create your Product Requirements Document based on these user stories

### What This Enables

Completing user stories enables:

* Clear foundation for PRD creation
* Better understanding of MVP scope
* Structured approach to defining functionality
* Alignment between problems and solutions

### Related Resources

* [05 — Planning](05-planning.md) - Return to Planning overview

***

> 💡 **Tip**: Don't rush user stories. Well-defined stories lead to better PRDs and clearer implementation plans. 📝 **Note**: User stories are the foundation of your PRD. Spend time getting them right.
