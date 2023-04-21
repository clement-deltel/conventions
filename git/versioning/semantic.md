# Semantic Versioning <!-- omit in toc -->

## Table of Contents <!-- omit in toc -->

- [1. Introduction](#1-introduction)
- [2. Key takeaways](#2-key-takeaways)
- [3. Rules](#3-rules)
- [4. Pros](#4-pros)
- [5. Cons](#5-cons)
- [6. References](#6-references)

## 1. Introduction

Here you will find a set of rules and requirements that dictate how version numbers are assigned and incremented, under the scope of the [Semantic Versioning](https://semver.org/) specification.

## 2. Key takeaways

Projects must use a version number MAJOR.MINOR.PATCH, incrementing:

- **MAJOR** version when you make incompatible API changes
- **MINOR** version when you add functionality in a backwards compatible manner
- **PATCH** version when you make backwards compatible bug fixes
- Additional labels for pre-release and build metadata are available as extensions, such as alpha.X, beta.X, or rc.X. X is an incremental number that can be omitted for the first version of the label.

## 3. Rules

Software using semantic versioning:
- **MUST** declare a public API

A normal version number:
- **MUST** take the form X.Y.Z
- **MUST** NOT contain leading zeroes
- Major version zero (0.y.z) is for initial development
- **SHOULD** be precise and comprehensive

Increment:
- Patch version **MUST** be reset to 0 when minor version is incremented
- Patch and minor versions **MUST** be reset to 0 when major version is incremented

Pre-release and build:
- Pre-release version **MAY** be denoted by appending a hyphen and a series of dot separated identifiers
- Build metadata **MAY** be denoted by appending a plus sign and a series of dot separated identifiers

Valid semantic version: `<major>.<minor>.<patch>-<pre-release>+<build>`

## 4. Pros

- Explain the developers about what type of changes have taken place
- Keep things clean and meaningful
- Keep track of every transition in the software development phase
- Help other people who might be using your project as a dependency
- Sane way to release and upgrade packages without having to roll new versions of dependent packages

## 5. Cons

- Not exclusively but mostly suitable for public API
- Compress a huge amount of information into a single number
- Treats all scenarios in the same way
- Any breaking change can make even the smallest change bump the major version

## 6. References

General:
- https://semver.org/
- https://en.wikipedia.org/wiki/Software_versioning
- https://www.geeksforgeeks.org/introduction-semantic-versioning/
- https://softwareengineering.stackexchange.com/questions/440811/how-do-i-choose-a-versioning-scheme-when-semantic-versioning-semver-isnt-appr
- https://gist.github.com/jashkenas/cbd2b088e20279ae2c8e

Regular Expressions to check versioning validity:
- https://regex101.com/r/Ly7O1x/3/
- https://regex101.com/r/vkijKf/1/
