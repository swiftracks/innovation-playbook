# Getting Started

**Purpose**: A practical, outcome-focused guide for product innovation teams

**Version**: 1.0.0

**Audience**: Product Managers, Developers, and Innovation Teams

## Welcome

This guide helps you systematically validate ideas, build MVPs, and launch products that deliver real value. Every chapter is designed for action—you'll create real artifacts, not just read concepts.

## Choose Your Path

**Where are you in your innovation journey?**

### 🎯 Validating an Idea? → Start with "Decide What to Build"

**Why validation matters**: Most product failures happen because we build something nobody wants. The Decide section helps you validate your idea **before** investing time and resources in building.

**What you'll do**: Use **Swift CNS** (an AI-powered validation platform) to systematically test your assumptions through experiments, document learnings, and make data-driven go/no-go decisions.

**Time commitment**: 2-4 weeks for thorough validation

**Prerequisites**: 
- Swift CNS account at [app.swiftcns.ai](https://app.swiftcns.ai)
- Initial idea or problem hypothesis
- Access to potential users for experiments

**Start here**: [Decide What to Build](decide/index.md)

> 💡 **Tip**: Even if you're eager to build, spending 2-4 weeks validating can save months of wasted effort. The Decide section uses Swift CNS to make validation systematic and efficient.

### 🏗️ Ready to Build? → Start with "Build the MVP"

**When to use**: You have a validated idea (completed Decide section) or you're building something with clear requirements.

**What you'll do**: Plan your MVP, set up development tools (Cursor IDE), build features collaboratively with AI assistance, and deploy to Firebase.

**Time commitment**: 4-8 weeks depending on complexity

**Prerequisites**:
- Validated hypothesis or clear requirements
- Cursor IDE installed
- Firebase account

**Start here**: [Build the MVP](build/index.md)

### 🚀 Have an MVP? → Start with "Launch & Iterate"

**When to use**: You have a working MVP and need to get it in front of users, gather feedback, and iterate.

**What you'll do**: Prepare your ICP, develop messaging and channel strategies, build your website, launch private beta, run experiments, and synthesize insights.

**Time commitment**: Ongoing iteration cycles

**Prerequisites**:
- Working MVP
- Deployment infrastructure ready

**Start here**: [Launch & Iterate](launch/index.md)

## Guide Structure

This guide follows a three-phase journey:

```
Decide What to Build (Swift CNS)
    ├─ 01 — Idea / Problem
    ├─ 02 — Identify Critical Assumptions
    ├─ 03 — Form Testable Hypotheses
    ├─ 04 — Design & Run Experiments
    ├─ 05 — Extract Key Learnings
    └─ 06 — Synthesize Insights → Decision
    ↓
Build the MVP (Cursor, UX Pilot, Firebase)
    ├─ 05 — Planning
    ├─ 06 — Setup
    ├─ 08 — Build Features
    └─ 09 — Deploy
    ↓
Launch & Iterate (Swift CNS)
    ├─ 01 — Prepare ICP
    ├─ 02 — Develop Messaging Strategy
    ├─ 03 — Design Channel Strategy
    ├─ 04 — Build Website V1
    ├─ 05 — Setup Tool Stack
    ├─ 06 — Launch Private Beta
    ├─ 07 — Run Experiments
    ├─ 08 — Synthesize Insights
    └─ 09 — Exit to Public Beta
```

See the [Dependency Map](dependency-map.md) for detailed chapter relationships and learning paths.

## Understanding the DECIDE Section

**Why validation before building is critical:**

Most teams jump straight to building, only to discover later that:
- Users don't actually have the problem you thought they had
- The solution doesn't fit their workflow
- They won't pay for it
- The market isn't ready

The **Decide What to Build** section uses **Swift CNS** to help you avoid these pitfalls by:

1. **Articulating the problem clearly** - Use Swift CNS chat to refine your idea and value proposition
2. **Identifying critical assumptions** - Swift CNS AI helps you find what must be true for success
3. **Forming testable hypotheses** - Convert assumptions into measurable statements
4. **Designing experiments** - Create structured tests to validate your hypotheses
5. **Extracting learnings** - Document insights in Swift CNS Learning Cards
6. **Making decisions** - Use Swift CNS Insights to synthesize everything into a go/no-go decision

**The Swift CNS Workflow:**

1. **Start New Chat** - Begin AI-guided conversation about your idea in Swift CNS
2. **Idea Analysis** - Swift CNS AI analyzes your idea and asks clarifying questions
3. **Assumptions Mapping** - AI helps identify critical assumptions that must be true
4. **Experiment Design** - AI guides you to create structured experiments
5. **Learning Cards** - Document insights and learnings from experiments in Swift CNS
6. **Insights** - View aggregated insights in Swift CNS to make go/no-go decisions

All validation work happens within Swift CNS, providing a systematic, AI-guided approach to decision-making.

> ⚠️ **Important**: The Decide chapters (01-06) must be done sequentially. Each builds on the previous one. Swift CNS AI guides you through the entire process.

**Ready to validate?** Set up Swift CNS and start: [Decide What to Build](decide/index.md)

## Tool Prerequisites

You don't need all tools upfront. Set them up as you reach each section. Detailed setup instructions are provided in the relevant chapters.

### For "Decide What to Build" Section

**Swift CNS** - AI-powered validation platform
- **What it's used for**: AI-guided validation, creating experiments, documenting learnings in Learning Cards, synthesizing insights for decisions
- **Access**: [app.swiftcns.ai](https://app.swiftcns.ai)
- **Used in**: All Decide chapters (01-06)
- **Prerequisites**: Google account for sign-in, initial idea or problem hypothesis
- **Quick setup**:
  1. Visit [app.swiftcns.ai](https://app.swiftcns.ai)
  2. Sign in with your Google account
  3. Create a new project (or select existing)
  4. Start a new chat to begin validation
- **When**: Set up before starting Decide section

> 💡 **Tip**: All validation work happens within Swift CNS. You'll use chat, experiments, learning cards, and insights features throughout the Decide section.

### For "Build the MVP" Section

**UX Pilot** - Mockup generation tool
- **What it's used for**: Generating visual mockups of complete user journeys for MVP planning
- **Used in**: Planning chapter (05), specifically in the mockup design phase
- **Prerequisites**: User stories and PRD from earlier in Planning chapter
- **Setup**: Follow instructions in [05 — Planning: Design Mockups](build/05-planning-mockups.md)
- **When**: Set up during Planning chapter

**Cursor** - AI-powered IDE
- **What it's used for**: AI-powered collaborative development, generating implementation plans, building features end-to-end, configuring development rules via `.cursorrules`
- **Access**: [cursor.sh](https://cursor.sh)
- **Used in**: Setup (06) and Build Features (08) chapters
- **Prerequisites**: Git repository (created in Setup chapter)
- **Quick setup**:
  1. Install Cursor IDE from [cursor.sh](https://cursor.sh)
  2. Follow [06 — Setup: Git & Cursor](build/06-setup-git-cursor.md) to clone your repository
  3. Configure `.cursorrules` as described in [06 — Setup: .cursorrules](build/06-setup-cursorrules.md)
  4. Use Cursor's plan mode to generate implementation plan in [06 — Setup: Implementation Planning](build/06-setup-implementation-planning.md)
- **When**: Set up during Setup chapter

> 💡 **Tip**: Cursor is your primary development tool for the Build section. You'll collaborate with Cursor AI throughout Setup and Build Features chapters.

**Firebase** - Backend infrastructure
- **What it's used for**: Hosting MVP application, authentication, Cloud Functions, production deployment
- **Access**: [firebase.google.com](https://firebase.google.com)
- **Used in**: Deploy chapter (09)
- **Prerequisites**: Google account, working MVP features ready for deployment, completed QA testing
- **Quick setup**:
  1. Sign up at [firebase.google.com](https://firebase.google.com)
  2. Create a new Firebase project
  3. Follow [09 — Deploy](build/09-deploy.md) for detailed setup instructions
  4. Configure Authentication, Hosting, and Functions as needed
- **When**: Set up during Deploy chapter

> 💡 **Tip**: Firebase setup happens during the Deploy chapter. You'll configure all services as part of the deployment process.

### For "Launch & Iterate" Section

**Swift CNS** - Also used for experiments and insights in Launch section
- **What it's used for**: Running experiments (outbound, growth marketing, product), synthesizing insights
- **Used in**: Run Experiments (07) and Synthesize Insights (08) chapters
- **Prerequisites**: Swift CNS account (same as Decide section)
- **When**: Use existing Swift CNS account from Decide section, or set up if starting directly with Launch

## Chapter Structure

Every chapter includes:

* **Learning Outcomes** - What you'll achieve
* **Jobs-to-Be-Done** - Context for when to use it
* **Inputs** - What you need before starting
* **Activities** - Step-by-step guidance
* **Apply It Now** - Interactive task
* **Artifacts** - What you'll create
* **Templates** - Reusable structures
* **Examples** - Worked examples
* **Checklist** - Quick reference
* **Self-Assessment** - Verify understanding

## Key Principles

This guide follows these core principles:

1. **Start with outcomes**: Every chapter defines measurable learning outcomes
2. **Architect the content**: Clear structure with dependency mapping
3. **Design for doing**: Templates, examples, checklists, and self-assessments
4. **Adopt a house style**: Consistent voice, glossary, and formatting
5. **Build interaction**: Quizzes, decision trees, and "Apply It Now" tasks

## What You'll Create

As you work through this guide, you'll produce:

* **Problem statements** and value propositions
* **Hypothesis canvases** and experiment plans
* **PRDs** and technical specifications
* **MVP architectures** and thin vertical implementations
* **Launch plans** and feedback loops

## Resources

* [Dependency Map](dependency-map.md) - Chapter relationships and learning paths
* [Glossary](glossary.md) - Key terms and definitions
* [Cadence](start-here/cadence.md) - Establishing work rhythms
* [Style Guide](/broken/pages/eQPCw2dkrAu2IfAAE7W1) - Voice, formatting, and callout standards

## Quick Reference

**Need to validate an idea?** → [Decide What to Build](decide/index.md)  
**Ready to build?** → [Build the MVP](build/index.md)  
**Have an MVP to launch?** → [Launch & Iterate](launch/index.md)  
**Want templates only?** → Go directly to chapter Templates  
**Want examples only?** → Go directly to chapter Examples

## Next Steps

1. **Choose your path** above based on where you are in your journey
2. **Set up required tools** for your chosen section
3. **Start with the first chapter** in your chosen section
4. **Follow chapters sequentially** (especially in Decide section)

**Most common starting point**: If you have an idea, start with [Decide What to Build](decide/index.md) to validate it before building.

***

> 💡 **Tip**: Bookmark the [Dependency Map](dependency-map.md) for quick navigation  
> 📝 **Note**: You can always return to this section if you need to reorient yourself
