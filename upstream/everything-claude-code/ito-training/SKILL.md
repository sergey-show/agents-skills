---
id: everything-claude-code__ito-training
name: ito-training
version: 1.0.0
description: >-
  Inspect the availability of ML training on a completed Itô compute booking and, when the canonical backend becomes available, hand off an explicitly confirmed training manifest. Use after ito-compute has booked GPU nodes and the user wants pre-training, fine-tuning, or RL on that metal. ECC implements no training stack of its own.
role: ito-training
category: meta
triggers:
  - ito training
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - shell.exec
sources:
  - research/everything-claude-code/skills/ito-training/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ito-training
---

# ito-training

## Role

Portable distillation of upstream skill `ito-training` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Inspect the availability of ML training on a completed Itô compute booking and, when the canonical backend becomes available, hand off an explicitly confirmed training manifest. Use after ito-compute has booked GPU nodes and the user wants pre-training, fine-tuning, or RL on that metal. ECC implements no training stack of its own.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
