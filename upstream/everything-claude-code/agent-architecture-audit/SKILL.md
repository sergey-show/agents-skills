---
id: everything-claude-code__agent-architecture-audit
name: agent-architecture-audit
version: 1.0.0
description: >-
  Full-stack diagnostic for agent and LLM applications. Audits the 12-layer agent stack for wrapper regression, memory pollution, tool discipline failures, hidden repair loops, and rendering corruption. Produces severity-ranked findings with code-first fixes. Essential for developers building agent applications, autonomous loops, or any LLM-powered feature. Use when an agent or LLM feature misbehaves and the failing layer is unknown, or before shipping an agent stack.
role: agent-architecture-audit
category: ops
triggers:
  - agent architecture audit
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/skills/agent-architecture-audit/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: agent-architecture-audit
---

# agent-architecture-audit

## Role

Portable distillation of upstream skill `agent-architecture-audit` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Full-stack diagnostic for agent and LLM applications. Audits the 12-layer agent stack for wrapper regression, memory pollution, tool discipline failures, hidden repair loops, and rendering corruption. Produces severity-ranked findings with code-first fixes. Essential for developers building agent applications, autonomous loops, or any LLM-powered feature. Use when an agent or LLM feature misbehaves and the failing layer is unknown, or before shipping an agent stack.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
