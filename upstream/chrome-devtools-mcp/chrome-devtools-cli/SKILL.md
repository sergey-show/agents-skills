---
id: chrome-devtools-mcp__chrome-devtools-cli
name: chrome-devtools-cli
version: 1.0.0
description: >-
  Use this skill to write shell scripts or run shell commands to automate tasks in the browser or otherwise use Chrome DevTools via CLI.
role: chrome-devtools-cli
category: engineering
triggers:
  - chrome devtools cli
capabilities_required:
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - test.run
sources:
  - research/chrome-devtools-mcp/skills/chrome-devtools-cli/SKILL.md
harness: any
upstream_repo: chrome-devtools-mcp
upstream_skill: chrome-devtools-cli
---

# chrome-devtools-cli

## Role

Portable distillation of upstream skill `chrome-devtools-cli` from `chrome-devtools-mcp`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use this skill to write shell scripts or run shell commands to automate tasks in the browser or otherwise use Chrome DevTools via CLI.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
