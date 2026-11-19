---
id: chrome-devtools-mcp__chrome-devtools
name: chrome-devtools
version: 1.0.0
description: >-
  Uses Chrome DevTools via MCP for efficient debugging, troubleshooting and browser automation. Use when debugging web pages, automating browser interactions, analyzing performance, or inspecting network requests. This skill does not apply to `--slim` mode (MCP configuration).
role: chrome-devtools
category: meta
triggers:
  - chrome devtools
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/chrome-devtools-mcp/skills/chrome-devtools/SKILL.md
harness: any
upstream_repo: chrome-devtools-mcp
upstream_skill: chrome-devtools
---

# chrome-devtools

## Role

Portable distillation of upstream skill `chrome-devtools` from `chrome-devtools-mcp`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Uses Chrome DevTools via MCP for efficient debugging, troubleshooting and browser automation. Use when debugging web pages, automating browser interactions, analyzing performance, or inspecting network requests. This skill does not apply to `--slim` mode (MCP configuration).

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
