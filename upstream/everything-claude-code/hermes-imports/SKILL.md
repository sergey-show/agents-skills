---
id: everything-claude-code__hermes-imports
name: hermes-imports
version: 1.0.0
description: >-
  Convert local Hermes operator workflows into sanitized ECC skills and release-pack artifacts. Use when preparing a Hermes workflow for public ECC reuse without leaking private workspace state, credentials, or local-only paths.
role: hermes-imports
category: research
triggers:
  - hermes imports
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
sources:
  - research/everything-claude-code/skills/hermes-imports/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: hermes-imports
---

# hermes-imports

## Role

Portable distillation of upstream skill `hermes-imports` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Convert local Hermes operator workflows into sanitized ECC skills and release-pack artifacts. Use when preparing a Hermes workflow for public ECC reuse without leaking private workspace state, credentials, or local-only paths.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
