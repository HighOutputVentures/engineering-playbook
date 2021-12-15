# Merge Strategies



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
