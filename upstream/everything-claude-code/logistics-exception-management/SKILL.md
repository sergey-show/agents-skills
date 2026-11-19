---
id: everything-claude-code__logistics-exception-management
name: logistics-exception-management
version: 1.0.0
description: >-
  Codified freight-exception handling expertise for shipment delays, damages, losses, shortages, and carrier disputes, with escalation protocols, carrier-specific behaviors by mode, claims procedures, and eat-the-cost vs fight-the-claim judgment frameworks. Use when handling shipping exceptions, freight claims, delivery issues, or carrier disputes.
role: logistics-exception-management
category: ops
triggers:
  - logistics exception management
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/logistics-exception-management/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: logistics-exception-management
---

# logistics-exception-management

## Role

Portable distillation of upstream skill `logistics-exception-management` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Codified freight-exception handling expertise for shipment delays, damages, losses, shortages, and carrier disputes, with escalation protocols, carrier-specific behaviors by mode, claims procedures, and eat-the-cost vs fight-the-claim judgment frameworks. Use when handling shipping exceptions, freight claims, delivery issues, or carrier disputes.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
