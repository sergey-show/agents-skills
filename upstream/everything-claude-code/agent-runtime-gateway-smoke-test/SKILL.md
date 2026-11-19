---
id: everything-claude-code__agent-runtime-gateway-smoke-test
name: agent-runtime-gateway-smoke-test
version: 1.0.0
description: >-
  Verify a local agent API, temporary gateway tunnel, and remote sandbox callback with a tool-free task, then restore the original app connection.
role: agent-runtime-gateway-smoke-test
category: research
triggers:
  - agent runtime gateway smoke test
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/agent-runtime-gateway-smoke-test/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: agent-runtime-gateway-smoke-test
---

# agent-runtime-gateway-smoke-test

## Role

Portable distillation of upstream skill `agent-runtime-gateway-smoke-test` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Verify a local agent API, temporary gateway tunnel, and remote sandbox callback with a tool-free task, then restore the original app connection.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
