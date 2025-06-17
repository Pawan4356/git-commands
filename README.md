# 📘 Git Commands Cheat Sheet

Here are a few Git commands that you may require while building a project.

### 🔧 Setup & Configuration

```bash
git config --global user.name "Your Name"          # Set global username
git config --global user.email "your@email.com"     # Set global email
git config --global core.editor "code"              # Set default editor (VS Code)
git config --list                                    # View current config
```

### 📁 Repository Initialization

```bash
git init                      # Initialize a new Git repo
git clone <url>               # Clone remote repo
```

### 📦 Staging & Committing

```bash
git status                    # Show changes
git add <file>                # Stage file
git add .                     # Stage all changes
git commit -m "message"       # Commit with message
git reset <file>              # Unstage file
git reset --hard              # Undo all changes (DANGEROUS)
```

### 🌿 Branching

```bash
git branch                    # List branches
git branch <name>             # Create branch
git checkout <name>           # Switch to branch
git checkout -b <name>        # Create and switch

# Delete branch
git branch -d <name>          # Delete local
git push origin --delete <name> # Delete remote
```

### 🔀 Merging & Rebasing

```bash
git merge <branch>            # Merge into current
git rebase <branch>           # Rebase onto another
```

### ⬆️ Remote Repositories

```bash
git remote add origin <url>   # Add remote
git remote -v                 # List remotes
git push origin <branch>      # Push branch
git push -u origin <branch>   # Push and track
git pull                      # Pull latest changes
git fetch                     # Fetch changes

# Force push
git push -f origin <branch>
```

### 🕵️‍♂️ Viewing History & Logs

```bash
git log                       # Full commit history
git log --oneline             # One-line format
git diff                      # Show unstaged changes
git diff <branch1> <branch2>  # Compare branches
```

### 🔙 Undoing Changes

```bash
git checkout -- <file>        # Discard changes
git revert <commit>           # Revert commit
git reset --soft HEAD~1       # Undo last commit (keep changes staged)
git reset --hard HEAD~1       # Undo last commit completely
```

### 🧹 Ignore & Cleanup

```bash
# In .gitignore
node_modules/
*.log
venv/
__pycache__/

# Git cleanup
.gitignore                    # Ignore file list
git clean -fd                 # Delete untracked files/folders
git rm --cached <file>        # Remove from git, keep in disk
```

### 🛠️ Maintenance & Optimization

```bash
git gc                        # Cleanup repo
git fsck                      # Check repo integrity
```

---

✅ Use this as a reference while working on your Git projects.

Would you like a PDF version as well?
