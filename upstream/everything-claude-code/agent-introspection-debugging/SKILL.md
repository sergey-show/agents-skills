---
id: everything-claude-code__agent-introspection-debugging
name: agent-introspection-debugging
version: 1.0.0
description: >-
  Structured self-debugging workflow for AI agent failures using capture, diagnosis, contained recovery, and introspection reports. Use when an agent run fails and you need a reproducible diagnosis instead of a retry.
role: agent-introspection-debugging
category: meta
triggers:
  - agent introspection debugging
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/agent-introspection-debugging/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: agent-introspection-debugging
---

# agent-introspection-debugging

## Role

Portable distillation of upstream skill `agent-introspection-debugging` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Structured self-debugging workflow for AI agent failures using capture, diagnosis, contained recovery, and introspection reports. Use when an agent run fails and you need a reproducible diagnosis instead of a retry.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
