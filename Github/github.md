# Git & GitHub Commands Handbook

> **Author:** Sakshi Shewale
>
> This file contains all the important Git and GitHub commands that I learn during my Full Stack Development Journey. The purpose of this document is to help me revise Git concepts before interviews and while working on projects.

---

# What is Git?

Git is a **Version Control System (VCS)** used to track changes in source code. It allows developers to save different versions of a project, collaborate with others, and restore previous versions whenever required.

---

# What is GitHub?

GitHub is a cloud-based platform that hosts Git repositories. It allows developers to store code online, collaborate with team members, manage projects, and showcase their work.

---

# Git Workflow

Working Directory
        ↓
Staging Area
        ↓
Local Repository
        ↓
Remote Repository (GitHub)

---

# 1. Check Git Version

```bash
git --version
```

### Purpose

Checks whether Git is installed on the computer and displays the installed version.

---

# 2. Initialize a Repository

```bash
git init
```

### Purpose

Creates a new Git repository inside the current project folder.

### When to Use

Run only once when starting a new project.

---

# 3. Check Repository Status

```bash
git status
```

### Purpose

Shows:

- Current branch
- Modified files
- Untracked files
- Files ready to commit

### When to Use

Use frequently while working.

---

# 4. Add All Files

```bash
git add .
```

### Purpose

Adds all modified and new files to the Staging Area.

---

# 5. Add a Specific File

```bash
git add filename
```

Example

```bash
git add README.md
```

### Purpose

Stages only the specified file.

---

# 6. Commit Changes

```bash
git commit -m "Initial project structure"
```

### Purpose

Creates a snapshot of the staged files.

### Good Commit Message Examples

```text
Added HTML Introduction notes

Completed HTML Forms

Built Portfolio Homepage

Added JavaScript Arrays examples
```

Avoid messages like:

```text
Done

Update

Final

Hello
```

---

# 7. Rename Branch to Main

```bash
git branch -M main
```

### Purpose

Changes the current branch name to `main`.

---

# 8. Connect Local Repository to GitHub

```bash
git remote add origin https://github.com/username/repository-name.git
```

### Purpose

Connects the local project with the remote GitHub repository.

---

# 9. Verify Remote Repository

```bash
git remote -v
```

### Purpose

Displays the connected remote repositories.

Example Output

```text
origin https://github.com/username/repository.git (fetch)

origin https://github.com/username/repository.git (push)
```

---

# 10. Push Code to GitHub

```bash
git push -u origin main
```

### Purpose

Uploads the local repository to GitHub.

`-u` sets the upstream branch for future pushes.

---

# 11. Push Latest Changes

```bash
git push
```

### Purpose

Uploads newly committed changes.

---

# 12. Download Latest Changes

```bash
git pull
```

### Purpose

Downloads and merges the latest changes from GitHub.

---

# 13. Clone an Existing Repository

```bash
git clone repository-url
```

Example

```bash
git clone https://github.com/username/project.git
```

### Purpose

Downloads an existing GitHub repository to the local computer.

---

# 14. View Commit History

```bash
git log
```

### Purpose

Displays all commits made in the repository.

---

# 15. Short Commit History

```bash
git log --oneline
```

### Purpose

Displays commits in a concise format.

---

# 16. Remove a File from Staging Area

```bash
git restore --staged filename
```

### Purpose

Removes a staged file without deleting it.

---

# 17. Restore a Deleted File

```bash
git restore filename
```

### Purpose

Restores the file to the last committed version.

---

# Git Workflow Summary

Create or Modify Files

↓

git status

↓

git add .

↓

git commit -m "Meaningful message"

↓

git push

---

# Best Practices

- Write meaningful commit messages.
- Commit regularly after completing logical tasks.
- Pull the latest changes before starting work on a shared project.
- Never upload sensitive information such as passwords or API keys.
- Keep your README.md updated.
- Organize repositories with a clear folder structure.

---

# Interview Questions

### What is Git?

Git is a distributed version control system that tracks changes in source code.

---

### What is GitHub?

GitHub is a cloud platform for hosting Git repositories.

---

### Difference Between Git and GitHub

| Git | GitHub |
|------|---------|
| Version Control System | Cloud Hosting Platform |
| Works Locally | Works Online |
| Tracks Changes | Stores Repositories |

---

### What is a Repository?

A repository is a storage location that contains the project files along with their complete version history.

---

### What is a Commit?

A commit is a saved snapshot of the project at a particular point in time.

---

### What is the Staging Area?

The staging area is an intermediate area where selected changes are prepared before creating a commit.

---

# Daily Git Workflow

1. Open Project
2. Make Changes
3. Check Status
4. Stage Files
5. Commit Changes
6. Push to GitHub

---

# Commands to Remember

```bash
git init

git status

git add .

git commit -m "message"

git branch -M main

git remote add origin URL

git push -u origin main

git push

git pull

git log
```

---

**Last Updated:** August 2026