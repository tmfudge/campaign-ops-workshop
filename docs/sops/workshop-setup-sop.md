# Workshop Environment Setup SOP
Version: 1.0
Last Updated: January 12, 2025

## Purpose
This SOP provides comprehensive instructions for setting up and maintaining the workshop environment, including all necessary tools, repositories, and configurations.

## 1. Initial Setup

### 1.1 Software Installation
1. Required Software:
   - VS Code
   - Git (version 2.39.3 or higher)
   - Node.js (latest LTS version)
   - GitHub Desktop (optional)

2. Installation Steps:
   ```bash
   # Check Git version
   git --version

   # Check Node version
   node --version
   ```

### 1.2 GitHub Repository Setup
1. Repository Creation:
   ```bash
   # Navigate to Documents
   cd Documents

   # Create and initialize repository
   mkdir campaign-ops-workshop
   cd campaign-ops-workshop
   git init
   git branch -M main
   ```

2. Folder Structure Creation:
   ```bash
   # Create main folders
   mkdir -p docs assets templates prompts scripts

   # Create subfolders
   mkdir -p assets/presentations assets/images assets/videos
   mkdir -p docs/guides docs/examples docs/tutorials
   mkdir -p templates/hubspot templates/zapier templates/email
   mkdir -p prompts/claude prompts/chatgpt
   ```

3. Git Visibility Setup:
   ```bash
   # Add .gitkeep to maintain folder structure
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
   ```

### 1.3 Repository Configuration
1. Git Configuration:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your-email@example.com"
   ```

2. GitHub Connection:
   ```bash
   git remote add origin [your-repository-url]
   git push -u origin main
   ```

### 1.4 Tool Authentication
1. GitHub Authentication
   - Generate SSH key if needed
   - Add SSH key to GitHub account
   - Test connection

2. VS Code Setup
   - Install recommended extensions
   - Configure Git integration
   - Set up workspace settings

## 2. Maintenance Procedures

### 2.1 Regular Updates
1. Repository Updates:
   ```bash
   git pull origin main
   git push origin main
   ```

2. Documentation Updates:
   - Review and update SOPs monthly
   - Update README as needed
   - Maintain change logs

### 2.2 Backup Procedures
1. Local Backups:
   - Create regular local backups
   - Document backup location
   - Test restore procedures

2. Remote Backups:
   - Maintain GitHub repository
   - Consider secondary remote
   - Document recovery steps

## 3. Troubleshooting

### 3.1 Common Issues
1. Git Issues:
   - Connection problems
   - Push/pull conflicts
   - Authentication errors

2. Environment Issues:
   - Path problems
   - Permission errors
   - Tool conflicts

### 3.2 Resolution Steps
1. Git Problems:
   ```bash
   # Reset local changes
   git reset --hard origin/main

   # Clean untracked files
   git clean -fd
   ```

2. Environment Problems:
   - Verify installations
   - Check configurations
   - Validate permissions

## 4. Quality Control

### 4.1 Testing Procedures
1. Setup Validation:
   - Test all tool connections
   - Verify access rights
   - Check configurations

2. Documentation Review:
   - Verify accuracy
   - Update procedures
   - Test instructions

## Change Log
- 2025-01-12: Initial SOP creation
- [Future updates to be logged here]
