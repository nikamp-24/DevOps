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

## Day 3 — Git Branching

### 1. List Branches

- `git branch` - Lists the local branches in the repository.

- `git branch --list` - Lists all local branches.

### 2. Create a Branch

- `git branch <branch-name>` - Creates a new branch with the specified name.

### 3. Switch Branch

- `git switch <branch-name>` - Switches to the specified branch.

- `git checkout <branch-name>` - Switches to the specified branch.

### 4. Create and Switch to a New Branch

- `git checkout -b <branch-name>` - Creates a new branch and switches to it immediately.

### 5. Push a Branch to Remote

- `git push <alias-name> <branch-name>` - Pushes the specified local branch to the remote repository.

### 6. List Remote Branches

- `git branch -r` - Lists the branches available on the remote repository.

### 7. List Local and Remote Branches

- `git branch -a` - Lists all local and remote branches.

### 8. Rename Current Branch

- `git branch -m <new-branch-name>` - Renames the current branch.

### 9. Rename a Specific Branch

- `git branch -m <old-branch-name> <new-branch-name>` - Renames the specified branch.

### 10. Delete Remote Branch

- `git push origin -d <branch-name>` - Deletes the specified branch from the remote repository.

## Day 3 — Git push

### 1. Delete Local Branch

- `git branch -d <branch-name>` - Deletes a local branch that has already been merged.

- `git branch -D <branch-name>` - Forcefully deletes a local branch, even if it has not been merged.

### 2. Force Push

- `git push -f origin <branch-name>` - Forcefully pushes local changes to the specified remote branch.

- `git push --force-with-lease origin <branch-name>` - Force pushes changes while checking that the remote branch has not changed unexpectedly.


## Day 4 — File and Text Commands

### 1. cat

- `cat filename` - Displays the contents of a file.

- `cat < filename` - Displays the contents of a file using input redirection.

### 2. echo

- `echo "text"` - Displays the specified text on the terminal.

- `echo "text" > filename` - Writes the specified text into a file. If the file already contains data, the existing content is replaced.

- `echo "text" >> filename` - Appends the specified text to the end of a file without replacing the existing content.

### 3. nano

- `nano filename` - Opens a file in the Nano text editor for creating or editing the file.

#### Basic Nano Steps

1. Open the file:
   `nano filename`

2. Start typing directly - Nano opens in editing mode, so you can immediately insert or modify text.

3. Save the file:
   `Ctrl + S`

4. Exit Nano:
   `Ctrl + X`

5. If Nano asks whether to save changes:
   - Press `Y` - Save changes.
   - Press `N` - Exit without saving.
   - Press `Enter` - Confirm the filename.

### 4. vi

- `vi filename` - Opens a file in the Vi text editor for creating or editing the file.

#### Basic Vi Steps

1. Open the file:
   `vi filename`

2. Enter Insert Mode:
   - Press `i` - Starts inserting text at the cursor position.

3. Type or edit your content.

4. Exit Insert Mode:
   - Press `Esc`

5. Save the file:
   - Type `:w`
   - Press `Enter`

6. Save and Exit:
   - Press `Esc`
   - Type `:wq`
   - Press `Enter`

7. Exit without saving:
   - Press `Esc`
   - Type `:q!`
   - Press `Enter`

### 5. vim

- `vim filename` - Opens a file in the Vim text editor for creating or editing the file.

#### Basic Vim Steps

1. Open the file:
   `vim filename`

2. Enter Insert Mode:
   - Press `i` - Starts inserting text.

3. Type or edit your content.

4. Exit Insert Mode:
   - Press `Esc`

5. Save the file:
   - Type `:w`
   - Press `Enter`

6. Save and Exit:
   - Press `Esc`
   - Type `:wq`
   - Press `Enter`

7. Exit without saving:
   - Press `Esc`
   - Type `:q!`
   - Press `Enter`

### Quick Reference

| Editor | Open | Insert/Edit | Save | Save & Exit | Exit Without Saving |
|---|---|---|---|---|---|
| Nano | `nano filename` | Type directly | `Ctrl + S` | `Ctrl + S`, `Ctrl + X` | `Ctrl + X`, then `N` |
| Vi | `vi filename` | `i` | `Esc` → `:w` → Enter | `Esc` → `:wq` → Enter | `Esc` → `:q!` → Enter |
| Vim | `vim filename` | `i` | `Esc` → `:w` → Enter | `Esc` → `:wq` → Enter | `Esc` → `:q!` → Enter |
