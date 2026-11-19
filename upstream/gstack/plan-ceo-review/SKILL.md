---
id: gstack__plan-ceo-review
name: plan-ceo-review
version: 1.0.0
description: >-
  CEO/founder-mode plan review. Use for: think bigger, expand scope, strategy review. (gstack)
role: plan-ceo-review
category: meta
triggers:
  - plan ceo review
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
  - subagent.spawn
  - test.run
sources:
  - research/gstack/plan-ceo-review/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: plan-ceo-review
---

# plan-ceo-review

## Role

Portable distillation of upstream skill `plan-ceo-review` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

CEO/founder-mode plan review. Use for: think bigger, expand scope, strategy review. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
