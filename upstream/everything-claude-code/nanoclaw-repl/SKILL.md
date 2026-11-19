---
id: everything-claude-code__nanoclaw-repl
name: nanoclaw-repl
version: 1.0.0
description: >-
  Operate and extend NanoClaw, ECC's zero-dependency session-aware REPL, with persistent markdown-backed sessions and slash commands for model switching, skill loading, session branching, cross-session search, history compaction, and export. Use when running or extending scripts/claw.js, or when resuming, branching, compacting, searching, or exporting a NanoClaw session.
role: nanoclaw-repl
category: meta
triggers:
  - nanoclaw repl
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
sources:
  - research/everything-claude-code/skills/nanoclaw-repl/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: nanoclaw-repl
---

# nanoclaw-repl

## Role

Portable distillation of upstream skill `nanoclaw-repl` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Operate and extend NanoClaw, ECC's zero-dependency session-aware REPL, with persistent markdown-backed sessions and slash commands for model switching, skill loading, session branching, cross-session search, history compaction, and export. Use when running or extending scripts/claw.js, or when resuming, branching, compacting, searching, or exporting a NanoClaw session.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
