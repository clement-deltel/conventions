# Repository Structure <!-- omit in toc -->

## Table of Contents <!-- omit in toc -->

- [1. Introduction](#1-introduction)
- [2. Directories](#2-directories)
- [3. Root files](#3-root-files)
  - [3.1 Choose the appropriate license](#31-choose-the-appropriate-license)
- [4. References](#4-references)

## 1. Introduction

List of rules to follow when creating a repository in order to respect a standard structure.

## 2. Directories

- **build/**: scripts related to build process (Dockerfile, docker compose, ...)
- **dep/**: dependency files
- **docs/**: documentation files, alternatively `doc`
- **resources/**: static resources, alternatively `res` (images, ...)
- **src/**: source code files
- **tests/**: automated/integration/unit tests
- **scripts/**: tools and utilities, alternatively `tools`

**.github/** directory (convention directory used to place GitHub related stuff):
- **CONTRIBUTING.md**
- **PULL_REQUEST_TEMPLATE.md**
- **ISSUE_TEMPLATE/**
- **workflows**: configuration files for GitHub Actions.

## 3. Root files

Mandatory:
- add a **README.md**
- add a **LICENSE.md**
- add a **.gitignore**

Optional:
- **CHANGELOG.md**: describe what are the changes throughout the different versions and releases in the repository.
- **CONTRIBUTING.md**: explain how people should contribute the the repository.
- **CONTRIBUTORS.md**: list all the people who have contributed to the repository.
- **ISSUE_TEMPLATE**: project contributors will automatically see the template's contents in the issue body. If you need multiple templates, add them to a directory named **ISSUE_TEMPLATE/**.
- **PULL_REQUEST_TEMPLATE**: project contributors will automatically see the template's contents in the pull request body. If you need multiple templates, add them to a directory named **PULL_REQUEST_TEMPLATE/**.
- **.gitmodules**: define submodule(s) used in the repository

### 3.1 Choose the appropriate license

Useful links:
- https://choosealicense.com/
- https://ufal.github.io/public-license-selector/

## 4. References

- https://climbtheladder.com/10-git-repository-naming-best-practices/
- https://www.codementor.io/@louiekwan/azure-devops-guardrails-naming-conventions-and-standards-1gn1v7bebh
- https://medium.com/code-factory-berlin/github-repository-structure-best-practices-248e6effc405
