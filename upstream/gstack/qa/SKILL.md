---
id: gstack__qa
name: qa
version: 1.0.0
description: >-
  Use when you test the site, API or CLI and fix bugs. Use for: qa test this, find bugs on site, test the site. (gstack)
role: qa
category: meta
triggers:
  - qa
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
  - research/gstack/qa/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: qa
---

# qa

## Role

Portable distillation of upstream skill `qa` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when you test the site, API or CLI and fix bugs. Use for: qa test this, find bugs on site, test the site. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
