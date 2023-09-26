# Naming <!-- omit in toc -->

## Table of Contents <!-- omit in toc -->

- [1. Introduction](#1-introduction)
- [2. Repository](#2-repository)
- [3. Branch](#3-branch)
- [4. Commit](#4-commit)
- [5. Pull requests / Merge requests](#5-pull-requests--merge-requests)
- [6. Miscellaneous](#6-miscellaneous)
- [7. Resources](#7-resources)

## 1. Introduction

List of criteria to match and rules to follow when naming a git object.

## 2. Repository

Criteria:
- Descriptive
- Readable
- Consistent
- Contextual
- Future-friendly
- Extensible
- Reusable
- Brief (short/succinct)

Rules:
- use lower case
- use dashes "-"
- make it as short as possible
- make sure the name is unique
- no camel case
  - problem with camel case is that there are often different interpretations of words
- no underscore "_"
  - "_" is harder to type than "-"
- no spaces
  - no support on certain platforms
  - not practical when working on a local clone

Examples:
- `[customer name]-[product/project name]-[purpose]-[framework/language]`
  - customer-project-api-django
- `[product/project name]-[purpose]-[framework/language]`
  - project-api-flask
- `[product/project name]-[purpose]`
  - project-rest-api
- `[language/framework]-[product/project]`
  - python-automation-scripts

## 3. Branch

Criteria:
- Descriptive
- Contextual
- Brief (short/succinct)

Rules:
- use lower case
- use identifiers from corresponding tickets in an external service if applies
- use personal feature branches and a team-wide feature branch when several people are working on the same feature
- delete your branch from the upstream repository after it's merged

Examples:
- `git checkout -b feature`
- team-wide branch: `git checkout -b feature/main`
- personal branch: `git checkout -b feature/clement`

## 4. Commit

Criteria:
- Descriptive
- Readable
- Contextual
- Future-friendly
- Brief (short/succinct)

Rules:
- use the editor, not the terminal
- order your commits logically
- each commit should be a single logical change
- do not split a single logical change into several commits, the implementation of a feature and the corresponding tests should be together

Example:
- [git commit template](https://github.com/clement-deltel/dotfiles/blob/main/.gitmessage.txt)

## 5. Pull requests / Merge requests

Criteria:
- Descriptive
- Readable
- Contextual
- Future-friendly

Rules:
- keep the history clean and simple
- do not rewrite published history

Good practices:
- rebase your branch onto the branch it's going to be merged to
- squash commits while merging

## 6. Miscellaneous

Rules:
- use annotated tags for marking releases
- use lightweight tags for personal use, such as to bookmark commits
- perform maintenance tasks occasionally:
  - [git-gc](https://git-scm.com/docs/git-gc)
  - [git-prune](https://git-scm.com/docs/git-prune)
  - [git-fsck](https://git-scm.com/docs/git-fsck)

## 7. Resources

- https://moduscreate.com/blog/github-semantic-naming/
- https://github.com/bcgov/BC-Policy-Framework-For-GitHub/blob/master/BC-Gov-Org-HowTo/Naming-Repos.md
- https://github.com/agis/git-style-guide
- https://climbtheladder.com/10-git-repository-naming-best-practices/
