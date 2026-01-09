# =========================
# GLOBAL GIT CONFIGURATION
# =========================

# Set your Git username (shown in commits)
git config --global user.name "Your Name"

# Set your Git email (should match GitHub email)
git config --global user.email "you@example.com"

# Set VS Code as the default Git editor
git config --global core.editor "code --wait"

# Handle line endings (recommended for macOS/Linux)
git config --global core.autocrlf input

# Open and edit the global Git configuration file
git config --global -e



# =========================
# CHECKING GIT HISTORY
# =========================

# Show commit history in one-line format
git log --oneline

# Show full commit history
git log



# =========================
# RESET / ROLLBACK
# =========================

# Move HEAD back by 1 commit and discard all changes
# ⚠️ This will permanently delete the last commit
git reset --hard HEAD~1



# =========================
# FILE STATUS
# =========================

# Short status (compact view)
git status -s

# Detailed status of tracked and untracked files
git status



# =========================
# REMOVE GIT FROM PROJECT
# =========================

# Remove Git tracking from the project
# ⚠️ This deletes Git history permanently
rm -rf .git



# =========================
# BRANCHING
# =========================

# Create a new branch
git branch branch_name

# List all branches
git branch

# Switch to an existing branch
git switch branchName

# Create a new branch and switch to it
git switch -C branchName

# Delete a branch (safe delete)
git branch -d branchName



# =========================
# MERGING
# =========================

# First switch to main branch
git switch main

# Merge another branch into main
git merge branchName



# =========================
# STASHING CHANGES
# =========================

# Save uncommitted changes temporarily
git stash

# Apply the last stashed changes
git stash apply



# =========================
# CLONING A REPOSITORY
# =========================

# Clone a GitHub repository to your local machine
git clone repository_link



# =====================================================
# COLLABORATION WORKFLOW (COMPUTER & DEVELOPER - HET)
# =====================================================

# ---------- COMPUTER (MAIN OWNER) ----------

# 1. Create project
# 2. Initialize Git and write initial code
# 3. Push code to GitHub main branch
git init
git add .
git commit -m "Initial commit"
git push origin main

# 4. Give GitHub access to Het



# ---------- DEVELOPER (HET) ----------

# Clone the project from GitHub
git clone repository_link

# Create and switch to a new branch
git switch -C feature_branch

# Make code changes
git add .
git commit -m "Added new feature"

# Push branch to GitHub
git push -u origin feature_branch



# ---------- COMPUTER (MERGE CHANGES) ----------

# Fetch all remote branches
git fetch

# View available branches
git branch

# Switch to feature branch (optional review)
git switch feature_branch

# Switch back to main branch
git switch main

# Merge feature branch into main
git merge feature_branch

# Push updated main branch to GitHub
git push origin main



# ---------- DEVELOPER (HET SYNC MAIN) ----------

# Switch to main branch
git switch main

# Fetch latest changes
git fetch

# Pull latest main branch updates
git pull
