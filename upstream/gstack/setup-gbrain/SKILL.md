---
id: gstack__setup-gbrain
name: setup-gbrain
version: 1.0.0
description: >-
  Set up gbrain for this coding agent: install the CLI, initialize a local PGLite or Supabase brain, register MCP, capture per-remote trust policy. Use for: setup gbrain, install gbrain, connect gbrain. (gstack)
role: setup-gbrain
category: meta
triggers:
  - setup gbrain
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
  - subagent.spawn
  - test.run
sources:
  - research/gstack/setup-gbrain/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: setup-gbrain
---

# setup-gbrain

## Role

Portable distillation of upstream skill `setup-gbrain` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Set up gbrain for this coding agent: install the CLI, initialize a local PGLite or Supabase brain, register MCP, capture per-remote trust policy. Use for: setup gbrain, install gbrain, connect gbrain. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
