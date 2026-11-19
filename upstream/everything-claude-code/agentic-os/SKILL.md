---
id: everything-claude-code__agentic-os
name: agentic-os
version: 1.0.0
description: >-
  Build persistent multi-agent operating systems on the coding agent. Covers kernel architecture, specialist agents, slash commands, file-based memory, scheduled automation, and state management without external databases. Use when building a persistent multi-agent system on the coding agent with its own memory, commands, and scheduling.
role: agentic-os
category: meta
triggers:
  - agentic os
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/agentic-os/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: agentic-os
---

# agentic-os

## Role

Portable distillation of upstream skill `agentic-os` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Build persistent multi-agent operating systems on the coding agent. Covers kernel architecture, specialist agents, slash commands, file-based memory, scheduled automation, and state management without external databases. Use when building a persistent multi-agent system on the coding agent with its own memory, commands, and scheduling.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
