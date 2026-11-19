---
id: everything-claude-code__module-governance
name: module-governance
version: 1.0.0
description: >-
  Establish or maintain a business module's local agent instructions, domain-context links, and interface ownership when implementing a new module or changing its responsibilities. Reuse project-level rules and existing ECC workflows; ordinary bug fixes, styling, and read-only design discussions do not start module documentation setup.
role: module-governance
category: meta
triggers:
  - module governance
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/module-governance/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: module-governance
---

# module-governance

## Role

Portable distillation of upstream skill `module-governance` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Establish or maintain a business module's local agent instructions, domain-context links, and interface ownership when implementing a new module or changing its responsibilities. Reuse project-level rules and existing ECC workflows; ordinary bug fixes, styling, and read-only design discussions do not start module documentation setup.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
