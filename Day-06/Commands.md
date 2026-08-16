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


## 4. git show

### Purpose

Displays detailed information about a specific commit, including the commit metadata and the actual changes introduced by that commit.

### Syntax

git show <commit-hash>

### Example

git show 60a30d9

### Example Without Commit Hash

git show

This displays the latest commit referenced by `HEAD`.

### Important Information Displayed

- Commit hash
- Author
- Date
- Commit message
- Changed files
- Actual code or documentation changes

### Real-World Use

Useful for reviewing a specific commit, investigating changes, troubleshooting issues, and understanding what was changed by a particular developer.

### Difference from git log

`git log` → Shows commit history.

`git show` → Shows detailed information and actual changes for a specific commit.


## 5. git show --stat

### Purpose

Displays a summary of a specific commit, including the changed files and the number of insertions and deletions.

### Syntax

git show --stat <commit-hash>

### Example

git show --stat 629d7ed

### Example Output

    README.md | 7 ++++++-
    1 file changed, 6 insertions(+), 1 deletion(-)

### Meaning

- `1 file changed` → One file was modified.
- `6 insertions(+)` → Six lines were added.
- `1 deletion(-)` → One line was removed.

### Difference from git show

`git show` displays the complete line-by-line changes.

`git show --stat` displays a summary of the changes.

### Real-World Use

Useful when a developer wants a quick overview of the scope of a commit without reviewing the complete diff.