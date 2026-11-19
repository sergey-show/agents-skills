---
id: everything-claude-code__contract-first
name: contract-first
version: 1.0.0
description: >-
  Coordinate frontend/backend or service-to-service work through one authoritative machine-checkable contract (OpenAPI, AsyncAPI, Protocol Buffers, or JSON Schema), with generated consumer types and contract-verified integration. Use when parallel consumer and provider work must evolve an API or event schema without field drift, mock/production shape mismatch, or one side silently redefining the interface.
role: contract-first
category: design
triggers:
  - contract first
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/contract-first/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: contract-first
---

# contract-first

## Role

Portable distillation of upstream skill `contract-first` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Coordinate frontend/backend or service-to-service work through one authoritative machine-checkable contract (OpenAPI, AsyncAPI, Protocol Buffers, or JSON Schema), with generated consumer types and contract-verified integration. Use when parallel consumer and provider work must evolve an API or event schema without field drift, mock/production shape mismatch, or one side silently redefining the interface.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
