---
id: gstack__document-release
name: document-release
version: 1.0.0
description: >-
  Release documentation audit. Use for: update docs after ship, document what changed. (gstack)
role: document-release
category: ops
triggers:
  - document release
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/gstack/document-release/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: document-release
---

# document-release

## Role

Portable distillation of upstream skill `document-release` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Release documentation audit. Use for: update docs after ship, document what changed. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
