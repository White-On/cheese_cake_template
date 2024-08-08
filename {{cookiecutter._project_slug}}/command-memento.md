# Git Command Memento

### Initialize a New Repository
```sh
# Initialize a new Git repository
git init
```
### Publish a New Repository for the First Time
```sh
# Create a new repository on GitHub/GitLab/etc.

# Add the remote repository
git remote add origin <repository-url>

# Push the changes to the remote repository
git push -u origin master
```

### Clone an Existing Repository
```sh
# Clone a repository from a remote source
git clone <repository-url>
```

### Configuration
```sh
# Set global username
git config --global user.name "Your Name"

# Set global email
git config --global user.email "your.email@example.com"
```

### Basic Workflow
```sh
# Check the status of your repository
git status

# Add changes to the staging area
git add <file>
# Add all changes
git add .

# Commit changes
git commit -m "Your commit message"

# View commit history
git log
```

### Branching
```sh
# Create a new branch
git branch <branch-name>

# Switch to a branch
git checkout <branch-name>

# Create and switch to a new branch
git checkout -b <branch-name>

# List all branches
git branch

# Delete a branch
git branch -d <branch-name>
```

### Merging
```sh
# Merge a branch into the current branch
git merge <branch-name>
```

### Stashing
```sh
# Stash changes
git stash

# List stashes
git stash list

# Apply the most recent stash
git stash apply

# Apply and drop the most recent stash
git stash pop

# Drop a specific stash
git stash drop <stash@{0}>
```

### Remote Repositories
```sh
# Add a remote repository
git remote add origin <repository-url>

# View remote repositories
git remote -v

# Push changes to a remote repository
git push origin <branch-name>

# Pull changes from a remote repository
git pull origin <branch-name>

# Push tags to a remote repository
git push origin --tags
```

### Tagging
```sh
# Create a new tag
git tag <tag-name>

# Push a tag to a remote repository
git push origin <tag-name>
```

### Undoing Changes
```sh
# Unstage a file
git reset <file>

# Undo the last commit but keep changes
git reset --soft HEAD~1

# Undo the last commit and discard changes
git reset --hard HEAD~1

# Revert a commit by creating a new commit
git revert <commit-hash>
```

### Viewing Differences
```sh
# Show changes in the working directory
git diff

# Show changes between commits
git diff <commit1> <commit2>

# Show changes in a specific file
git diff <file>
```