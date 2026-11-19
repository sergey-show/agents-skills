---
id: everything-claude-code__config-gc
name: config-gc
version: 1.0.0
description: >-
  Garbage collection for your the coding agent configuration. Periodically scans ~/.claude (skills, memory, hooks, permissions, MCP servers, caches) for redundant, stale, orphaned, or low-value items, then walks the user through a confirm-each-deletion cleanup. Use when the user says "clean up my config", "config GC", "too many skills", "audit my setup", "my .claude is bloated", or asks for a periodic config review.
role: config-gc
category: meta
triggers:
  - config gc
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
sources:
  - research/everything-claude-code/skills/config-gc/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: config-gc
---

# config-gc

## Role

Portable distillation of upstream skill `config-gc` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Garbage collection for your the coding agent configuration. Periodically scans ~/.claude (skills, memory, hooks, permissions, MCP servers, caches) for redundant, stale, orphaned, or low-value items, then walks the user through a confirm-each-deletion cleanup. Use when the user says "clean up my config", "config GC", "too many skills", "audit my setup", "my .claude is bloated", or asks for a periodic config review.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
