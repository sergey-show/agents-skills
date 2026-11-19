---
id: gstack__devex-review
name: devex-review
version: 1.0.0
description: >-
  Live developer experience audit. Use for: live dx audit, test developer experience. (gstack)
role: devex-review
category: meta
triggers:
  - devex review
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/gstack/devex-review/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: devex-review
---

# devex-review

## Role

Portable distillation of upstream skill `devex-review` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Live developer experience audit. Use for: live dx audit, test developer experience. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
