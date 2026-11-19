---
id: gstack__landing-report
name: landing-report
version: 1.0.0
description: >-
  Read-only queue dashboard for workspace-aware ship. Use for: landing report, version queue, ship queue. (gstack)
role: landing-report
category: meta
triggers:
  - landing report
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
sources:
  - research/gstack/landing-report/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: landing-report
---

# landing-report

## Role

Portable distillation of upstream skill `landing-report` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Read-only queue dashboard for workspace-aware ship. Use for: landing report, version queue, ship queue. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
