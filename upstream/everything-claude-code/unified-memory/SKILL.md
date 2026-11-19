---
id: everything-claude-code__unified-memory
name: unified-memory
version: 1.0.0
description: >-
  Share durable, inspectable context and handoffs between Claude, Codex, Hermes, the coding agent, OpenCode, and other agents through the local ECC Memory Vault. Use when an agent must save work state, transfer context, resume another agent's task, or search shared project knowledge.
role: unified-memory
category: meta
triggers:
  - unified memory
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/unified-memory/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: unified-memory
---

# unified-memory

## Role

Portable distillation of upstream skill `unified-memory` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Share durable, inspectable context and handoffs between Claude, Codex, Hermes, the coding agent, OpenCode, and other agents through the local ECC Memory Vault. Use when an agent must save work state, transfer context, resume another agent's task, or search shared project knowledge.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
