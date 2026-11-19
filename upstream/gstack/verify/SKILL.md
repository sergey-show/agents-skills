---
id: gstack__verify
name: verify
version: 1.0.0
description: >-
  Use when coding: run the checks and tests /ship picks until green. Use for: verify my change, run the checks, make the tests pass. (gstack)
role: verify
category: meta
triggers:
  - verify
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/gstack/verify/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: verify
---

# verify

## Role

Portable distillation of upstream skill `verify` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when coding: run the checks and tests /ship picks until green. Use for: verify my change, run the checks, make the tests pass. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
