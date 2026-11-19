---
id: everything-claude-code__autonomous-agent-harness
name: autonomous-agent-harness
version: 1.0.0
description: >-
  Transform the coding agent into a fully autonomous agent system with persistent memory, scheduled operations, computer use, and task queuing. Replaces standalone agent frameworks (Hermes, AutoGPT) by leveraging the coding agent's native crons, dispatch, MCP tools, and memory. Use when the user wants continuous autonomous operation, scheduled tasks, or a self-directing agent loop.
role: autonomous-agent-harness
category: meta
triggers:
  - autonomous agent harness
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/autonomous-agent-harness/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: autonomous-agent-harness
---

# autonomous-agent-harness

## Role

Portable distillation of upstream skill `autonomous-agent-harness` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Transform the coding agent into a fully autonomous agent system with persistent memory, scheduled operations, computer use, and task queuing. Replaces standalone agent frameworks (Hermes, AutoGPT) by leveraging the coding agent's native crons, dispatch, MCP tools, and memory. Use when the user wants continuous autonomous operation, scheduled tasks, or a self-directing agent loop.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
