# Git and GitHub Basics - README

This guide provides an overview of basic Git commands and GitHub usage for beginners. It is intended to help users manage and collaborate on projects effectively.

---

## Table of Contents
- [Introduction](#introduction)
- [Installing Git](#installing-git)
- [Configuring Git](#configuring-git)
- [Basic Git Commands](#basic-git-commands)
  - [Creating a Repository](#creating-a-repository)
  - [Cloning a Repository](#cloning-a-repository)
  - [Staging and Committing](#staging-and-committing)
  - [Branching](#branching)
  - [Merging](#merging)
  - [Viewing History](#viewing-history)
- [Pushing to GitHub](#pushing-to-github)
- [Pulling from GitHub](#pulling-from-github)
- [Additional Git Commands](#additional-git-commands)
- [Resources](#resources)

---

## Introduction
Git is a distributed version control system used for tracking changes in source code. GitHub is a web-based hosting service for Git repositories, enabling collaboration and sharing of projects.

---

## Installing Git
1. Download Git from the [official website](https://git-scm.com/).
2. Follow the installation instructions for your operating system.
3. Verify the installation:
   ```bash
   git --version
   ```

---

## Configuring Git
Set your username and email:
```bash
git config --global user.name "Your Name"
git config --global user.email "youremail@example.com"
```

To check the configuration:
```bash
git config --list
```

---

## Basic Git Commands

### Creating a Repository
1. Initialize a new Git repository:
   ```bash
   git init
   ```
2. Create a `.gitignore` file to specify files and directories to ignore.

### Cloning a Repository
Clone an existing repository from GitHub:
```bash
git clone <repository-url>
```

### Staging and Committing
1. Add files to the staging area:
   ```bash
   git add <file-name>
   ```
   To add all changes:
   ```bash
   git add .
   ```
2. Commit the changes:
   ```bash
   git commit -m "Your commit message"
   ```

### Branching
1. Create a new branch:
   ```bash
   git branch <branch-name>
   ```
2. Switch to the branch:
   ```bash
   git checkout <branch-name>
   ```
3. Combine the two steps:
   ```bash
   git checkout -b <branch-name>
   ```

### Merging
1. Switch to the branch you want to merge into (e.g., `main`):
   ```bash
   git checkout main
   ```
2. Merge another branch into it:
   ```bash
   git merge <branch-name>
   ```

### Viewing History
View the commit history:
```bash
git log
```

---

## Pushing to GitHub
1. Add the remote repository:
   ```bash
   git remote add origin <repository-url>
   ```
2. Push the changes to GitHub:
   ```bash
   git push -u origin <branch-name>
   ```

---

## Pulling from GitHub
Fetch and merge changes from the remote repository:
```bash
git pull origin <branch-name>
```

---

## Additional Git Commands
- **Check status**: Shows the working directory and staging area status:
  ```bash
  git status
  ```
- **Undo changes**:
  - Unstage a file:
    ```bash
    git reset <file-name>
    ```
  - Revert a commit:
    ```bash
    git revert <commit-hash>
    ```
- **Delete a branch**:
  ```bash
  git branch -d <branch-name>
  ```

---

## Resources
- [Git Documentation](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com/)
- [Try Git](https://try.github.io/)

---
