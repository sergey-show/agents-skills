---
id: chrome-devtools-mcp__a11y-debugging
name: a11y-debugging
version: 1.0.0
description: >-
  Uses Chrome DevTools MCP for accessibility (a11y) debugging and auditing based on web.dev guidelines. Use when testing semantic HTML, ARIA labels, focus states, keyboard navigation, tap targets, and color contrast.
role: a11y-debugging
category: meta
triggers:
  - a11y debugging
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - test.run
sources:
  - research/chrome-devtools-mcp/skills/a11y-debugging/SKILL.md
harness: any
upstream_repo: chrome-devtools-mcp
upstream_skill: a11y-debugging
---

# a11y-debugging

## Role

Portable distillation of upstream skill `a11y-debugging` from `chrome-devtools-mcp`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Uses Chrome DevTools MCP for accessibility (a11y) debugging and auditing based on web.dev guidelines. Use when testing semantic HTML, ARIA labels, focus states, keyboard navigation, tap targets, and color contrast.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
