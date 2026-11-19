---
id: everything-claude-code__context-and-decisions
name: context-and-decisions
version: 1.0.0
description: >-
  Govern stable domain context with a narrowly scoped CONTEXT.md when needed, and route hard-to-reverse decisions to ECC's existing architecture-decision-records skill. Use when domain terms require repeated explanation, one term has multiple meanings, unclear language causes module-boundary mistakes, or domain semantics must remain separate from architecture decisions.
role: context-and-decisions
category: engineering
triggers:
  - context and decisions
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/context-and-decisions/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: context-and-decisions
---

# context-and-decisions

## Role

Portable distillation of upstream skill `context-and-decisions` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Govern stable domain context with a narrowly scoped CONTEXT.md when needed, and route hard-to-reverse decisions to ECC's existing architecture-decision-records skill. Use when domain terms require repeated explanation, one term has multiple meanings, unclear language causes module-boundary mistakes, or domain semantics must remain separate from architecture decisions.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
