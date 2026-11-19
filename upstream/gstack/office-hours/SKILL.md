---
id: gstack__office-hours
name: office-hours
version: 1.0.0
description: >-
  YC Office Hours — two modes. Use for: brainstorm this, is this worth building. (gstack)
role: office-hours
category: meta
triggers:
  - office hours
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
  - research/gstack/office-hours/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: office-hours
---

# office-hours

## Role

Portable distillation of upstream skill `office-hours` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

YC Office Hours — two modes. Use for: brainstorm this, is this worth building. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
