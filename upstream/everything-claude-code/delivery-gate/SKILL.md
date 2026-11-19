---
id: everything-claude-code__delivery-gate
name: delivery-gate
version: 1.0.0
description: >-
  Stop hook that blocks Claude from finishing until quality checks pass. Detects rationalization patterns (surface text heuristics), stale learning logs (filesystem mtime), and low disk space. Complements self-audit by mechanically enforcing learning capture habits. Use when Claude should be mechanically blocked from declaring work finished before quality checks and learning capture actually pass.
role: delivery-gate
category: engineering
triggers:
  - delivery gate
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/delivery-gate/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: delivery-gate
---

# delivery-gate

## Role

Portable distillation of upstream skill `delivery-gate` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Stop hook that blocks Claude from finishing until quality checks pass. Detects rationalization patterns (surface text heuristics), stale learning logs (filesystem mtime), and low disk space. Complements self-audit by mechanically enforcing learning capture habits. Use when Claude should be mechanically blocked from declaring work finished before quality checks and learning capture actually pass.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
