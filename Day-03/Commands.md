# Day-03 Commands

## git branch

**Purpose:**
Display all local branches. The branch marked with `*` is the currently active branch.

```bash
git branch
```

**Example Output:**

```text
* main
  feature-login
```

---

## git branch feature-login

**Purpose:**
Create a new branch named `feature-login`.

```bash
git branch feature-login
```

**Example Output:**

```text
(No output if successful)
```

---

## git switch feature-login

**Purpose:**
Switch from the current branch to the `feature-login` branch.

```bash
git switch feature-login
```

**Example Output:**

```text
Switched to branch 'feature-login'
```

---

## git status

**Purpose:**
Display the current status of the working directory and staging area.

```bash
git status
```

**Example Output:**

```text
On branch feature-login
nothing to commit, working tree clean
```

---

## git add .

**Purpose:**
Stage all modified and new files for the next commit.

```bash
git add .
```

**Example Output:**

```text
(No output if successful)
```

---

## git commit -m "Complete Day-03 Git Branching practical"

**Purpose:**
Save the staged changes with a meaningful commit message.

```bash
git commit -m "Complete Day-03 Git Branching practical"
```

**Example Output:**

```text
[feature-login 72dcecd] Complete Day-03 Git Branching practical
```

---

## git switch main

**Purpose:**
Switch back to the `main` branch.

```bash
git switch main
```

**Example Output:**

```text
Switched to branch 'main'
```

---

## git merge feature-login

**Purpose:**
Merge the `feature-login` branch into the `main` branch.

```bash
git merge feature-login
```

**Example Output:**

```text
Updating ...
Fast-forward
```

---

## git log --oneline --graph --all

**Purpose:**
Display the commit history of all branches in a graphical format.

```bash
git log --oneline --graph --all
```

---

## git push origin main

**Purpose:**
Push the latest changes from the local `main` branch to the GitHub repository.

```bash
git push origin main
```

**Example Output:**

```text
To https://github.com/...
main -> main
```

---

## git branch -d feature-login

**Purpose:**
Delete the local `feature-login` branch after it has been merged successfully.

```bash
git branch -d feature-login
```

**Example Output:**

```text
Deleted branch feature-login (was 72dcecd).
```