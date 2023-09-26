# GitHub Flow <!-- omit in toc -->

## Table of Contents <!-- omit in toc -->

- [1. Overview](#1-overview)
- [2. Branches](#2-branches)
- [3. Flow](#3-flow)
  - [3.1 Initialize a new project](#31-initialize-a-new-project)
  - [3.2 Developer role](#32-developer-role)
  - [3.3 Good practices](#33-good-practices)
- [4. Pros](#4-pros)
- [5. Cons](#5-cons)
- [6. References](#6-references)

## 1. Overview

![GitHub Flow Branching Strategy](../../resources/git-strategies-github-flow-graph.jpg "GitHub Flow Branching Strategy")

## 2. Branches

- **main**
  - long-lived
  - developer MUST NOT use force push on this branch
  - developer MUST open a pull request to add changes to this branch
  - developer MUST merge only stable features to this branch
- **feature**
  - short-lived
  - branches off the **main** branch
  - one developer at a time on a branch
  - develop new features

## 3. Flow

### 3.1 Initialize a new project

1. Create a new repository with the **main** branch as default.

### 3.2 Developer role

1. Create a new **feature** or **bugfix** branch from **main** following naming conventions available [here](../naming.md).
2. . Start working on the feature or bugfix.
3. Rebase the branch onto **main** before creating a pull request to merge it into **main** (avoid unnecessary merge commits).
4. Bump version and update release notes when ready (if applicable).
5. Merge this branch into **main** after peer review.
6. Add a release tag.
7. Delete the **feature** or **bugfix** branch.

### 3.3 Good practices

- Commit often and push frequently.
- Protect the long-lived branches.
- **Delete the feature / bugfix branch once done**: this indicates that the work on the branch is complete and prevents you or others from accidentally using old branches.
- Whenever possible assign the merge request to the person who knows most about the codebase you are changing.
- Reopening an issue means creating a new feature branch with the same name and a new merge request.

## 4. Pros

- CI/CD friendly
- simpler alternative to GitFlow
- fast and streamlined branching strategy
- short production cycles and frequent releases
- fast feedback loops so teams can quickly identify issues and resolve them
- ideal for small teams and web applications since there is no need to manage multiple versions

## 5. Cons

- not suitable for handling multiple versions of the code
- unstable production code if branches are not properly tested before merging
- lack of development branch, and consequently more susceptible to bugs
- lack of transparency meaning developers cannot see what other developers are working on

## 6. References

General:
- https://www.flagship.io/git-branching-strategies/
- https://docs.github.com/en/get-started/quickstart/github-flow
- https://scottchacon.com/2011/08/31/github-flow.html

GitHub default branch master to main:
- https://github.com/github/renaming
