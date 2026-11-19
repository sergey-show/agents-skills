---
id: gstack__setup-browser-cookies
name: setup-browser-cookies
version: 1.0.0
description: >-
  Import cookies from your real Chromium browser into the headless browse session. Use for: import browser cookies, login to test site. (gstack)
role: setup-browser-cookies
category: meta
triggers:
  - setup browser cookies
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
  - research/gstack/setup-browser-cookies/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: setup-browser-cookies
---

# setup-browser-cookies

## Role

Portable distillation of upstream skill `setup-browser-cookies` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Import cookies from your real Chromium browser into the headless browse session. Use for: import browser cookies, login to test site. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
