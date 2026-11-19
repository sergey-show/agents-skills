---
id: gstack__design-review
name: design-review
version: 1.0.0
description: >-
  Designer's eye QA: finds visual inconsistency, spacing issues, hierarchy problems, AI slop patterns, and slow interactions — then fixes them; --build checks UI while you build it. Use for: visual design audit, design qa. (gstack)
role: design-review
category: design
triggers:
  - design review
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/gstack/design-review/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: design-review
---

# design-review

## Role

Portable distillation of upstream skill `design-review` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Designer's eye QA: finds visual inconsistency, spacing issues, hierarchy problems, AI slop patterns, and slow interactions — then fixes them; --build checks UI while you build it. Use for: visual design audit, design qa. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
