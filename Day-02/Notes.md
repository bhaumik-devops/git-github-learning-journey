# Day 02 - Git Fundamentals Notes


# 1. What is Git?

Git is a Distributed Version Control System (DVCS) used to track changes in source code during software development.

It helps developers collaborate, maintain version history, and restore previous versions whenever required.

---

## Real-World Example

Suppose you are writing a book.

Day 1:
You write Chapter 1.

Day 2:
You add Chapter 2.

Day 3:
By mistake you delete Chapter 1.

Without Git:
Chapter 1 may be lost forever.

With Git:
You can restore the previous version within seconds.

Git works exactly like a save history for your project.

---

## Key Points

- Git tracks every change.
- Git stores project history.
- Git allows collaboration.
- Git helps restore previous versions.
- Git is fast and reliable.


# 2. What is Version Control?

Version Control is a system that records changes to files over time so that you can recall specific versions whenever required.

---

## Real-World Example

Imagine you are writing your resume.

Version 1:
Basic Resume

Version 2:
Added Skills

Version 3:
Added Projects

Version 4:
By mistake, you delete all your projects.

Without Version Control:
You have to recreate everything manually.

With Version Control:
You can restore Version 3 within seconds.

---

## Why is Version Control Important?

- Keeps complete project history.
- Allows multiple developers to work together.
- Helps recover deleted or modified files.
- Makes collaboration easy.
- Reduces the risk of losing work.

---

## Key Points

- Tracks every change.
- Stores previous versions.
- Makes teamwork easier.
- Prevents accidental data loss.
- Essential for software development.


# 3. Why Git Was Created?

Git was created by Linus Torvalds in 2005 to efficiently manage the development of the Linux Kernel.

It was designed to be fast, distributed, secure, and capable of handling large software projects.

---

## Why Git Became Popular?

- Very Fast
- Free and Open Source
- Distributed Version Control System
- Supports Team Collaboration
- Highly Reliable
- Used by millions of developers worldwide

---

## Key Points

- Created by Linus Torvalds.
- Released in 2005.
- Developed for the Linux Kernel.
- Fast, Secure and Distributed.
- Most popular Version Control System today.


# 4. Git vs GitHub

Git is a Distributed Version Control System used to track changes in files.

GitHub is a cloud-based hosting platform for Git repositories that enables collaboration and remote storage.

---

## Real-World Example

Suppose you have a notebook.

Git is like writing and maintaining all the versions of that notebook.

GitHub is like storing that notebook safely in an online locker so that you can access it from anywhere and share it with others.

---

## Difference Between Git and GitHub

| Git | GitHub |
|------|---------|
| Version Control System | Cloud Hosting Platform |
| Works locally | Works online |
| Tracks changes | Stores repositories |
| No internet required for most operations | Internet required |

---

## Key Points

- Git and GitHub are different.
- Git can work without GitHub.
- GitHub uses Git.
- GitHub helps in collaboration and backup.


## Interview Questions

### Q1. What is Git?

Git is a Distributed Version Control System used to track changes in source code.

---

### Q2. What is GitHub?

GitHub is a cloud-based platform used to host Git repositories.

---

### Q3. What is the difference between Git and GitHub?

Git is a Version Control System.

GitHub is an online hosting platform for Git repositories.

---

### Q4. Can Git work without GitHub?

Yes.

Git works perfectly on a local computer without GitHub.


# 5. Repository

A Repository is a storage location where all project files, folders, and Git history are maintained.

Repositories can be Local or Remote.

---

## Types of Repository

### Local Repository

Stored on your computer.

### Remote Repository

Stored on GitHub or another Git hosting service.

---

## Real-World Example

Imagine you have a cupboard.

Inside the cupboard, you keep:

- Documents
- Files
- Books
- Notes

Everything is stored in one place.

A Git Repository works in the same way.

It stores all your project files and their history.

---

## Key Points

- Repository stores project files.
- Repository stores commit history.
- Can be Local or Remote.
- Every Git project has a repository.


# 6. Working Directory

The Working Directory is the folder where you actively create, modify, or delete project files.

These changes are not part of Git history until they are staged and committed.

---

## Real-World Example

Imagine you are writing notes in a notebook.

While writing, the notebook is your Working Directory.

Nothing is permanently recorded in Git until you save your work as a commit.

---

## Key Points

- Current working folder.
- Create and edit files here.
- Git detects changes.
- Changes are not committed yet.


# 7. Staging Area

The Staging Area is an intermediate area where you prepare changes before creating a commit.

Git commits only the files that are added to the staging area.

---

## Real-World Example

Imagine you are sending documents through a courier.

Working Directory = Documents on your desk.

Staging Area = Documents placed inside the courier envelope.

Commit = Courier dispatched.

---

## Key Points

- Temporary area before commit.
- Files are added using `git add`.
- Only staged files are committed.
- Gives you control over what gets committed.

# 8. Commit

A Commit is a permanent snapshot of your staged changes in the Git repository.

Each commit represents a specific version of your project.

---

## Real-World Example

Imagine writing a book.

After completing one chapter, you save it as "Chapter 1 Completed".

That saved version is similar to a Git Commit.

---

## Key Points

- Permanent snapshot of changes.
- Created using `git commit`.
- Every commit has a unique ID.
- Helps restore previous versions.


# 9. HEAD

HEAD is a pointer that refers to the current (latest) commit in your Git repository.

Whenever a new commit is created, HEAD automatically points to that commit.

---

## Real-World Example

Imagine you are reading a book.

You place a bookmark on the page you are currently reading.

That bookmark is like HEAD.

When you move to the next page, the bookmark also moves.

Similarly, when you create a new commit, HEAD moves to the latest commit.

---

## Key Points

- HEAD is a pointer.
- It points to the latest commit.
- Moves automatically after every new commit.
- Represents your current working version.