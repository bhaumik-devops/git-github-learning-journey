# Day-04 Commands

---

## git branch

**Purpose:**
Display all local branches.

```bash
git branch
```

**Example Output:**

```text
* main
  feature-a
  feature-b
  feature-login
```

---

## git switch feature-a

**Purpose:**
Switch to the `feature-a` branch.

```bash
git switch feature-a
```

**Example Output:**

```text
Switched to branch 'feature-a'
```

---

## git switch feature-b

**Purpose:**
Switch to the `feature-b` branch.

```bash
git switch feature-b
```

**Example Output:**

```text
Switched to branch 'feature-b'
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

## git status

**Purpose:**
Display the current status of the repository.

```bash
git status
```

**Example Output:**

```text
On branch main
nothing to commit, working tree clean
```

---

## git add .

**Purpose:**
Stage all modified and new files.

```bash
git add .
```

**Example Output:**

```text
(No output if successful)
```

---

## git commit -m "Add conflict demo file"

**Purpose:**
Create a commit after adding the conflict demo file.

```bash
git commit -m "Add conflict demo file"
```

**Example Output:**

```text
[feature-a 11047a1] Add conflict demo file
```

---

## git commit -m "Update conflict demo file in feature-b"

**Purpose:**
Save the updated version of the conflict demo file in the `feature-b` branch.

```bash
git commit -m "Update conflict demo file in feature-b"
```

**Example Output:**

```text
[feature-b 7bb79c0] Update conflict demo file in feature-b
```

---

## git merge feature-a

**Purpose:**
Merge the `feature-a` branch into the current branch.

```bash
git merge feature-a
```

**Example Output:**

```text
Updating ...
Fast-forward
```

---

## git merge main

**Purpose:**
Merge the `main` branch into the current branch.

```bash
git merge main
```

**Example Output:**

```text
Auto-merging conflict-demo.txt
CONFLICT (add/add): Merge conflict in conflict-demo.txt
Automatic merge failed; fix conflicts and then commit the result.
```

---

## git add conflict-demo.txt

**Purpose:**
Mark the conflicted file as resolved after editing it.

```bash
git add conflict-demo.txt
```

**Example Output:**

```text
(No output if successful)
```

---

## git commit -m "Resolve merge conflict"

**Purpose:**
Complete the merge after resolving the conflict.

```bash
git commit -m "Resolve merge conflict"
```

**Example Output:**

```text
[feature-b 1072a76] Resolve merge conflict
```

---

## git log --oneline --graph --all

**Purpose:**
Display the complete commit history with all branches.

```bash
git log --oneline --graph --all
```

---

## git push origin main

**Purpose:**
Push the latest changes from the local `main` branch to GitHub.

```bash
git push origin main
```

**Example Output:**

```text
To https://github.com/...
main -> main
```