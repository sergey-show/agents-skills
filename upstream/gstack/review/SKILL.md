---
id: gstack__review
name: review
version: 1.0.0
description: >-
  Use when you review a diff before it lands: local changes, a branch or a PR. Use for: review my changes, look over my diff, review this pr. (gstack)
role: review
category: meta
triggers:
  - review
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
  - research/gstack/review/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: review
---

# review

## Role

Portable distillation of upstream skill `review` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when you review a diff before it lands: local changes, a branch or a PR. Use for: review my changes, look over my diff, review this pr. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
