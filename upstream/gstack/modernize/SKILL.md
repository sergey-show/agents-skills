---
id: gstack__modernize
name: modernize
version: 1.0.0
description: >-
  Bring an aging PR onto its current base and decide: MODERNIZE, REWORK or CLOSE. Use for: modernize this pr, rebase this old pr. (gstack)
role: modernize
category: meta
triggers:
  - modernize
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/gstack/modernize/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: modernize
---

# modernize

## Role

Portable distillation of upstream skill `modernize` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Bring an aging PR onto its current base and decide: MODERNIZE, REWORK or CLOSE. Use for: modernize this pr, rebase this old pr. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
