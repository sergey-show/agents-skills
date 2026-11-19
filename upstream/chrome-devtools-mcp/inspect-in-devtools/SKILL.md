---
id: chrome-devtools-mcp__inspect-in-devtools
name: inspect-in-devtools
version: 1.0.0
description: >-
  Use this skill to connect to the Chrome DevTools UI for interactive debugging, UI/UX review, Q&A, showing elements/network requests/panels to the user, inspecting the user's current DevTools selection, and addressing or polling for DevTools UI comment threads.
role: inspect-in-devtools
category: meta
triggers:
  - inspect in devtools
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
sources:
  - research/chrome-devtools-mcp/skills/inspect-in-devtools/SKILL.md
harness: any
upstream_repo: chrome-devtools-mcp
upstream_skill: inspect-in-devtools
---

# inspect-in-devtools

## Role

Portable distillation of upstream skill `inspect-in-devtools` from `chrome-devtools-mcp`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use this skill to connect to the Chrome DevTools UI for interactive debugging, UI/UX review, Q&A, showing elements/network requests/panels to the user, inspecting the user's current DevTools selection, and addressing or polling for DevTools UI comment threads.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
