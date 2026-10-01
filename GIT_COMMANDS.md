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


## Day 2 — Remote Repository & Git Pull

### 1. Git Local Configuration

- `git config user.name "Your Name"` - Sets the Git username locally for the current repository.

- `git config user.email "your@email.com"` - Sets the Git email locally for the current repository.

- `git config --list` - Displays the Git configuration settings for the current repository.

- `git config --local --list` - Displays only the local configuration settings of the current repository.

### 2. Connect Local Repository to GitHub

- `git remote add origin <repository-url>` - Connects the local Git repository to a remote GitHub repository.

### 3. Git Remote

- `git remote -v` - Displays the URLs of the remote repositories for fetching and pushing.

- `git remote` - Displays the names of the configured remote repositories.

### 4. Meaning of Origin

- `origin` - The default name commonly given to the remote GitHub repository when a remote repository is added.

- `git remote add origin <repository-url>` - Adds the GitHub repository as a remote named `origin`.

### 5. Git Pull

- `git pull` - Fetches the latest changes from the remote repository and merges them into the current local branch.

- `git pull origin main` - Fetches and merges the latest changes from the `main` branch of the remote repository named `origin`.

### 6. Git Fetch

- `git fetch` - Downloads the latest changes from the remote repository without merging them into the current branch.

- `git fetch origin` - Fetches the latest changes from the remote repository named `origin`.

### 7. Verbose Output

- `git pull -v` - Performs a pull operation and displays detailed information about the operation.

- `git fetch -v` - Fetches changes and displays detailed information about the operation.

- `git remote -v` - Displays the remote repository URLs for fetch and push operations.
