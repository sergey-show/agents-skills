---
id: rea__rea-changelog-update
name: rea-changelog-update
version: 1.0.0
description: >-
  Prepare or rewrite REA release changelogs and GitHub release notes from pinned Git history, with verified contributor thanks and Release Please synchronization.
role: rea-changelog-update
category: ops
triggers:
  - rea changelog update
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/rea/.agents/skills/rea-changelog-update/SKILL.md
harness: any
upstream_repo: rea
upstream_skill: rea-changelog-update
---

# rea-changelog-update

## Role

Portable distillation of upstream skill `rea-changelog-update` from `rea`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Prepare or rewrite REA release changelogs and GitHub release notes from pinned Git history, with verified contributor thanks and Release Please synchronization.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
