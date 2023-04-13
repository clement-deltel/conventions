# Naming

## Table of Contents

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

## 4. Commit

## 5. Pull requests / Merge requests

## Resources

- https://moduscreate.com/blog/github-semantic-naming/
- https://github.com/bcgov/BC-Policy-Framework-For-GitHub/blob/master/BC-Gov-Org-HowTo/Naming-Repos.md
- https://github.com/agis/git-style-guide
