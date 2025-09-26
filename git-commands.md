# git-commands

# Basic Git Commands

## Initialize Repository

```bash
git init
```

## Clone Repository

```bash
git clone <repo_url>
```

## Check Status

```bash
git status
```

## Add Changes

```bash
git add <file>
git add .
```

## Commit Changes

```bash
git commit -m "your message"
```

## View History

```bash
git log
```

## Branches

```bash
git branch <branch_name>
git checkout <branch_name>
git checkout -b <branch_name>
```

## Merge Branches

```bash
git checkout main
git merge <branch_name>
```

## Push to Remote

```bash
git push origin <branch_name>
```

## Pull from Remote

```bash
git pull origin <branch_name>
```

## 🔄 Pull Changes with Rebase

Sometimes, when you’re working on a branch, you want to **update your local branch with remote changes** but keep a **clean linear history**.

This is where `git pull --rebase` is useful.

### Commands:

```bash
# Switch to your branch
git switch <branch_name>

# Pull latest changes from remote and rebase
git pull --rebase origin <branch_name>

```

## ⚡ Advanced Commands

### Stash changes temporarily

```bash
git stash          # Save current changes
git stash pop      # Apply the stashed changes back
git stash list     # See all stashed changes
git stash apply    # Apply changes but keeps them in the list
git stash clear    # deletes all the stash list
```

### Check remote repositories

```bash
git remote -v                       # Show remote URLs
git remote add origin <repo_url>    # Add a new remote

```

### Delete a branch

```bash
git branch -d <branch_name>                  # Delete local branch
git push origin --delete <branch_name>       # Delete remote branch
```