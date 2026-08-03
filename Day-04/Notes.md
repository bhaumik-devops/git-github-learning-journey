# Day-04 - Git Merge Conflicts

# 1. What is a Merge Conflict?

A merge conflict occurs when Git is unable to automatically combine changes from two branches.

The developer must manually decide which changes should be kept.

---

## Real World Example

Suppose two developers edit the same line in README.md.

Developer A changes:

Version 1.0

Developer B changes:

Version 2.0

Git cannot decide which version is correct.

Therefore, Git reports a Merge Conflict.

---

## Interview Question

Q. What is a Merge Conflict?

Answer:

A Merge Conflict occurs when Git cannot automatically merge changes because the same file or the same lines were modified differently in multiple branches.


# 2. Why Do Merge Conflicts Happen?

A merge conflict happens when Git cannot automatically combine changes from different branches.

This usually occurs when multiple developers modify the same file or the same lines differently.

---

## Common Reasons

- Two developers edit the same line.
- One developer deletes a file while another edits it.
- Different changes are made to the same section of a file.
- A branch is outdated before merging.

---

## Real World Example

Developer A changes:

Project Version: 1.0

Developer B changes:

Project Version: 2.0

Both edited the same line.

Git cannot decide which version should remain.

Therefore, a Merge Conflict occurs.

---

## Important Points

- Merge Conflicts are normal.
- They are not Git errors.
- Developers resolve them manually.
- After resolving, the merge can continue successfully.

---

## Interview Question

Q. Why do Merge Conflicts happen?

Answer:

Merge Conflicts happen when Git cannot automatically merge changes because the same file or the same lines were modified differently in multiple branches.


# 3. Types of Merge Conflicts

## Common Types of Merge Conflicts

### 1. Same Line Conflict

Be developers ek j file ni ek j line ne alag rite modify kare.

Aa sauthi common merge conflict che.

---

### 2. Modify/Delete Conflict

Ek developer file modify kare che.

Bijo developer e j file delete kari de che.

Git ne khabar padti nathi ke file rakhvi ke delete karvi.

---

### 3. Rename Conflict

Ek developer file nu naam badle che.

Bijo developer e j file edit kare che.

Git conflict report kari shake che.

---

### 4. Add/Add Conflict

Be developers same name ni navi file create kare.

Example:

config.txt

Banney branch ma create thay che.

Git manually resolve karva kahe che.

---

## Real World Example

Developer A:

README.md

Version 1.1

Developer B:

README.md

Version 2.0

Git cannot decide which version should remain.

Conflict occurs.

---

## Summary

Merge Conflicts generally happen because:

- Same line edited
- File deleted and modified
- File renamed
- Same file added differently

---

## Interview Question

Q. What are the common types of Merge Conflicts?

Answer:

The most common Merge Conflicts are:

- Same Line Conflict
- Modify/Delete Conflict
- Rename Conflict
- Add/Add Conflict


## Practical Observation

During this practical, I intentionally created a merge conflict between two branches.

Git displayed conflict markers because both branches contained different versions of the same file.

I manually resolved the conflict by choosing the required content, removed the conflict markers, staged the file using `git add`, and completed the merge with a new commit.

This practical helped me understand how Git handles merge conflicts in real-world software development.


# Interview Questions

### Q1. What is a Merge Conflict?

### Q2. Why do Merge Conflicts occur?

### Q3. How do you resolve a Merge Conflict?

### Q4. What are conflict markers in Git?

### Q5. What is the difference between Fast-forward Merge and a Merge Conflict?

### Q6. What is an Add/Add Conflict?

### Q7. Can Git resolve every Merge Conflict automatically?

### Q8. What should you do after resolving a Merge Conflict?

### Q9. Which command stages a resolved conflict?

### Q10. Which command completes the merge after resolving the conflict?