---
id: agent-skills__git-workflow-and-versioning
name: git-workflow-and-versioning
version: 1.0.0
description: >-
  Structures git workflow practices. Use when making any code change. Use when committing, branching, resolving conflicts, splitting uncommitted work in a messy working tree into clean atomic commits, opening or reviewing a pull request (PR), pushing to a remote, or when you need to organize work across multiple parallel streams. Use when cutting a release, choosing a semantic version bump, tagging, or writing a changelog. Use when asked to write a commit message or a changelog entry for a change, or to split a change into commits, even when the diff is pasted inline and the message seems easy to write from it.
role: git-workflow-and-versioning
category: ops
triggers:
  - git workflow and versioning
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/agent-skills/skills/git-workflow-and-versioning/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: git-workflow-and-versioning
---

# git-workflow-and-versioning

## Role

Portable distillation of upstream skill `git-workflow-and-versioning` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Structures git workflow practices. Use when making any code change. Use when committing, branching, resolving conflicts, splitting uncommitted work in a messy working tree into clean atomic commits, opening or reviewing a pull request (PR), pushing to a remote, or when you need to organize work across multiple parallel streams. Use when cutting a release, choosing a semantic version bump, tagging, or writing a changelog. Use when asked to write a commit message or a changelog entry for a change, or to split a change into commits, even when the diff is pasted inline and the message seems easy to write from it.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
