---
id: ponytail__ponytail-gain
name: ponytail-gain
version: 1.0.0
description: >-
  Show ponytail's measured savings (code, cost, speed) from the benchmark. One-shot display. Use for /ponytail-gain, "what does ponytail save", "ponytail impact".
role: ponytail-gain
category: security
triggers:
  - ponytail gain
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/ponytail/skills/ponytail-gain/SKILL.md
harness: any
upstream_repo: ponytail
upstream_skill: ponytail-gain
---

# ponytail-gain

## Role

Portable distillation of upstream skill `ponytail-gain` from `ponytail`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Show ponytail's measured savings (code, cost, speed) from the benchmark. One-shot display. Use for /ponytail-gain, "what does ponytail save", "ponytail impact".

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
