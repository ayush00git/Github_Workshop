# git-commands

# Basic Git Commands

## 📂 Initialize Repository

```bash
git init
```

## ⬇️ Clone Repository

```bash
git clone <repo_url>
```

## 📊 Check Status

```bash
git status
```

## ➕ Add Changes

```bash
git add <file>
git add .
```

## 📝 Commit Changes

```bash
git commit -m "your message"
```

## 📜 View History

```bash
git log
```

## 🌿 Branches

```bash
git branch <branch_name>
git checkout <branch_name>
git checkout -b <branch_name>
```

## 🔀 Merge Branches

```bash
git checkout main
git merge <branch_name>
```

## ☁️ Push to Remote

```bash
git push origin <branch_name>
```

## ⬆️ Pull from Remote

```bash
git pull origin <branch_name>
```

✅ These are the essential Git commands you’ll use daily!

## 🔄 Pull Changes with Rebase

Sometimes, when you’re working on a branch, you want to **update your local branch with remote changes** but keep a **clean linear history**.

This is where `git pull --rebase` is useful.

### ✅ Commands:

```bash
# Switch to your branch
git checkout <branch_name>

# Pull latest changes from remote and rebase
git pull --rebase origin <branch_name>

```

## ⚡ Advanced Commands

### Stash changes temporarily

```bash
git stash          # Save current changes
git stash pop      # Apply the stashed changes back
git stash list     # See all stashed changes

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

### Undo last commit (keep changes)

```bash
git reset --soft HEAD~1

```

### View differences

```bash
git diff          # See unstaged changes
git diff --staged # See staged changes

```

### Tag a release

```bash
git tag -a v1.0 -m "Release version 1.0"
git push origin v1.0

```

> 💡 Tip: For beginners, the basic commands are enough. Advanced commands help in collaborative workflows and keeping your history clean.
