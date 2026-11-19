---
id: gstack__plan-design-review
name: plan-design-review
version: 1.0.0
description: >-
  Designer's eye plan review — interactive, like CEO and Eng review. Use for: design plan review, review ux plan. (gstack)
role: plan-design-review
category: design
triggers:
  - plan design review
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
  - research/gstack/plan-design-review/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: plan-design-review
---

# plan-design-review

## Role

Portable distillation of upstream skill `plan-design-review` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Designer's eye plan review — interactive, like CEO and Eng review. Use for: design plan review, review ux plan. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
