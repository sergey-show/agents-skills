---
id: gstack__unfreeze
name: unfreeze
version: 1.0.0
description: >-
  Clear the freeze boundary set by /freeze, allowing edits to all directories again. Use for: unfreeze edits, unlock all directories. (gstack)
role: unfreeze
category: meta
triggers:
  - unfreeze
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
sources:
  - research/gstack/unfreeze/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: unfreeze
---

# unfreeze

## Role

Portable distillation of upstream skill `unfreeze` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Clear the freeze boundary set by /freeze, allowing edits to all directories again. Use for: unfreeze edits, unlock all directories. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
