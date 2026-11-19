---
id: everything-claude-code__docs-governance
name: docs-governance
version: 1.0.0
description: >-
  Route broad documentation-governance requests to existing ECC skills and run an opt-in, read-only audit of mapped documentation roles, links, ADR indexes, and evidence references. Use when a user asks for documentation governance, project-knowledge organization, documentation integrity, or a deterministic docs audit without naming a narrower skill.
role: docs-governance
category: engineering
triggers:
  - docs governance
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/docs-governance/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: docs-governance
---

# docs-governance

## Role

Portable distillation of upstream skill `docs-governance` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Route broad documentation-governance requests to existing ECC skills and run an opt-in, read-only audit of mapped documentation roles, links, ADR indexes, and evidence references. Use when a user asks for documentation governance, project-knowledge organization, documentation integrity, or a deterministic docs audit without naming a narrower skill.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
