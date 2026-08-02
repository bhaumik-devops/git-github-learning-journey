# Day-03 - Git Branching

# 1. What is a Git Branch?

A Git branch is an independent line of development that allows developers to work on new features, bug fixes, or experiments without affecting the main branch.

---

## Real World Example

Suppose tame Amazon ma DevOps Engineer cho.

Main branch:

Production Website

Developer A:

Feature Login

Developer B:

Payment Gateway

Developer C:

Dark Mode

Badha alag branches par kaam kare che.

Feature complete thay pachi branch ne main ma merge karvama aave che.

---

## Important Points

- Branch creates an isolated environment.
- Main code remains safe.
- Multiple developers can work simultaneously.
- Easy to merge after completion.

---

## Interview Question

Q. What is a Git Branch?

Answer:

A Git branch is an independent line of development used to develop features, fix bugs, or experiment without affecting the main branch.


# 2. Why do We Use Branches?

Git branches allow developers to work independently without affecting the main branch.

Branches are mainly used for:

- Developing new features
- Fixing bugs
- Testing new ideas
- Collaborating with team members

---

## Benefits

- Keeps the main branch stable.
- Safe experimentation.
- Easy collaboration.
- Easy rollback if something goes wrong.
- Multiple developers can work at the same time.

---

## Real World Example

Imagine a banking application.

Developer A is working on Login Feature.

Developer B is fixing a Payment Bug.

Developer C is developing Notifications.

If everyone works directly on the main branch, their changes may interfere with each other.

Instead, each developer creates a separate branch.

After testing, all branches are merged into the main branch.

---

## Interview Question

Q. Why do developers use Git branches?

Answer:

Developers use Git branches to work independently on new features, bug fixes, or experiments without affecting the main branch. After testing, the changes are merged into the main branch.


# 3. Main Branch vs Feature Branch

## What is Main Branch?

The Main Branch is the primary and stable branch of a Git repository.

It usually contains the production-ready and tested code.

Developers should avoid making direct changes to the main branch.

---

## What is Feature Branch?

A Feature Branch is a temporary branch created from the main branch to develop a new feature, fix a bug, or test an idea.

Once the work is completed and tested, it is merged back into the main branch.

---

## Comparison

| Main Branch                    | Feature Branch |
|--------------------------------|----------------|
| Stable code                    | Development code |
| Production ready               | Work in progress |
| Shared by everyone             | Used by individual developers |
| Protected branch               | Temporary branch |

---

## Workflow

Main Branch

↓

Create Feature Branch

↓

Develop Feature

↓

Test

↓

Merge into Main Branch

---

## Example

Main Branch

↓

feature-login

↓

Add Login Functionality

↓

Testing

↓

Merge into Main

---

## Interview Question

Q. What is the difference between the Main branch and a Feature branch?

Answer:

The Main branch contains stable and production-ready code, whereas a Feature branch is used to develop new features or fix bugs without affecting the Main branch.


# 4. Git Branch Workflow

A Git Branch Workflow is a standard development process where developers create a separate branch for every new feature, bug fix, or experiment.

After development and testing, the branch is merged back into the Main branch.

---

## Standard Workflow

1. Clone the repository.
2. Create a new branch.
3. Switch to the new branch.
4. Develop the feature.
5. Commit the changes.
6. Test the feature.
7. Merge the branch into Main.
8. Push the updated Main branch to GitHub.

---

## Workflow Diagram

Main Branch

↓

Create Feature Branch

↓

Develop Feature

↓

Commit Changes

↓

Testing

↓

Merge into Main

↓

Push to GitHub

---

## Real World Example

Project:

Online Shopping Website

Main Branch

↓

feature-cart

↓

Add Shopping Cart

↓

Testing

↓

Merge into Main

↓

Deploy to Production

---

## Advantages

- Safe Development
- Easy Team Collaboration
- Stable Production Code
- Easy Bug Fixes
- Better Code Review

---

## Interview Question

Q. Explain the Git Branch Workflow.

Answer:

The Git Branch Workflow starts by creating a new branch from the Main branch. Developers work on the feature, commit their changes, test the code, and finally merge the branch back into the Main branch after successful testing.


## Practical Observation

During the practical, I created a file named `login-feature.txt` inside the `feature-login` branch.

When I switched to the `main` branch, the file disappeared because it was not part of the `main` branch.

When I switched back to the `feature-login` branch, the file appeared again.

This practical proved that every Git branch has its own independent snapshot of the project.