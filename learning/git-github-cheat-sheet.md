# Git and GitHub Cheat Sheet

Quick reference for Odin Project practice.

## Daily flow

```bash
git status
git checkout -b feature/my-task
git add .
git commit -m "Add my task"
git push -u origin feature/my-task
```

## Common commands

| Command | What it does |
| --- | --- |
| `git status` | Shows what changed |
| `git diff` | Shows unstaged changes |
| `git diff --staged` | Shows staged changes |
| `git add <file>` | Stage one file |
| `git add .` | Stage all current changes |
| `git commit -m "message"` | Save a commit |
| `git log --oneline` | Show commit history |
| `git branch` | List branches |
| `git checkout -b <name>` | Create and switch to a branch |
| `git switch <name>` | Switch branches |
| `git push` | Send commits to GitHub |
| `git pull` | Download remote changes |

## Branching

```bash
git checkout -b fix/navbar-spacing
```

Good branch names:

- `feature/signup-form`
- `fix/footer-alignment`
- `docs/git-notes`

## Commit examples

```bash
git commit -m "Add signup form validation"
git commit -m "Fix navigation hover state"
git commit -m "Update GitHub notes"
```

## Reviewing before commit

```bash
git status
git diff
git add .
git diff --staged
git commit -m "Describe the change"
```

## Undo basics

```bash
git restore <file>
git restore --staged <file>
```

- `git restore <file>` removes unstaged changes in that file.
- `git restore --staged <file>` unstages a file but keeps the edits.

## GitHub tips

- Push your branch with:

```bash
git push -u origin <branch-name>
```

- Open a pull request when you want to merge or ask for feedback.
- Add a short PR description that explains:
  - what changed
  - why it changed
  - how you tested it

## Quick reminders

- `git status` before you commit.
- `git diff` before you stage.
- Small commits are easier to understand.
- Push often so your work is safe.
