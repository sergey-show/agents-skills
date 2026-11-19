---
id: gstack__scrape
name: scrape
version: 1.0.0
description: >-
  Pull data from a web page through the Aside browser — your real, already signed-in sessions. Use for: scrape this page, get data from, pull from. (gstack)
role: scrape
category: meta
triggers:
  - scrape
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
  - test.run
sources:
  - research/gstack/scrape/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: scrape
---

# scrape

## Role

Portable distillation of upstream skill `scrape` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Pull data from a web page through the Aside browser — your real, already signed-in sessions. Use for: scrape this page, get data from, pull from. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
