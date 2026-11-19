---
id: everything-claude-code__ui-demo
name: ui-demo
version: 1.0.0
description: >-
  Record polished UI demo videos using Playwright. Use when the user asks to create a demo, walkthrough, screen recording, or tutorial video of a web application. Produces WebM videos with visible cursor, natural pacing, and professional feel.
role: ui-demo
category: design
triggers:
  - ui demo
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
sources:
  - research/everything-claude-code/skills/ui-demo/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ui-demo
---

# ui-demo

## Role

Portable distillation of upstream skill `ui-demo` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Record polished UI demo videos using Playwright. Use when the user asks to create a demo, walkthrough, screen recording, or tutorial video of a web application. Produces WebM videos with visible cursor, natural pacing, and professional feel.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
