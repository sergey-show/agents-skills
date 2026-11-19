---
id: gstack__spec
name: spec
version: 1.0.0
description: >-
  Turn vague intent into a precise, executable spec in five phases. Use for: spec this out, file an issue, write up a ticket. (gstack)
role: spec
category: meta
triggers:
  - spec
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
  - research/gstack/spec/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: spec
---

# spec

## Role

Portable distillation of upstream skill `spec` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Turn vague intent into a precise, executable spec in five phases. Use for: spec this out, file an issue, write up a ticket. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
