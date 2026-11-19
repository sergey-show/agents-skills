---
id: everything-claude-code__safety-guard
name: safety-guard
version: 1.0.0
description: >-
  Guard against destructive operations with three modes: Careful intercepts dangerous commands (rm -rf, git push --force, DROP TABLE) for confirmation, Freeze locks writes to one directory, and Guard combines both. Advisory: the agent applies these rules itself; no hook ships with it. Use when working on production systems, running agents autonomously, restricting edits to a directory, or during migrations, deploys, and data changes.
role: safety-guard
category: ops
triggers:
  - safety guard
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/skills/safety-guard/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: safety-guard
---

# safety-guard

## Role

Portable distillation of upstream skill `safety-guard` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Guard against destructive operations with three modes: Careful intercepts dangerous commands (rm -rf, git push --force, DROP TABLE) for confirmation, Freeze locks writes to one directory, and Guard combines both. Advisory: the agent applies these rules itself; no hook ships with it. Use when working on production systems, running agents autonomously, restricting edits to a directory, or during migrations, deploys, and data changes.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
