---
id: gstack__freeze
name: freeze
version: 1.0.0
description: >-
  Restrict file edits to a specific directory for the session. Use for: freeze edits to directory, lock editing scope. (gstack)
role: freeze
category: meta
triggers:
  - freeze
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
sources:
  - research/gstack/freeze/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: freeze
---

# freeze

## Role

Portable distillation of upstream skill `freeze` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Restrict file edits to a specific directory for the session. Use for: freeze edits to directory, lock editing scope. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
