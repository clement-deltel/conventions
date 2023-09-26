# Calendar Versioning <!-- omit in toc -->

## Table of Contents <!-- omit in toc -->

- [1. Introduction](#1-introduction)
- [2. Key takeaways](#2-key-takeaways)
- [3. Rules](#3-rules)
- [4. Pros](#4-pros)
- [5. Cons](#5-cons)
- [6. References](#6-references)

## 1. Introduction

Here you will find a set of rules and requirements that dictate how version numbers are assigned and incremented, under the scope of the [Calendar Versioning](https://calver.org/) specification.

## 2. Key takeaways

There are multiple calendar versioning schemes. Here is the standard terminology in addition to the "[semantic](semantic.md)" versions:

- **YYYY** - Full year - 2006, 2016, 2106
- **YY** - Short year - 6, 16, 106
- **0Y** - Zero-padded year - 06, 16, 106
- **MM** - Short month - 1, 2 ... 11, 12
- **0M** - Zero-padded month - 01, 02 ... 11, 12
- **WW** - Short week (since start of year) - 1, 2, 33, 52
- **0W** - Zero-padded week - 01, 02, 33, 52
- **DD** - Short day - 1, 2 ... 30, 31
- **0D** - Zero-padded day - 01, 02 ... 30, 31

## 3. Rules

- traditional incremented version numbers are 0-based
- date segments are 1-based
- short and zero-padded years are relative to the year 2000
- usage of weeks is usually mutually exclusive with months/days

## 4. Pros

- Suitable for
  - projects featuring a large or constantly-changing scope
  - projects time-sensitive in any way
  - projects where external changes drive new project releases
- Works well with already mature and famous projects

## 5. Cons

- Versions tell you nothing about the projects except their release dates
- Researching some libraries and having to decide over which one to use can be difficult

## 6. References

- https://calver.org/
- https://www.cockroachlabs.com/blog/calendar-versioning/
