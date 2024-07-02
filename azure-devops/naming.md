# Naming <!-- omit in toc -->

## Table of Contents <!-- omit in toc -->

- [1. Introduction](#1-introduction)
- [2. Domains](#2-domains)
- [3. Projects](#3-projects)
  - [3.1 General](#31-general)
  - [3.2 Project description](#32-project-description)
- [4. Teams](#4-teams)
- [5. Pipelines](#5-pipelines)
- [6. Miscellaneous](#6-miscellaneous)
- [7. References](#7-references)

## 1. Introduction

List of criteria to match and rules to follow when naming an Azure DevOps object. For anything git-related, please refer to [Git Naming Conventions](../git/naming.md).

## 2. Domains

Rules:
- Add icon
- Pascal Case (ex. Project Name) or lower case (ex. project name), recommending the latter since it is used in the URL (replacing spaces by underscores if any)
- No underscore or hyphen to separate words, only spaces

## 3. Projects

### 3.1 General

Rules:
- Add project profile image
- Pascal Case (ex. Project Name) or lower case (ex. project name), recommending the latter since it is used in the URL (replacing spaces by underscores if any)
- No underscore or hyphen to separate words, only spaces

### 3.2 Project description

- One sentence to give the big picture of the project
- List who are the administrators and/or maintainers of the project so that anyone can contact them quickly

## 4. Teams

- Pascal Case (ex. Team Name)
- no underscore, only hyphen or spaces (ex Development, DevOps, QA...)
- no need for a "Team" suffix, it is redundant in the naming. People should be able to identify if a given object is a team by the icon of it, or by hovering on it with the mouse

## 5. Pipelines

- {Repo Name} : {Pipeline Description} (`git-app-repo : ci-build` for instance)

Reasons
- keeps pipelines visually bounded to related repositories in the DevOps UI
- follows industry standards, what's done in the open source world on GitHub, etc.
- ease for navigation when cloned locally

## 6. Miscellaneous

Good practices:
- Creation of a dedicated project where people can suggest some improvements of the platform to the administrators

## 7. References

- https://www.codementor.io/@louiekwan/azure-devops-guardrails-naming-conventions-and-standards-1gn1v7bebh
