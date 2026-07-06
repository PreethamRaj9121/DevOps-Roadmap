# 🚀 Git Interview Questions & Cheat Sheet

A practical collection of Git interview questions, commands, and real-world scenarios for DevOps Engineers.

⭐ Star this repository if it helped you.

---

# 📚 Table of Contents

- Git Basics
- Common Git Commands
- Git Interview Questions
- Branching
- Merge & Rebase
- Reset vs Revert
- Real DevOps Scenarios

---

# 🌿 Git Basics

## What is Git?

Git is a distributed version control system used to track changes in source code and collaborate with teams.

---

## Difference Between Git and GitHub?

**Git**
- Version Control System

**GitHub**
- Cloud platform to host Git repositories

---

# 🚀 Must Know Git Commands

## Clone Repository

```bash
git clone <repository-url>
```

---

## Check Repository Status

```bash
git status
```

---

## Stage Files

```bash
git add .
```

---

## Commit Changes

```bash
git commit -m "Initial Commit"
```

---

## Push Changes

```bash
git push origin main
```

---

## Pull Latest Changes

```bash
git pull origin main
```

---

## View Commit History

```bash
git log --oneline
```

---

## Check Branches

```bash
git branch
```

---

## Create New Branch

```bash
git checkout -b feature-login
```

---

## Switch Branch

```bash
git checkout main
```

---

## Merge Branch

```bash
git merge feature-login
```

---

## Delete Branch

```bash
git branch -d feature-login
```

---

# 🎯 Git Interview Questions

## 1. What is Git?

Git is a distributed version control system used to track code changes.

---

## 2. Difference Between Git and GitHub?

Git is a tool.

GitHub is a hosting platform for Git repositories.

---

## 3. What is a Repository?

A repository stores project files and complete version history.

---

## 4. What is a Commit?

A commit is a snapshot of your code at a specific point in time.

---

## 5. What is a Branch?

A branch is an independent line of development.

---

## 6. Why Do We Create Branches?

To develop features without affecting the main branch.

---

## 7. Difference Between git fetch and git pull?

**git fetch**

- Downloads latest changes
- Doesn't merge

**git pull**

- Downloads
- Automatically merges

---

## 8. Difference Between git merge and git rebase?

**Merge**

- Preserves commit history
- Creates merge commit

**Rebase**

- Creates cleaner linear history
- Rewrites commit history

---

## 9. Difference Between git reset and git revert?

**git reset**

- Removes commits
- Rewrites history

**git revert**

- Creates a new commit to undo changes
- Safe for shared branches

---

## 10. What is HEAD?

HEAD points to the current branch or latest commit.

---

## 11. What is Origin?

Origin is the default remote repository.

---

## 12. What is Staging Area?

Temporary area before committing code.

---

## 13. What Causes Merge Conflicts?

When multiple developers modify the same lines of code.

---

## 14. How Do You Resolve Merge Conflicts?

1. Open conflicting file
2. Resolve conflicts
3. git add .
4. git commit

---

## 15. Difference Between Fork and Clone?

Fork

- Creates your own copy on GitHub

Clone

- Downloads repository locally

---

# 🔥 Real DevOps Scenarios

## Scenario 1

You committed to the wrong branch.

Solution:

```bash
git cherry-pick
```

or

```bash
git reset
```

---

## Scenario 2

You pushed buggy code.

Solution:

```bash
git revert <commit-id>
```

---

## Scenario 3

You accidentally deleted local changes.

Recover using:

```bash
git reflog
```

---

## Scenario 4

Someone force-pushed to main.

Recover using:

```bash
git reflog
```

---

## Scenario 5

Need latest code without overwriting work.

```bash
git stash

git pull

git stash pop
```

---

# ⭐ Most Asked Git Commands

```bash
git clone
git status
git add .
git commit -m
git push
git pull
git fetch
git branch
git checkout
git merge
git rebase
git stash
git stash pop
git log --oneline
git diff
git reset
git revert
git reflog
```

---

# 💡 Pro Tips

✅ Commit small changes frequently

✅ Use meaningful commit messages

✅ Never commit secrets or passwords

✅ Create feature branches for every task

✅ Pull latest changes before pushing

---

⭐ Star this repository if it helped you.

📸 Follow **@devops._raj** for daily DevOps Interview Questions, Projects, Roadmaps & Career Tips.
