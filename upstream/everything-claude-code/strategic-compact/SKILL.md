---
id: everything-claude-code__strategic-compact
name: strategic-compact
version: 1.0.0
description: >-
  Suggests manual context compaction at logical intervals to preserve context through task phases rather than arbitrary auto-compaction. Use when a session is approaching a context limit and a task phase is a natural place to compact.
role: strategic-compact
category: research
triggers:
  - strategic compact
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/strategic-compact/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: strategic-compact
---

# strategic-compact

## Role

Portable distillation of upstream skill `strategic-compact` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Suggests manual context compaction at logical intervals to preserve context through task phases rather than arbitrary auto-compaction. Use when a session is approaching a context limit and a task phase is a natural place to compact.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
