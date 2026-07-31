# Day 02 - Git Commands

## Check Git Version

```bash
git --version
```

### Purpose

Displays the installed Git version.
```

## Initialize a Git Repository

```bash
git init
```

### Purpose

Creates a new Git repository in the current folder.
```

## Check Working Directory Status

```bash
git status
```

### Purpose

Displays the current status of the working directory and staging area.
```
## Add All Files to Staging Area

```bash
git add .
```

### Purpose

Adds all modified and new files to the staging area.

---

## Add a Specific File

```bash
git add filename
```

### Purpose

Adds only the specified file to the staging area.
```

## Create a Commit

```bash
git commit -m "Your commit message"
```

### Purpose

Creates a new commit with the staged changes.

---

## Example

```bash
git commit -m "Added Day 02 Git notes"
```

## View Commit History

```bash
git log
```

### Purpose

Displays the complete commit history. The latest commit is pointed to by HEAD.
```


# Git Commands - Day 02

| Command                           | Description |
|-----------------------------------|--------------------------------------------|
| git status                        | Check the current status of the repository.|
| git add .                         | Add all changes to the staging area. |
| git commit -m "message"           | Create a new commit with a message. |
| git log --oneline                 | Display commit history in one line. |
| git init                          | Initialize a new Git repository. |