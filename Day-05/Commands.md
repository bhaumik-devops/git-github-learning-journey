# Day-05 Commands

## Branch Management

## 1. git branch -a

### Purpose

The `git branch -a` command displays all branches available in the local repository, including local branches and remote-tracking branches.

### Syntax

git branch -a

### Example

git branch -a

### Example Output

  feature-a
  feature-b
  feature-login
* main
  remotes/origin/HEAD -> origin/main
  remotes/origin/main

### How to Understand the Output

- `feature-a`, `feature-b`, `feature-login`, `main`
  → These are local branches.

- `remotes/origin/main`
  → This is a remote-tracking branch representing the `main` branch on the remote repository.

- `*`
  → Indicates the branch currently checked out.

### Real-World Use

A developer can use `git branch -a` to quickly see all local branches and remote-tracking branches before switching branches, creating a branch, or working with a remote repository.

### Interview Question

Q. What is the difference between `git branch` and `git branch -a`?

Answer:

`git branch` displays only local branches, whereas `git branch -a` displays both local branches and remote-tracking branches.

### Practical Status

- [x] Command executed
- [x] Output checked
- [x] Concept understood


## 2. git branch -r

### Purpose

The `git branch -r` command displays only the remote-tracking branches available in the local Git repository.

### Syntax

git branch -r

### Example

git branch -r

### Example Output

  origin/HEAD -> origin/main
  origin/main

### How to Understand the Output

- `origin/main`
  → Represents the remote-tracking reference for the `main` branch on GitHub.

- `origin/HEAD -> origin/main`
  → Indicates that the default branch of the remote repository is `main`.

### Real-World Use

A developer can use `git branch -r` to check which remote branches are currently known to their local Git repository.

For example, before checking out a remote feature branch, a developer can first use:

git branch -r

to see the available remote-tracking branches.

### Interview Question

Q. What does `git branch -r` show?

Answer:

`git branch -r` shows only the remote-tracking branches available in the local Git repository.

### Practical Status

- [x] Command executed
- [x] Output checked
- [x] Concept understood

---

### 3. git remote -v

Purpose:

Syntax:

Example:

Output:

Real World Use:

---

### 4. git remote show origin

Purpose:

Syntax:

Example:

Output:

Real World Use:

---

### 5. git fetch

Purpose:

Syntax:

Example:

Output:

Real World Use:

---

### 6. git fetch --all

Purpose:

Syntax:

Example:

Output:

Real World Use:

---

### 7. git branch -d

Purpose:

Syntax:

Example:

Output:

Real World Use:

---

### 8. git branch -D

Purpose:

Syntax:

Example:

Output:

Real World Use: