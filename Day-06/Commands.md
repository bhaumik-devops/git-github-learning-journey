## 1. git diff

### Purpose

Shows unstaged changes in tracked files.

### Syntax

git diff

### Example

git diff

### Important Point

`git diff` is used to review changes in the working directory before staging them.

`+` indicates an added line.

`-` indicates a removed line.

---

## 2. git diff --staged

### Purpose

Shows changes that have already been added to the staging area and are ready to be committed.

### Syntax

git diff --staged

### Example

git diff --staged

### Important Point

Use this command before committing to review exactly what is currently staged.

---

## 3. git restore --staged

### Purpose

Removes a file from the staging area without deleting its changes from the working directory.

### Syntax

git restore --staged <file-name>

### Example

git restore --staged Day-05/Notes.md

### Important Point

This command unstages the file but keeps the changes in the working directory.

It moves the file from:
Staging Area → Working Directory