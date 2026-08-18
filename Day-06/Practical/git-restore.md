# git restore Practical

## Command

git restore Day-06/Notes.md

## Purpose

The `git restore` command discards unstaged changes in a tracked file and restores the file to its last committed state.

## Practical Test

A temporary line was added to:

Day-06/Notes.md

The change was verified using:

git diff

The output showed:

+TEMPORARY RESTORE TEST

The change was then discarded using:

git restore Day-06/Notes.md

## Verification

After running `git restore`, `git diff` produced no output.

`git status` also showed that `Day-06/Notes.md` was no longer modified.

The temporary test file was then deleted.

Final result:

nothing to commit, working tree clean

## Learning

`git restore <file>` discards unstaged changes from the working directory and restores the file to its last committed version.

Important:

`git restore --staged <file>` is different. It removes a file from the staging area while keeping its working-directory changes.