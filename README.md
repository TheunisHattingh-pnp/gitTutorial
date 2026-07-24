# Git Tutorial

A hands-on introduction to Git for anyone getting started with version control.

## What is Git?

Git is a **version control system** — it tracks changes to your files over time, so you can:

- See what changed, when, and who changed it
- Go back to an earlier version if something breaks
- Work on the same project as a team without overwriting each other's work

## Setup (do this once)

Tell Git who you are — this stamps your name on every change you make:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

## The core workflow

Most day-to-day Git work is a loop of four commands:

```bash
git status          # What has changed? (run this constantly)
git add <file>      # Stage a change you want to save
git commit -m "..." # Save the staged changes as a snapshot
git push            # Send your commits to the remote (e.g. GitHub)
```

### The three areas to understand

| Area | What it is |
| ---- | ---------- |
| **Working directory** | Your actual files, where you edit |
| **Staging area** | Changes you've marked to include in the next commit (`git add`) |
| **Repository** | The saved history of commits (`git commit`) |

## Essential commands cheat sheet

```bash
git init                 # Start tracking a new project
git clone <url>          # Copy an existing remote project locally
git status               # Show the state of your working directory
git add <file>           # Stage a file (use "git add ." for everything)
git commit -m "message"  # Commit staged changes with a message
git log --oneline        # View commit history, one line each
git diff                 # See unstaged changes
git pull                 # Fetch and merge changes from the remote
git push                 # Upload your commits to the remote
```

## Branches (the next step)

Branches let you work on something without touching the main code:

```bash
git branch feature-x       # Create a branch
git switch feature-x       # Move onto it
# ...make commits...
git switch main            # Go back to main
git merge feature-x        # Bring the changes in
```

## Try it yourself

1. Make a change to this file (add your name below!).
2. Run `git status` to see it flagged.
3. `git add README.md`
4. `git commit -m "Add my name"`
5. `git log --oneline` to see your commit in history.

### People who have completed the exercise

Theunis Hattingh
Cobyn Mulder
Xavier Nunes

## Handy resources

- [Official Git docs](https://git-scm.com/doc)
- [Interactive branching visualizer](https://learngitbranching.js.org/)
- [GitHub's Git cheat sheet (PDF)](https://education.github.com/git-cheat-sheet-education.pdf)
