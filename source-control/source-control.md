# Source Control

## Overview

## Goals

* Following industry best practice to work
* Improve code quality by enforcing reviews before
* Improve traceability of features and fixes through a clean commit history.

## General Guidance

Be consistent

### Create a new repository

* Agree on the branch, release and merge strategy
* Define the merge strategy
* Lock the default branch and merge using pull requess(PRs)
* Establish branch/PR policies
* For public repositories the default should contain the following files:
  * LICENSE
  * README.md
  * CONTRIBUTING.md

### Commit Best Practices

## Merge Strategies

### Branch Policies

Configure protected branches at Git

### Rebase topic branch before Squash merge into main

#### Advantage of `Squash and Merge`

Follow the code standards

Peer code reviews

### Naming Branches

Look for `CONTRIBUTING.md`

`feature/*` `fix/*`

### Branching Model

#### Trunk-based development

Short-lived branches

Make use of Squash and Merge

### Commit Message

Follow this format:

```
[type]([optional scope]): [short summary]
  │       │             │
  │       │             └─⫸ Summary in present tense and imperative form. Not capitalized. No period at the end.
  │       │
  │       └─⫸ Commit Scope: bounded changes like. For example:
  │                          api | bazel | server | projection | framework
  │
  └─⫸ Commit Type: build|ci|docs|feat|fix|perf|refactor|test

[optional body]

[optional footer]
```

Example:

```
feat(api): add basic member's CRUD API

It includes a generic create, fetch all, update one and delete one endpoint for member.

closes JAM-12
```

```
feat: make lastname required

BREAKING CHANGE: `lastname` would required during create/register of an account.
```

### Versioning

To achieve loosely coupled components. This will allow developers to detect breaking changes or seamless updates (rollback and new release, A/B Testing, etc) just by looking at the version number

`major.minor.patch`

* `Major` - a breaking change
* `Minor` - a backward-compatible minor change
* `Patch` - no API change, fixes, or enhancements

### Git Guidance

### Resources

1. https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit
2. https://www.conventionalcommits.org/en/v1.0.0-beta.4/
