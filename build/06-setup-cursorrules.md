# 06 — Setup: .cursorrules

**Purpose**: Configure `.cursorrules` file with development rules for rapid MVP development

**Outcome**: Have a customized `.cursorrules` file that guides Cursor to generate high-quality code aligned with your MVP needs

**Audience**: PM / Dev / Both

**Time**: 30-60 minutes

**Prerequisites**: [06 — Setup: Git & Cursor](06-setup-git-cursor.md) - Git repository cloned in Cursor

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Understand what `.cursorrules` is and why it's critical
2. Create a `.cursorrules` file using the template
3. Customize rules based on your specific needs
4. Configure rules for TypeScript, React, and MVP development
5. Ensure rules align with your tech stack and coding standards

## Jobs-to-Be-Done

- **When**: I have cloned my repository in Cursor and need to configure development rules
- **I want**: To set up `.cursorrules` with strong development guidelines
- **So that**: Cursor generates high-quality, consistent code that follows best practices

## Inputs

- Git repository cloned in Cursor from [06 — Setup: Git & Cursor](06-setup-git-cursor.md)
- Repository open in Cursor IDE
- Understanding of your tech stack
- [.cursorrules Template](05-setup-cursorrules-template.md) for reference

## Activities

### 1. Understand .cursorrules

Before creating your `.cursorrules` file, understand what it is and why it's important.

**What is `.cursorrules`?**
- A configuration file that tells Cursor how to write code
- Contains rules, guidelines, and best practices for code generation
- Acts as a "coding style guide" for AI-assisted development
- Helps Cursor understand your project's specific needs and constraints

**Why is it critical?**
- **Consistency**: Ensures Cursor generates code that follows your standards
- **Quality**: Helps Cursor avoid common mistakes and anti-patterns
- **Efficiency**: Reduces need for code review and refactoring
- **Alignment**: Keeps generated code aligned with your tech stack and MVP scope
- **Time Savings**: Better code generation means less time fixing issues

**What happens without `.cursorrules`?**
- Cursor may generate code that doesn't follow your conventions
- Inconsistent patterns across the codebase
- Potential over-engineering or under-engineering
- Missing best practices for your specific stack
- More time spent on code review and fixes

> ⚠️ **Warning**: Strong `.cursorrules` help Cursor generate better code. Don't skip this step - it significantly improves code quality and consistency throughout development.

### 2. Review the Template

Review the `.cursorrules` template to understand what's included.

**Template Location**: [.cursorrules Template](05-setup-cursorrules-template.md)

**Key Sections in Template**:
- **Core Principles**: MVP-first mindset, quality over speed, type safety
- **Code Quality Standards**: TypeScript, React, code organization, error handling
- **Technology Stack Conventions**: React, Zustand, Tailwind, Radix UI, Firebase
- **Development Workflow**: Before/during/after writing code
- **Performance Considerations**: Lazy loading, optimization, bundle size
- **Security**: API keys, validation, authentication
- **Accessibility**: Semantic HTML, keyboard navigation, ARIA
- **MVP-Specific Guidelines**: Ship fast, user value first, technical debt

**Review Process**:
1. Open the template file: [05-setup-cursorrules-template.md](05-setup-cursorrules-template.md)
2. Read through each section
3. Understand what each section covers
4. Note sections that may need customization for your MVP
5. Identify any additional rules you might need

> 💡 **Tip**: Take time to understand the template. The more you understand it, the better you can customize it for your needs.

### 3. Create .cursorrules File

Create a `.cursorrules` file in your project root.

**Process**:

1. **Open Repository in Cursor**: Ensure your repository folder is open
2. **Create New File**:
   - Right-click in the file explorer (root folder)
   - Select "New File"
   - Name it exactly: `.cursorrules` (including the leading dot)
   - Alternatively, use File → New File and save as `.cursorrules`
3. **Copy Template Content**:
   - Open the template: [05-setup-cursorrules-template.md](05-setup-cursorrules-template.md)
   - Copy the entire content (everything inside the markdown code block)
   - Paste into your new `.cursorrules` file
4. **Save File**: Save the file (Cursor should auto-save)

**File Location**:
- Must be in the project root (same level as `package.json` or `README.md`)
- File name: `.cursorrules` (exact name, with leading dot)
- No file extension needed

**Verification**:
- Check that `.cursorrules` appears in your file explorer
- Verify it's in the root folder
- Open the file to confirm content is there

### 4. Customize Rules for Your MVP

Customize the `.cursorrules` file based on your specific needs.

**Customization Process**:

#### Step 1: Review Core Principles

Review and adjust core principles if needed:
- **MVP First**: Ensure this aligns with your approach
- **Quality Over Speed**: Adjust balance if needed
- **Type Safety**: Confirm TypeScript strict mode is appropriate
- **Component Reusability**: Adjust based on your component strategy

#### Step 2: Customize Code Quality Standards

**TypeScript Configuration**:
- Verify strict mode settings match your preferences
- Adjust type inference preferences if needed
- Add any project-specific type conventions

**React Best Practices**:
- Confirm component patterns match your approach
- Adjust hook usage guidelines if needed
- Add any React 19 specific patterns you want to use

**Code Organization**:
- Review folder structure suggestions
- Adjust to match your preferred organization
- Add any project-specific folders (e.g., `src/lib/`, `src/config/`)

**Error Handling**:
- Review error handling patterns
- Adjust based on your error handling strategy
- Add any logging or monitoring requirements

#### Step 3: Verify Tech Stack Conventions

Review each technology section and ensure it matches your stack:

**Core Framework**:
- Verify React version matches your plan
- Confirm TypeScript version
- Check Vite configuration if applicable

**State Management**:
- Verify Zustand patterns (or adjust if using different state management)
- Add any store organization preferences

**Styling**:
- Confirm Tailwind CSS usage
- Verify Radix UI components you're using
- Add any design system or theme requirements

**Backend**:
- Verify Firebase services you're using
- Add any Firebase-specific patterns
- Include security rules guidelines

**AI Integration** (if applicable):
- Add Anthropic SDK patterns
- Include prompt engineering guidelines
- Add error handling for AI features

#### Step 4: Add MVP-Specific Rules

Add any rules specific to your MVP:

**Examples**:
- Specific component patterns for your domain
- Data model conventions
- API integration patterns
- Authentication flow requirements
- Any domain-specific best practices

**Process**:
1. Review your PRD for any specific technical requirements
2. Add rules that enforce these requirements
3. Include any constraints or limitations
4. Document any MVP-specific shortcuts or technical debt

#### Step 5: Review and Refine

**Review Checklist**:
- [ ] All sections are relevant to your MVP
- [ ] Tech stack matches your implementation plan
- [ ] Code organization matches your preferences
- [ ] MVP-specific guidelines are included
- [ ] Rules are clear and actionable
- [ ] No conflicting guidelines

**Common Customizations**:
- Adjust folder structure
- Add specific component patterns
- Include domain-specific rules
- Add project-specific conventions
- Remove irrelevant sections (if any)

### 5. Test .cursorrules Configuration

Test that Cursor recognizes and uses your `.cursorrules` file.

**Testing Process**:

1. **Verify File Recognition**:
   - Open Cursor
   - Check that Cursor recognizes the `.cursorrules` file
   - Cursor should automatically use the rules

2. **Test Code Generation**:
   - Ask Cursor to generate a simple component
   - Verify it follows your rules:
     - TypeScript types are used
     - Component structure matches your conventions
     - Error handling is included
     - Code organization follows your structure

3. **Check Consistency**:
   - Generate multiple components
   - Verify consistency across generated code
   - Ensure rules are being followed

**If Rules Aren't Working**:
- Verify file is named exactly `.cursorrules`
- Check file is in project root
- Ensure file has content (not empty)
- Try restarting Cursor
- Check Cursor documentation for any issues

### 6. Commit .cursorrules to Repository

Save your `.cursorrules` file to version control.

**Process**:

1. **Stage File**:
   ```bash
   git add .cursorrules
   ```

2. **Commit File**:
   ```bash
   git commit -m "Add .cursorrules configuration"
   ```

3. **Push to Remote**:
   ```bash
   git push
   ```

**Why Commit It?**
- Ensures consistency across team members
- Version control for rule changes
- Easy to share and collaborate
- Part of project setup documentation

> 💡 **Tip**: Keep `.cursorrules` in version control. It's part of your project configuration and should be shared with the team.

## Apply It Now

**Task**: Create and customize `.cursorrules` file

1. Review the `.cursorrules` template
   - Understand what's included
   - Identify customization needs

2. Create `.cursorrules` file in project root
   - Copy template content
   - Save as `.cursorrules` in root folder

3. Customize rules for your MVP
   - Adjust core principles if needed
   - Customize code quality standards
   - Verify tech stack conventions
   - Add MVP-specific rules

4. Test configuration
   - Verify Cursor recognizes the file
   - Test code generation
   - Check consistency

5. Commit to repository
   - Add `.cursorrules` to Git
   - Commit and push changes

**Artifacts**: You'll create:
- `.cursorrules` file in project root
- Customized rules for your MVP
- Configuration committed to repository

## Artifacts

You'll create:
- `.cursorrules` file with development rules
- Customized configuration for your MVP
- Version-controlled rules file

## Worked Example

**Situation**: Setting up `.cursorrules` for a B2B AI SaaS retrospective tool

**Setup Process**:
1. **Template Review**: Reviewed template and identified customization needs
   - Tech stack matches: React 19, TypeScript, Firebase, Anthropic
   - Need to add retrospective-specific patterns
   - Need to include AI integration guidelines

2. **File Creation**: Created `.cursorrules` in project root
   - Copied template content
   - Saved as `.cursorrules`

3. **Customization**:
   - **Code Organization**: Added `src/features/retrospectives/` folder structure
   - **AI Integration**: Added Anthropic SDK patterns and prompt guidelines
   - **Data Model**: Added Firestore patterns for retrospective data
   - **Component Patterns**: Added specific patterns for retrospective UI
   - **MVP Guidelines**: Added rules for rapid iteration on insights

4. **Testing**: Tested with Cursor
   - Generated a simple component
   - Verified TypeScript types and structure
   - Confirmed rules were followed

5. **Commit**: Committed to repository
   - `git add .cursorrules`
   - `git commit -m "Add .cursorrules with MVP-specific rules"`
   - `git push`

**Time**: 45 minutes total (30 min customization, 15 min testing)

## Checklist

Before proceeding to implementation planning, verify:
- [ ] `.cursorrules` file created in project root
- [ ] Template content copied and customized
- [ ] Rules customized for your MVP
- [ ] Tech stack conventions verified
- [ ] MVP-specific rules added
- [ ] Configuration tested with Cursor
- [ ] File committed to repository
- [ ] Ready to proceed to implementation planning

## Self-Assessment

1. **Where should `.cursorrules` be located?**
   - [ ] In any folder
   - [ ] In project root ✓
   - [ ] In src folder
   - [ ] It doesn't matter

2. **What should you customize in `.cursorrules`?** (Select all)
   - [ ] Tech stack conventions ✓
   - [ ] Code organization ✓
   - [ ] MVP-specific rules ✓
   - [ ] Everything in the template

3. **Why is `.cursorrules` important?**
   - [ ] It's optional
   - [ ] It helps Cursor generate better, consistent code ✓
   - [ ] It's required for Cursor to work
   - [ ] It's only for documentation

## Exit Criteria

You're ready to proceed to implementation planning when:
- [ ] `.cursorrules` file is created in project root
- [ ] Rules are customized for your MVP
- [ ] Tech stack conventions are verified
- [ ] Configuration is tested and working
- [ ] File is committed to repository

## Dependencies & Next Steps

### Prerequisites Completed
- [06 — Setup: Git & Cursor](06-setup-git-cursor.md) - Git repository cloned in Cursor

### Next Steps
- Proceed to [06 — Setup: Implementation Planning](06-setup-implementation-planning.md) to use Cursor Plan Mode and create implementation plan

### What This Enables

Completing `.cursorrules` setup enables:
- Consistent code generation from Cursor
- Better code quality from the start
- Reduced time on code review
- Alignment with your tech stack and standards
- Efficient MVP development

### Related Resources

- [.cursorrules Template](05-setup-cursorrules-template.md) - Template for Cursor development rules
- [06 — Setup](06-setup.md) - Return to Setup overview

---

> 💡 **Tip**: Take time to customize `.cursorrules` properly. Well-configured rules will save significant time during development.
> 📝 **Note**: You can update `.cursorrules` as your project evolves. Don't be afraid to refine it based on what you learn.
> ⚠️ **Warning**: Don't skip `.cursorrules` setup. It's critical for maintaining code quality and consistency throughout development.

