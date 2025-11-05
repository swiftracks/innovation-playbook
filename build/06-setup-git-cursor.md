# 06 — Setup: Git & Cursor

**Purpose**: Create Git repository and clone it in Cursor IDE

**Outcome**: Have a Git repository set up and cloned in Cursor, ready for development

**Audience**: PM / Dev / Both

**Time**: 15-30 minutes

**Prerequisites**: [05 — Planning](05-planning.md) - User stories, PRD, and mockups complete

## Learning Outcomes

By the end of this chapter, you will be able to:
1. Create a new Git repository in GitLab or GitHub
2. Clone the repository in Cursor IDE
3. Verify the setup is correct
4. Troubleshoot common setup issues

## Jobs-to-Be-Done

- **When**: I have a complete plan (user stories, PRD, mockups) and need to set up version control
- **I want**: To create a Git repository and clone it in Cursor
- **So that**: I can start development with proper version control and Cursor integration

## Inputs

- User stories, PRD, and mockups from [05 — Planning](05-planning.md)
- GitLab or GitHub account for version control
- Cursor IDE installed
- Basic understanding of Git

## Activities

### 1. Create Git Repository

Create a new GitLab or GitHub project for your MVP.

**Process**:

#### Option A: GitHub

1. **Navigate to GitHub**: Go to github.com and sign in
2. **Create New Repository**: 
   - Click the "+" icon in the top right
   - Select "New repository"
3. **Configure Repository**:
   - **Repository name**: Choose a name that reflects your MVP (e.g., `mvp-product-name`)
   - **Description**: Brief description of your MVP (optional)
   - **Visibility**: Choose Private (recommended for MVP) or Public
   - **Initialize repository**: 
     - Optionally check "Add a README file"
     - Optionally add `.gitignore` (choose Node template if using Node.js)
     - Optionally add a license (not necessary for MVP)
4. **Create Repository**: Click "Create repository"
5. **Note Repository URL**: Copy the repository URL (HTTPS or SSH)

#### Option B: GitLab

1. **Navigate to GitLab**: Go to gitlab.com and sign in
2. **Create New Project**: 
   - Click "New project" or the "+" icon
   - Select "Create blank project"
3. **Configure Project**:
   - **Project name**: Choose a name that reflects your MVP (e.g., `mvp-product-name`)
   - **Project slug**: Will auto-populate (can be changed)
   - **Visibility Level**: Choose Private (recommended for MVP) or Public
   - **Initialize repository**: 
     - Optionally check "Initialize repository with a README"
4. **Create Project**: Click "Create project"
5. **Note Repository URL**: Copy the repository URL (HTTPS or SSH)

**Repository Naming Tips**:
- Keep it simple and descriptive
- Use lowercase and hyphens (e.g., `mvp-retrospective-tool`)
- Avoid special characters and spaces
- Make it easy to remember and identify

> 💡 **Tip**: Choose a repository name that reflects your MVP. Keep it simple and descriptive. You can always rename it later if needed.

### 2. Clone Repository in Cursor

Open Cursor and clone your Git repository.

**Process**:

#### Method 1: Clone via Cursor UI

1. **Open Cursor IDE**: Launch Cursor application
2. **Clone Repository**:
   - Click "File" → "Clone Repository" (or use keyboard shortcut)
   - Alternatively, click "File" → "Open Folder" and then clone
3. **Enter Repository URL**:
   - Paste the repository URL you copied
   - Cursor will detect if it's a Git repository
4. **Choose Clone Location**:
   - Select where to clone the repository on your local machine
   - Choose a location you can easily find (e.g., `Documents/Projects/`)
5. **Clone Repository**:
   - Click "Clone" or "Open"
   - Cursor will clone the repository and open it
6. **Verify Clone**:
   - Check that the repository folder is open in Cursor
   - Verify you can see files (README if you created one)

#### Method 2: Clone via Command Palette

1. **Open Cursor IDE**: Launch Cursor application
2. **Open Command Palette**:
   - Press `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac)
   - Type "Git: Clone"
3. **Enter Repository URL**:
   - Paste the repository URL
   - Press Enter
4. **Choose Clone Location**:
   - Select the folder where you want to clone
5. **Open Repository**:
   - Cursor will ask if you want to open the cloned repository
   - Click "Open" to open it in Cursor

#### Method 3: Clone via Terminal (Advanced)

If you prefer using the terminal:

1. **Open Terminal in Cursor**:
   - Press `` Ctrl+` `` (backtick) to open integrated terminal
2. **Navigate to Project Directory**:
   ```bash
   cd ~/Documents/Projects  # or your preferred location
   ```
3. **Clone Repository**:
   ```bash
   git clone <repository-url>
   ```
4. **Open in Cursor**:
   - Use "File" → "Open Folder"
   - Navigate to the cloned repository folder
   - Click "Select Folder"

**Troubleshooting**:

- **Authentication Issues**: If you get authentication errors:
  - For HTTPS: You may need to set up a personal access token
  - For SSH: Ensure your SSH key is set up with GitHub/GitLab
  - See authentication documentation for your Git provider

- **Repository Not Found**: 
  - Verify the repository URL is correct
  - Ensure you have access to the repository
  - Check that the repository exists

- **Permission Denied**:
  - Verify you have read/write access to the repository
  - Check your Git provider account permissions

### 3. Verify Setup

Ensure the repository is properly set up and ready for development.

**Verification Steps**:

1. **Check Repository Status**:
   - Open the integrated terminal in Cursor (`` Ctrl+` ``)
   - Run: `git status`
   - Should show "On branch main" (or "master") and "nothing to commit"

2. **Verify Remote Connection**:
   - Run: `git remote -v`
   - Should show your repository URL (origin)

3. **Check File Structure**:
   - Verify you can see the repository files in Cursor's file explorer
   - If you initialized with README, you should see `README.md`

4. **Test Git Operations**:
   - Make a small test change (e.g., edit README.md)
   - Run: `git status` - should show the modified file
   - Run: `git diff` - should show the changes

**If Setup is Correct**:
- ✅ Repository is cloned
- ✅ Cursor is open to the repository folder
- ✅ Git is working properly
- ✅ Remote connection is configured
- ✅ Ready to proceed to `.cursorrules` setup

> 💡 **Tip**: If you encounter any issues, check the Cursor documentation or Git provider documentation for troubleshooting steps.

## Apply It Now

**Task**: Create Git repository and clone it in Cursor

1. Create a new repository in GitLab or GitHub
   - Choose a descriptive name
   - Set visibility (Private recommended for MVP)
   - Optionally initialize with README
   - Copy the repository URL

2. Clone repository in Cursor
   - Use Cursor's clone feature
   - Choose a local location
   - Open the cloned repository

3. Verify setup
   - Check Git status
   - Verify remote connection
   - Ensure repository is properly configured

**Artifacts**: You'll create:
- Git repository (GitLab or GitHub)
- Local cloned repository
- Repository ready for development

## Artifacts

You'll create:
- Git repository (remote)
- Local cloned repository
- Connection between local and remote repository

## Worked Example

**Situation**: Setting up Git repository for a B2B AI SaaS MVP

**Git Setup Process**:
1. **Repository Creation**: 
   - Created GitHub repository named `mvp-retrospective-tool`
   - Set visibility to Private
   - Initialized with README.md
   - Copied repository URL: `https://github.com/username/mvp-retrospective-tool.git`

2. **Clone in Cursor**:
   - Opened Cursor IDE
   - Used File → Clone Repository
   - Pasted repository URL
   - Cloned to `~/Documents/Projects/mvp-retrospective-tool`
   - Cursor automatically opened the repository

3. **Verification**:
   - Ran `git status` - confirmed clean repository
   - Ran `git remote -v` - confirmed remote connection
   - Verified README.md is visible in Cursor
   - Ready for next step

**Time**: 15 minutes total

## Checklist

Before proceeding to `.cursorrules` setup, verify:
- [ ] Git repository created in GitLab or GitHub
- [ ] Repository URL copied
- [ ] Repository cloned in Cursor
- [ ] Repository folder open in Cursor
- [ ] Git status verified (run `git status`)
- [ ] Remote connection verified (run `git remote -v`)
- [ ] Ready to proceed to `.cursorrules` setup

## Self-Assessment

1. **What should you do after creating the Git repository?**
   - [ ] Start coding immediately
   - [ ] Clone the repository in Cursor ✓
   - [ ] Deploy to production
   - [ ] Skip version control

2. **How do you verify the repository is properly cloned?**
   - [ ] Check the repository URL
   - [ ] Run `git status` and verify remote connection ✓
   - [ ] Deploy the application
   - [ ] Create a new branch

3. **What should you do if you get authentication errors?**
   - [ ] Skip Git setup
   - [ ] Check your Git provider authentication settings ✓
   - [ ] Use a different repository
   - [ ] Continue without Git

## Exit Criteria

You're ready to proceed to `.cursorrules` setup when:
- [ ] Git repository is created and accessible
- [ ] Repository is cloned in Cursor
- [ ] Repository folder is open in Cursor
- [ ] Git is working properly (verified with `git status`)
- [ ] Remote connection is configured correctly

## Dependencies & Next Steps

### Prerequisites Completed
- [05 — Planning](05-planning.md) - User stories, PRD, and mockups complete

### Next Steps
- Proceed to [06 — Setup: .cursorrules](06-setup-cursorrules.md) to configure development rules for Cursor

### What This Enables

Completing Git and Cursor setup enables:
- Version control for your MVP
- Cursor IDE ready for development
- Proper repository structure
- Foundation for collaborative development

### Related Resources

- [06 — Setup](06-setup.md) - Return to Setup overview
- Git provider documentation (GitHub or GitLab)

---

> 💡 **Tip**: Take time to set up Git properly. Good version control practices will save you time and help you collaborate effectively.
> 📝 **Note**: The repository structure will be set up in the next step when you configure `.cursorrules` and create the implementation plan.

