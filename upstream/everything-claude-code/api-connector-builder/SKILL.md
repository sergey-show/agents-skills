---
id: everything-claude-code__api-connector-builder
name: api-connector-builder
version: 1.0.0
description: >-
  Build a new API connector or provider by matching the target repo's existing integration pattern exactly. Use when adding one more integration without inventing a second architecture.
role: api-connector-builder
category: engineering
triggers:
  - api connector builder
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/skills/api-connector-builder/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: api-connector-builder
---

# api-connector-builder

## Role

Portable distillation of upstream skill `api-connector-builder` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Build a new API connector or provider by matching the target repo's existing integration pattern exactly. Use when adding one more integration without inventing a second architecture.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
