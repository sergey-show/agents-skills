---
id: gstack__sync-gbrain
name: sync-gbrain
version: 1.0.0
description: >-
  Keep gbrain current with this repo's code and refresh agent search guidance in CLAUDE.md. Use for: sync gbrain, refresh gbrain, reindex repo. (gstack)
role: sync-gbrain
category: meta
triggers:
  - sync gbrain
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/gstack/sync-gbrain/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: sync-gbrain
---

# sync-gbrain

## Role

Portable distillation of upstream skill `sync-gbrain` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Keep gbrain current with this repo's code and refresh agent search guidance in CLAUDE.md. Use for: sync gbrain, refresh gbrain, reindex repo. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
