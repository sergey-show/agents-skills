---
id: agent-skills__browser-testing-with-devtools
name: browser-testing-with-devtools
version: 1.0.0
description: >-
  Tests in real browsers via Chrome DevTools MCP. Use when building or debugging anything that runs in a browser. Use when you need to inspect the DOM, capture console errors, analyze network requests, profile performance, or verify visual output with real runtime data. Requires the chrome-devtools MCP server to be configured.
role: browser-testing-with-devtools
category: design
triggers:
  - browser testing with devtools
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - test.run
sources:
  - research/agent-skills/skills/browser-testing-with-devtools/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: browser-testing-with-devtools
---

# browser-testing-with-devtools

## Role

Portable distillation of upstream skill `browser-testing-with-devtools` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Tests in real browsers via Chrome DevTools MCP. Use when building or debugging anything that runs in a browser. Use when you need to inspect the DOM, capture console errors, analyze network requests, profile performance, or verify visual output with real runtime data. Requires the chrome-devtools MCP server to be configured.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
