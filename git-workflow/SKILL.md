---
id: git-workflow
name: Git Workflow
version: 1.0.0
description: >-
  Atomic commits, branch discipline, PR hygiene, versioning and
  changelogs. Use whenever committing, branching, splitting messy trees,
  opening PRs, or cutting releases.
role: Git / Versioning Lead
category: ops
triggers:
  - commit
  - atomic commits
  - pull request
  - branching
  - semver
  - changelog
  - git workflow
capabilities_required:
  - git.ops
capabilities_optional:
  - shell.exec
  - ask_user
  - filesystem.read
sources:
  - research/agent-skills/skills/git-workflow-and-versioning
harness: any
---

# Git Workflow

## Role
Git is the safety net. Commits are save points; branches are short-lived sandboxes; history is documentation — especially when agents generate code fast.

## When to use
Any commit/branch/PR/release/version bump; splitting messy working trees; writing commit messages or changelogs.

## Workflow
1. Prefer trunk-based short-lived branches; flags > long branches.
2. Slice → test → verify → atomic commit.
3. Message explains why; conventional prefixes when repo uses them.
4. PR small, focused, with test plan.
5. Semver + changelog for releases.

## Done when
History reviewable; each commit one logical change; main kept deployable per team policy.

## See also
- [approaches.md](approaches.md)

## Upstream depth

- `skills/upstream/agent-skills/git-workflow-and-versioning/`
- `skills/upstream/superpowers/finishing-a-development-branch/`
- `skills/upstream/mattpocock-skills/pr/`
