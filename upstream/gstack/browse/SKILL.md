---
id: gstack__browse
name: browse
version: 1.0.0
description: >-
  Drive a real browser through Aside: open a page, read it, click through a flow, take screenshots, check console errors. Use for: browse a page, open this url, take page screenshot. (gstack)
role: browse
category: meta
triggers:
  - browse
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/gstack/browse/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: browse
---

# browse

## Role

Portable distillation of upstream skill `browse` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Drive a real browser through Aside: open a page, read it, click through a flow, take screenshots, check console errors. Use for: browse a page, open this url, take page screenshot. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
