---
id: superpowers__using-git-worktrees
name: using-git-worktrees
version: 1.0.0
description: >-
  Use when starting feature work that needs isolation from current workspace or before executing implementation plans - ensures an isolated workspace exists via native tools or git worktree fallback
role: using-git-worktrees
category: meta
triggers:
  - using git worktrees
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/superpowers/skills/using-git-worktrees/SKILL.md
harness: any
upstream_repo: superpowers
upstream_skill: using-git-worktrees
---

# using-git-worktrees

## Role

Portable distillation of upstream skill `using-git-worktrees` from `superpowers`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when starting feature work that needs isolation from current workspace or before executing implementation plans - ensures an isolated workspace exists via native tools or git worktree fallback

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
