# README - Git Zero to Hero

## Git Fundamentals

### Saving Changes
```sh
git add file.txt   # Add a specific file to staging
git add .          # Add all changes from the current directory
git add -A         # Add all changes in the entire repository
```

### Checking Status
```sh
git status   # Show the current state of the working directory and staging area
```

### Viewing Commit History
```sh
git log             # Show a detailed history of commits
git log --oneline   # Show a concise commit history (one commit per line)
```

### Undoing Changes
```sh
git reset HEAD~1             # Undo the last commit and remove it from history
git revert <commitHash>      # Create a new commit that reverts the specified commit
git commit --amend --no-edit # Modify the last commit without creating a new one
```

### Undoing Untracked Changes
```sh
git clean -f      # Remove all untracked changes from the current directory
git clean -fd     # Remove all untracked changes from the entire repository
git reset --hard  # Reset everything to the last committed state
```

### Stashing Changes
```sh
git stash    # Stash changes temporarily
git stash -u # Stash all changes, including untracked files
```

### Viewing Stash List
```sh
git stash list   # Show all stashed changes
```

### Applying Stashed Changes
```sh
git stash pop   # Apply the latest stash and remove it from the stash list
```

### Branch Management
```sh
git checkout branch-name    # Switch to an existing branch
git checkout -b branch-name # Create and switch to a new branch
```

### Merging Branches
```sh
git merge another-branch   # Merge specified branch into the current one
```

### Viewing Branches
```sh
git branch --list   # List all branches
```

### Deleting a Branch
```sh
git branch -D branch-name   # Delete a specific branch
```

## Working with GitHub

### Cloning a Repository
```sh
git clone <repoUrl>   # Clone a repository from GitHub
```

### Adding a Remote Repository
```sh
git remote add origin <HTTPS_URL>   # Link a local repository to a remote one
```

### Viewing Remote Repositories
```sh
git remote -v   # Show the linked remote repositories
```

### Pushing Changes to GitHub
```sh
git push -u origin main   # Push changes to the main branch and set upstream tracking
```

### Pulling Changes from GitHub
```sh
git pull origin main   # Fetch and merge changes from the remote main branch
```

### Fetching Remote Changes
```sh
git fetch origin   # Fetch changes from the remote repository without merging
```
