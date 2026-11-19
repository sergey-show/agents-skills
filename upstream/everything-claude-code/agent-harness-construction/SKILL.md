---
id: everything-claude-code__agent-harness-construction
name: agent-harness-construction
version: 1.0.0
description: >-
  Design and optimize AI agent action spaces, tool definitions, and observation formatting for higher completion rates. Use when defining or revising an agent's tool set, action space, or observation format.
role: agent-harness-construction
category: design
triggers:
  - agent harness construction
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  []
sources:
  - research/everything-claude-code/skills/agent-harness-construction/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: agent-harness-construction
---

# agent-harness-construction

## Role

Portable distillation of upstream skill `agent-harness-construction` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Design and optimize AI agent action spaces, tool definitions, and observation formatting for higher completion rates. Use when defining or revising an agent's tool set, action space, or observation format.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
