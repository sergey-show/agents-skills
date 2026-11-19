---
id: gstack__open-gstack-browser
name: open-gstack-browser
version: 1.0.0
description: >-
  Launch GStack Browser — AI-controlled Chromium with the sidebar extension baked in. Use for: open gstack browser, launch chromium.
role: open-gstack-browser
category: meta
triggers:
  - open gstack browser
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
  - test.run
sources:
  - research/gstack/open-gstack-browser/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: open-gstack-browser
---

# open-gstack-browser

## Role

Portable distillation of upstream skill `open-gstack-browser` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Launch GStack Browser — AI-controlled Chromium with the sidebar extension baked in. Use for: open gstack browser, launch chromium.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
