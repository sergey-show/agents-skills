---
id: everything-claude-code__ck
name: ck
version: 1.0.0
description: >-
  Persistent per-project memory for the coding agent (Context Keeper) driven by deterministic Node.js /ck commands: init, save, resume, info, list, forget, and v1-to-v2 migrate, plus a SessionStart hook that injects a compact project brief. Use when context must survive across sessions, saving session state with next steps and decisions, resuming where a previous session left off, or picking up a project without re-explaining it.
role: ck
category: meta
triggers:
  - ck
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
sources:
  - research/everything-claude-code/skills/ck/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ck
---

# ck

## Role

Portable distillation of upstream skill `ck` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Persistent per-project memory for the coding agent (Context Keeper) driven by deterministic Node.js /ck commands: init, save, resume, info, list, forget, and v1-to-v2 migrate, plus a SessionStart hook that injects a compact project brief. Use when context must survive across sessions, saving session state with next steps and decisions, resuming where a previous session left off, or picking up a project without re-explaining it.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
