---
id: gstack__ios-sync
name: ios-sync
version: 1.0.0
description: >-
  Regenerate the iOS debug bridge against the latest upstream gstack templates. Use for: resync the ios debug bridge, regenerate ios accessors. (gstack)
role: ios-sync
category: meta
triggers:
  - ios sync
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
sources:
  - research/gstack/ios-sync/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: ios-sync
---

# ios-sync

## Role

Portable distillation of upstream skill `ios-sync` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Regenerate the iOS debug bridge against the latest upstream gstack templates. Use for: resync the ios debug bridge, regenerate ios accessors. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
