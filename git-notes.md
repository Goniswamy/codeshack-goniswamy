# Git Command Notes

## 1. git init

**Purpose:** Initializes a Git repository.

**Example:**
`git init -b main`

## 2. git status

**Purpose:** Shows the current state of the working directory.

**Example:**
`git status`

## 3. git add

**Purpose:** Stages changes for the next commit.

**Example:**
`git add README.md`

## 4. git commit

**Purpose:** Records staged changes in the repository history.

**Example:**
`git commit -m "Add README"`

## 5. git log

**Purpose:** Displays commit history.

**Example:**
`git log --oneline`

## 6. git diff

**Purpose:** Shows unstaged changes.

**Example:**
`git diff`

## 7. git branch

**Purpose:** Lists branches or creates a branch.

**Example:**
`git branch feature-docs`

## 8. git switch

**Purpose:** Switches to another branch.

**Example:**
`git switch main`

## 9. git merge

**Purpose:** Integrates changes from another branch.

**Example:**
`git merge feature-docs`

## 10. git clone

**Purpose:** Copies a remote repository to your computer.

**Example:**
`git clone https://github.com/USERNAME/REPOSITORY.git`

## 11. git remote

**Purpose:** Displays or configures remote repositories.

**Example:**
`git remote -v`

## 12. git push

**Purpose:** Uploads local commits to a remote repository.

**Example:**
`git push -u origin main`

## 13. git pull

**Purpose:** Fetches and integrates changes from a remote branch.

**Example:**
`git pull origin main`

## 14. git fetch

**Purpose:** Downloads remote updates without merging them into the current branch.

**Example:**
`git fetch origin`

## 15. git show

**Purpose:** Displays details about a commit.

**Example:**
`git show HEAD`


## Practical Example: Saving a Project Change

Suppose I create a new file named `hello.cpp` in my project.

```bash
git status
git add hello.cpp
git commit -m "Add hello world C++ example"
git log --oneline
```

**Explanation:**

- `git status` checks which files have changed.
- `git add hello.cpp` stages the new file.
- `git commit` saves the staged change in Git history.
- `git log --oneline` displays the commit history in a compact format.

This workflow helps me track changes and understand how Git records the progress of a project.


## Working with Git Branches

A branch allows me to work on a new feature or change without directly modifying the main branch.

### Example

```bash
git branch
git switch -c feature/add-login
git status
git add .
git commit -m "Add login feature"
git push -u origin feature/add-login
```

### Explanation

- `git branch` lists the local branches.
- `git switch -c feature/add-login` creates and switches to a new branch.
- `git status` checks the current branch and working-tree changes.
- `git add .` stages changes in the current directory and its subdirectories.
- `git commit` saves the staged changes.
- `git push -u origin feature/add-login` pushes the branch to GitHub and sets its upstream.

**Important:** This is an example workflow. The login feature must actually be implemented before using the example commit message in a real project.