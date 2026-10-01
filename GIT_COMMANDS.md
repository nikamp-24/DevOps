# Git Commands

## Day 1 — Git Basics

### 1. Initialize Repository

- `git init` - Initializes an empty Git repository in the current project folder.

### 2. Git Configuration

- `git config --global user.name "Your Name"` - Sets your Git username globally.
- `git config --global user.email "your@email.com"` - Sets your Git email globally.
- `git config --global --list` - Displays the Git configuration settings.

### 3. Git Status

- `git status` - Shows the current status of the working directory and staging area.

### 4. Add Files to Staging Area

- `git add filename` - Adds a specific file to the staging area.
- `git add .` - Adds all modified and untracked files to the staging area.

### 5. Commit Changes

- `git commit -m "message"` - Saves the staged changes in the local Git repository with a commit message.

### 6. Git Log

- `git log` - Displays the commit history of the repository.
- `git log --oneline` - Displays the commit history in a short, one-line format.

### 7. Verbose Output

- `git push -v` - Pushes commits to the remote repository and displays detailed information about the operation.

### 8. Push to GitHub

- `git push origin main` - Pushes the local commits from the `main` branch to the remote GitHub repository.
