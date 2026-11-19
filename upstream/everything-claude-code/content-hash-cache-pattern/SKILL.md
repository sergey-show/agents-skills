---
id: everything-claude-code__content-hash-cache-pattern
name: content-hash-cache-pattern
version: 1.0.0
description: >-
  Cache expensive file processing results using SHA-256 content hashes — path-independent, auto-invalidating, with service layer separation. Use when repeated file processing is slow and results should be cached and invalidated by content rather than path.
role: content-hash-cache-pattern
category: engineering
triggers:
  - content hash cache pattern
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/skills/content-hash-cache-pattern/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: content-hash-cache-pattern
---

# content-hash-cache-pattern

## Role

Portable distillation of upstream skill `content-hash-cache-pattern` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Cache expensive file processing results using SHA-256 content hashes — path-independent, auto-invalidating, with service layer separation. Use when repeated file processing is slow and results should be cached and invalidated by content rather than path.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
