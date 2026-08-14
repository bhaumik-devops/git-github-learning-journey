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