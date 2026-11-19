---
id: ponytail__ponytail-review
name: ponytail-review
version: 1.0.0
description: >-
  Quality review of a change: is the logic right, is it safe, does it hold under real load, is risky code tested, is it fast enough, and is every line needed. Reads the connected code, not only the diff. Each finding is explained in plain English. Use for "review this", "code review", "review the last commit", "review my PR", "is this over-engineered", /ponytail-review.
role: ponytail-review
category: engineering
triggers:
  - ponytail review
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - test.run
sources:
  - research/ponytail/skills/ponytail-review/SKILL.md
harness: any
upstream_repo: ponytail
upstream_skill: ponytail-review
---

# ponytail-review

## Role

Portable distillation of upstream skill `ponytail-review` from `ponytail`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Quality review of a change: is the logic right, is it safe, does it hold under real load, is risky code tested, is it fast enough, and is every line needed. Reads the connected code, not only the diff. Each finding is explained in plain English. Use for "review this", "code review", "review the last commit", "review my PR", "is this over-engineered", /ponytail-review.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
