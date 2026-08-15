# Day-06 — Git Diff & Change Management


🎯 Day-06 Objective

The objective of Day-06 is to understand how Git tracks changes between the working directory, staging area, and the last committed version.

The commands practiced so far are:

git diff
git diff --staged
git restore --staged

1. Understanding Git Change Areas

Git mainly works with three important areas:

Working Directory

The working directory contains the files that we are currently working on.

When we modify a tracked file, the changes initially exist in the working directory.

Staging Area

The staging area contains changes that have been selected for the next commit.

We move changes from the working directory to the staging area using:

git add <file-name>

Repository

The repository contains the committed version of the project.

Basic workflow:

Working Directory
      ↓
   git add
      ↓
 Staging Area
      ↓
  git commit
      ↓
  Repository

2. git diff

The git diff command shows the changes in tracked files that have not yet been staged.

Syntax

git diff

Example

After modifying a tracked file, run:

git diff

Git displays the differences between the current working version and the last committed version.

Important Symbols

+ = Added line

- = Removed line

For example:

+Today I started learning git diff.

The + means that this line was added.

Real-World Use

Developers use git diff before staging changes to review exactly what they have modified.

This helps prevent accidental or unwanted changes from being committed.

3. git diff --staged

The git diff --staged command shows the changes that have already been added to the staging area.

Syntax

git diff --staged

Example Workflow

First modify a tracked file:

Day-05/Notes.md

Then stage it:

git add Day-05/Notes.md

Now the change is in the staging area.

Run:

git diff --staged

Git displays the changes that are currently staged and ready to be committed.

Real-World Use

Developers commonly use git diff --staged immediately before committing.

It answers the question:

"What exactly am I about to commit?"

4. git diff vs git diff --staged
Command	Shows
git diff	Unstaged changes
git diff --staged	Staged changes
Simple Understanding
Working Directory
      ↓
  git diff
      ↓
Unstaged Changes


Working Directory
      ↓
   git add
      ↓
 Staging Area
      ↓
git diff --staged
      ↓
 Staged Changes

5. git restore --staged

The git restore --staged command removes a file from the staging area without deleting the changes from the working directory.

Syntax

git restore --staged <file-name>

Example

git restore --staged Day-05/Notes.md

What Happened in Our Practical

We staged Day-05/Notes.md using:

git add Day-05/Notes.md

Then we checked the staged changes using:

git diff --staged

After reviewing the changes, we used:

git restore --staged Day-05/Notes.md

This removed the file from the staging area, but the changes remained in the working directory.

Important Point

git restore --staged does NOT delete the changes.

It only moves the file:

Staging Area
      ↓
Working Directory

6. Practical Learning

During today's practical session:

We modified a tracked file.
We used git diff to inspect unstaged changes.
We staged a file using git add.
We used git diff --staged to inspect staged changes.
We used git restore --staged to remove the file from the staging area.
We verified the repository state using git status.

This helped us understand the difference between the working directory and staging area.

🎯 Day-06 Progress
Completed
 git diff
 git diff --staged
 git restore --staged
 Working Directory concept
 Staging Area concept
 Difference between unstaged and staged changes
Remaining
 git show
 git restore
 git rm
 git mv



 ## 7. git show

The `git show` command displays detailed information about a specific Git commit.

It can show:

- Commit ID
- Author
- Date
- Commit message
- Files changed
- Actual changes made in the commit

### Syntax

git show <commit-hash>

### Example

git show 60a30d9

In our practical session, `60a30d9` was the latest commit.

The command displayed:

- The full commit hash
- Author information
- Commit date
- Commit message
- Files modified by the commit
- The actual content changes

### Example Output

    commit 60a30d92616b7ae866e4ad18207e5decb44e7404
    Author: Bhaumik Dhebar
    Date: Fri Aug 14 22:46:01 2026 +0530

        Document git diff and staging commands

The output then displayed the changes made to `Day-06/Commands.md` and `Day-06/Notes.md`.

### Using git show Without a Commit Hash

The latest commit can also be inspected using:

git show

Git automatically uses `HEAD`, which represents the currently checked-out commit.

### Short Commit Hash

Git allows us to use a shortened commit hash when it uniquely identifies a commit.

Example:

git show 60a30d9

instead of using the complete SHA-1 hash.

### Real-World Use

Developers use `git show` to investigate what exactly changed in a particular commit.

It is useful for:

- Reviewing previous work
- Investigating bugs
- Checking configuration changes
- Understanding who made a change
- Reviewing changes before troubleshooting

### Important Difference

`git log --oneline` mainly shows commit history.

`git show <commit-hash>` shows detailed information and the actual changes for a specific commit.

### Simple Understanding

    git log --oneline
            ↓
    Find a commit
            ↓
    git show <commit-hash>
            ↓
    Inspect that commit