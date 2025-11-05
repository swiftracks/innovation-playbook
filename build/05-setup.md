# 05 — Setup

**Purpose**: Set up development environment and infrastructure

**Outcome**: Have a working development environment ready for building

**Audience**: PM / Dev / Both

**Time**: 4-8 hours

**Prerequisites**: [Decide What to Build](decide/index.md) - Decision to build

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Set up development environment and tools
2. Configure version control and CI/CD
3. Set up deployment infrastructure
4. Establish development workflow
5. Prepare for efficient building

## Jobs-to-Be-Done

- **When**: I have a decision to build and need to set up development
- **I want**: To set up development environment and infrastructure
- **So that**: I can build efficiently and deploy easily

## Inputs

- Decision to build from [06 — Synthesize Insights → Decision](decide/06-synthesize-insights-decision.md)
- Understanding of technology stack
- Access to deployment infrastructure
- Development tools and accounts

## Activities

### 1. Set Up Development Environment

**Choose Technology Stack**:
- **Frontend**: React, Vue, or similar
- **Backend**: Node.js, Python, or similar
- **Database**: PostgreSQL, MongoDB, or similar
- **AI/ML**: OpenAI, Anthropic, or similar

**Set Up Local Environment**:
- Install development tools
- Configure IDE/editor
- Set up package managers
- Install dependencies

> 💡 **Tip**: Use tools you're familiar with. Don't over-engineer for MVP.

### 2. Configure Version Control

**Set Up Git**:
- Initialize repository
- Configure .gitignore
- Set up branch strategy
- Configure remotes

**Branch Strategy** (simple for MVP):
- `main` - Production-ready code
- `develop` - Development branch
- `feature/*` - Feature branches

### 3. Set Up CI/CD

**Basic CI/CD Pipeline**:
- Automated tests (if applicable)
- Build process
- Deployment automation

**Tools** (choose one):
- GitHub Actions
- GitLab CI
- CircleCI
- Simple scripts

> 📝 **Note**: Keep CI/CD simple for MVP. You can enhance later.

### 4. Set Up Deployment Infrastructure

**Choose Deployment Platform**:
- **Cloud**: AWS, GCP, Azure
- **Platforms**: Heroku, Vercel, Netlify
- **Containers**: Docker, Kubernetes (if needed)

**Set Up Environments**:
- **Development**: Local development
- **Staging**: Pre-production testing
- **Production**: Live MVP

> 🎯 **Goal**: Deploy easily and reliably. Don't over-complicate.

### 5. Establish Development Workflow

**Workflow Steps**:
1. Create feature branch
2. Make changes locally
3. Test locally
4. Commit and push
5. Create pull request
6. Review and merge
7. Deploy automatically

**Documentation**:
- Setup instructions
- Development workflow
- Deployment process
- Troubleshooting guide

## Apply It Now

**Task**: Set up your development environment

1. Choose and set up technology stack
2. Configure version control (Git)
3. Set up basic CI/CD pipeline
4. Set up deployment infrastructure
5. Establish development workflow
6. Document setup and workflow

**Artifact**: A setup document with:
- Technology stack choices
- Development environment setup
- CI/CD configuration
- Deployment infrastructure
- Development workflow

## Artifacts

You'll create:
- Development environment setup
- Git repository configuration
- CI/CD pipeline configuration
- Deployment infrastructure setup
- Development workflow documentation

## Worked Example

**Situation**: Setting up for retrospective tool MVP

**Technology Stack**:
- Frontend: React + TypeScript
- Backend: Node.js + Express
- Database: PostgreSQL
- AI: OpenAI API
- Deployment: Vercel (frontend) + Railway (backend)

**Setup**:
```
1. Initialize Git repository
2. Set up React + TypeScript project
3. Set up Node.js + Express backend
4. Configure PostgreSQL database
5. Set up OpenAI API integration
6. Configure Vercel and Railway deployment
7. Set up basic CI/CD with GitHub Actions
```

**Development Workflow**:
```
1. Create feature branch: git checkout -b feature/ai-baseline
2. Make changes locally
3. Test locally: npm run dev
4. Commit: git commit -m "Add AI baseline"
5. Push: git push origin feature/ai-baseline
6. Create PR on GitHub
7. Review and merge
8. Auto-deploy to staging
```

## Checklist

Before proceeding to the next chapter, verify:
- [ ] Development environment is set up
- [ ] Version control is configured
- [ ] CI/CD pipeline is working
- [ ] Deployment infrastructure is ready
- [ ] Development workflow is established
- [ ] Setup is documented

## Self-Assessment

1. **What should you prioritize in MVP setup?**
   - [ ] Complex infrastructure
   - [ ] Simple, working setup ✓
   - [ ] Perfect tooling

2. **What environments should you set up?** (Select all)
   - [ ] Development ✓
   - [ ] Staging ✓
   - [ ] Production ✓
   - [ ] All environments

3. **What should be in your development workflow?** (Select all)
   - [ ] Feature branches ✓
   - [ ] Local testing ✓
   - [ ] Automated deployment ✓
   - [ ] Manual deployment only

## Exit Criteria

You're ready to proceed when:
- [ ] Development environment is set up and working
- [ ] Version control is configured
- [ ] CI/CD pipeline is working
- [ ] Deployment infrastructure is ready
- [ ] You can deploy code successfully

## Dependencies & Next Steps

### Prerequisites Completed
- [Decide What to Build](decide/index.md) - Decision to build

### Next Steps
- Proceed to [06 — AI Baseline](06-ai-baseline.md) to build core AI functionality
- OR proceed to [07 — UX Thin Vertical](07-ux-thin-vertical.md) to build user experience
- These can be done in parallel after setup

### What This Enables

Setup enables:
- Efficient development
- Automated deployment
- Reliable infrastructure
- Smooth development workflow

---

> 💡 **Tip**: Keep setup simple for MVP. You can enhance later.
> 📝 **Note**: Document your setup. You'll forget details later.
