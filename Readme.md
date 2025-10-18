## Basic of Git

This repository is the notes,key takeways, and best practices from the video **GitHub Basics Made Easy: A Fast Beginner’s Tutorial** :contentReference[oaicite:1]{index=1}

---

## Contents

- Introduction  
- Key Concepts  
- Common Git Commands  
- Branching & Merging  
- Commit Message Guidelines  
- Workflow & Collaboration  
- Tips & Gotchas  
- References  

---

## Introduction

This tutorial is designed for beginners to understand how Git and GitHub work, why version control is valuable, and how to use them in practice. It helps lay a foundation for collaborating on code in a team environment.

---

## Key Concepts

- **Git vs GitHub**  
  - *Git* is a version control system to track changes locally.  
  - *GitHub* is a hosting service for Git repositories (remote) — lets you share, collaborate, and manage projects.  

- **Repository (repo):** A folder (local or remote) containing your project files tracked by Git.

- **Commit:** A snapshot of changes you’ve made. Each commit gets an identifier (hash).

- **Branch:** A parallel line of development. It allows you to work on changes independently from the main codebase.

- **Merge:** The process of integrating changes from one branch into another (e.g., feature branch → main/master).

- **Remote:** A version of your repository hosted somewhere else (e.g., GitHub). You can fetch, pull, and push changes between your local and remote repos.

- **Pull Request (PR):** A GitHub feature for reviewing and discussing changes before merging into a base branch.

---

## Common Git Commands

Here’s a quick cheat sheet based on what the video covers (and what you should practice):

```bash
# Initialize a local repo
git init

# Check status
git status

# Stage changes for commit
git add <file>        # stage one file
git add .             # stage all changes

# Commit staged changes
git commit -m "Your descriptive message"

# View commit history (on current branch)
git log

# Create a new branch
git branch feature-xyz

# Switch branches
git checkout feature-xyz

# Merge a branch into current branch
git merge feature-xyz

# Delete a branch (once merged)
git branch -d feature-xyz

# Work with remote (GitHub)
git remote add origin <remote-url>
git push -u origin main        # push initial commit to remote
git pull                        # fetch & merge from remote
git push                        # push local commits to remote