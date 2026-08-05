# Day-05 - Git Branch Management & Remote Repository

# 1. What is Branch Management?

Branch Management is the process of creating, organizing, viewing and deleting Git branches.

It is an important part of every Git workflow.

---

## Why is Branch Management Important?

- Keeps the repository clean.
- Removes unused branches.
- Makes collaboration easier.
- Improves project organization.

---

## Interview Question

Q. What is Branch Management?

Answer:

Branch Management is the process of creating, organizing, viewing and deleting Git branches to maintain a clean Git repository.


# 2. Local Branch vs Remote Branch

## What is a Local Branch?

A Local Branch exists only on your computer.

You can create, modify and delete it using Git commands.

Examples:

- main
- feature-login
- feature-payment

---

## What is a Remote Branch?

A Remote Branch exists on GitHub (or another remote Git server).

It is shared with other developers.

Example:

origin/main

---

## Difference

| Local Branch | Remote Branch |
|--------------|---------------|
| Stored on your computer | Stored on GitHub |
| Visible only on your system | Visible to the team |
| Can work offline | Requires synchronization |

---

## Real World Example

Suppose three developers are working on a project.

Developer A creates a branch:

feature-login

Initially it exists only on Developer A's computer.

After running:

git push -u origin feature-login

the branch is uploaded to GitHub.

Now the team can also access it.

---

## Interview Question

Q. What is the difference between a Local Branch and a Remote Branch?

Answer:

A Local Branch exists on the developer's computer, while a Remote Branch exists on GitHub or another remote repository and can be shared with the team.