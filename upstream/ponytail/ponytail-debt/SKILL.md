---
id: ponytail__ponytail-debt
name: ponytail-debt
version: 1.0.0
description: >-
  List every `shortcut:` comment (and older `ponytail:` ones) as a debt ledger. One-shot report, changes nothing. Use for "ponytail debt", "what did ponytail defer", "list the shortcuts", /ponytail-debt.
role: ponytail-debt
category: engineering
triggers:
  - ponytail debt
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
sources:
  - research/ponytail/skills/ponytail-debt/SKILL.md
harness: any
upstream_repo: ponytail
upstream_skill: ponytail-debt
---

# ponytail-debt

## Role

Portable distillation of upstream skill `ponytail-debt` from `ponytail`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

List every `shortcut:` comment (and older `ponytail:` ones) as a debt ledger. One-shot report, changes nothing. Use for "ponytail debt", "what did ponytail defer", "list the shortcuts", /ponytail-debt.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
