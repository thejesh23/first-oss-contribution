# Git Cheat Sheet

The commands you'll actually use to make a contribution, in order.

## Glossary

- **Fork** — your own copy of someone else's repo, on your GitHub account.
- **Clone** — downloading a repo (or your fork of it) to your computer.
- **Origin** — the default name for the remote you cloned from (usually your fork).
- **Upstream** — the original repo you forked from, not your fork.
- **Branch** — a separate line of work, so you never commit straight to `main`.
- **Commit** — a saved snapshot of your changes with a message.
- **Pull request (PR)** — a request asking the original repo to pull in your commits.

## Commands

```bash
# Copy a repo to your machine
git clone https://github.com/YOUR-USERNAME/REPO.git

# See what's changed / staged
git status

# Create and switch to a new branch
git checkout -b my-branch-name

# Stage a specific file
git add path/to/file

# Save a snapshot with a message
git commit -m "short description of the change"

# Send your branch to your fork on GitHub
git push origin my-branch-name

# Add the original repo as a second remote (do this once, after cloning your fork)
git remote add upstream https://github.com/ORIGINAL-OWNER/REPO.git

# Pull the latest changes from the original repo into your local main
git checkout main
git fetch upstream
git rebase upstream/main

# See your commit history
git log --oneline
```

## Typical flow for one contribution

```bash
git checkout main
git fetch upstream
git rebase upstream/main        # stay in sync with the original repo
git checkout -b my-fix
# ... make changes ...
git add -A
git commit -m "fix: describe the change"
git push origin my-fix
# then open a PR on GitHub
```
