---
id: everything-claude-code__git-workflow
name: git-workflow
version: 1.0.0
description: >-
  Git workflow patterns including branching strategies, commit conventions, keeping history clean and readable, tidying local commits before merging, merge vs rebase, conflict resolution, and collaborative development best practices for teams of all sizes. Use when choosing a branching strategy, writing commit conventions, cleaning up history before a pull request, deciding merge versus rebase, or resolving conflicts.
role: git-workflow
category: ops
triggers:
  - git workflow
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/git-workflow/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: git-workflow
---

# git-workflow

## Role

Portable distillation of upstream skill `git-workflow` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Git workflow patterns including branching strategies, commit conventions, keeping history clean and readable, tidying local commits before merging, merge vs rebase, conflict resolution, and collaborative development best practices for teams of all sizes. Use when choosing a branching strategy, writing commit conventions, cleaning up history before a pull request, deciding merge versus rebase, or resolving conflicts.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
