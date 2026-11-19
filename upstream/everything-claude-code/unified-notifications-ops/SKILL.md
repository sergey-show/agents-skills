---
id: everything-claude-code__unified-notifications-ops
name: unified-notifications-ops
version: 1.0.0
description: >-
  Operate notifications as one ECC-native workflow across GitHub, Linear, desktop alerts, hooks, and connected communication surfaces. Use when the real problem is alert routing, deduplication, escalation, or inbox collapse.
role: unified-notifications-ops
category: ops
triggers:
  - unified notifications ops
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
sources:
  - research/everything-claude-code/skills/unified-notifications-ops/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: unified-notifications-ops
---

# unified-notifications-ops

## Role

Portable distillation of upstream skill `unified-notifications-ops` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Operate notifications as one ECC-native workflow across GitHub, Linear, desktop alerts, hooks, and connected communication surfaces. Use when the real problem is alert routing, deduplication, escalation, or inbox collapse.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
