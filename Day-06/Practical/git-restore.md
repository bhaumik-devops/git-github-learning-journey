# git restore Practical

## Command

git restore Day-06/Notes.md

## Purpose

The `git restore` command discards unstaged changes in a tracked file and restores the file to its last committed state.

## Practical Test

A temporary change was added to:

Day-06/Notes.md

The change was checked using:

git diff

The diff showed the temporary change.

The change was then discarded using:

git restore Day-06/Notes.md

## Verification

After running `git restore`:

- `git diff` produced no output.
- `Day-06/Notes.md` was no longer modified.
- The temporary test file was deleted.
- `git status` showed a clean working tree.

Final status:

nothing to commit, working tree clean

## Important Difference

`git restore <file>` discards unstaged changes in the working directory.

`git restore --staged <file>` removes a file from the staging area while keeping its working-directory changes.

## Learning

I learned how to safely identify and discard an unwanted unstaged change using `git restore`.