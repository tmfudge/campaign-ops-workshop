# Campaign Operations Workshop: Standard Operating Procedure (SOP)

## Section 1: Initial Setup

### 1.1 Required Software Installation
1. Install VS Code
   - Go to https://code.visualstudio.com/
   - Click the download button for your operating system
   - Run the installer
   - Open VS Code after installation

2. Install Git
   - Go to https://git-scm.com/downloads
   - Download and install Git for your operating system
   - Open terminal/command prompt and verify installation:
     ```bash
     git --version
     ```

3. Install Essential VS Code Extensions
   - Click the Extensions icon in VS Code (looks like four squares)
   - Search for and install:
     - "GitHub Pull Requests and Issues"
     - "GitLens"
     - "Markdown All in One"

### 1.2 GitHub Account Setup
1. Create GitHub Account (if you don't have one)
   - Go to https://github.com
   - Click "Sign up"
   - Follow the registration process
   - Verify your email address

2. Configure Git with GitHub
   - Open terminal in VS Code (Top menu: View > Terminal)
   - Set your Git username:
     ```bash
     git config --global user.name "Your Name"
     ```
   - Set your Git email:
     ```bash
     git config --global user.email "your-email@example.com"
     ```

### 1.3 Creating Your First Repository
1. Create Repository on GitHub
   - Go to https://github.com
   - Click the "+" in the top right
   - Select "New repository"
   - Name it "campaign-ops-workshop"
   - Add a description: "AI-Driven Marketing Campaign Operations Workshop"
   - Select "Public"
   - Check "Add a README file"
   - Click "Create repository"

2. Clone Repository in VS Code
   - In VS Code, press `Ctrl+Shift+P` (Windows/Linux) or `Cmd+Shift+P` (Mac)
   - Type "Git: Clone"
   - Press Enter
   - Paste your repository URL
   - Select a folder on your computer to store the project
   - Click "Open" when prompted

### 1.4 Basic Repository Structure
1. Create Essential Folders
   - In VS Code terminal, create the folder structure:
     ```bash
     # Create main folders
     mkdir -p docs assets templates prompts scripts

     # Create subfolders
     mkdir -p assets/presentations assets/images assets/videos
     mkdir -p docs/guides docs/examples docs/tutorials
     mkdir -p templates/hubspot templates/zapier templates/email
     mkdir -p prompts/claude prompts/chatgpt
     ```

2. Make Folders Visible in Git
   - Empty folders won't show in Git by default
   - Add .gitkeep files to make them visible:
     ```bash
     # Add .gitkeep to each folder
     touch docs/.gitkeep
     touch assets/presentations/.gitkeep
     touch assets/images/.gitkeep
     touch assets/videos/.gitkeep
     touch docs/guides/.gitkeep
     touch docs/examples/.gitkeep
     touch docs/tutorials/.gitkeep
     touch templates/hubspot/.gitkeep
     touch templates/zapier/.gitkeep
     touch templates/email/.gitkeep
     touch prompts/claude/.gitkeep
     touch prompts/chatgpt/.gitkeep
     touch scripts/.gitkeep

     # Add and commit these files
     git add -A
     git commit -m "Add .gitkeep files to maintain folder structure"
     git push origin main
     ```

2. Create Initial Files
   - Right-click in Explorer > New File
   - Create these files:
     - WORKSHOP.md (workshop overview)
     - SETUP.md (setup instructions)
     - .gitignore (for files to ignore)

### 1.5 Making Your First Commit
1. Stage Changes
   - Click the Source Control icon in VS Code (branch icon)
   - Click the "+" next to each changed file to stage them

2. Commit Changes
   - Enter a commit message: "Initial workshop setup"
   - Click the checkmark or press `Ctrl+Enter`

3. Push Changes
   - Click the "..." menu in Source Control
   - Select "Push"
   - Enter your GitHub credentials if prompted

## Section 2: Workshop Content Organization

### 2.1 Documentation Structure
1. Workshop Overview
   - Create docs/README.md
   - Include:
     - Workshop objectives
     - Prerequisites
     - Tools required
     - Learning outcomes

2. Implementation Guides
   - Create docs/guides/
   - Separate guides for:
     - HubSpot setup
     - AI tools configuration
     - Integration setup

### 2.2 Template Organization
1. Create Template Categories
   - templates/hubspot/ (HubSpot workflows)
   - templates/email/ (Email templates)
   - templates/automation/ (Automation workflows)

2. Template Documentation
   - Add README.md in each template folder
   - Document usage instructions
   - Include examples

## Next Steps
- Setting up AI tool connections
- Creating workshop materials
- Developing automation workflows
- Building presentation assets

Note: This SOP will be continuously updated as we progress through the workshop development.

## For Workshop Students
If you're a student accessing this repository:
1. Follow Section 1.1 and 1.2 for initial setup
2. Skip Section 1.3 (repository creation)
3. Instead of cloning, you'll fork the repository:
   - Click "Fork" in the top right of the repository page
   - Follow Section 1.4 and beyond for working with the content

