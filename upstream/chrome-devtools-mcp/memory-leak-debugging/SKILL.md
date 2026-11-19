---
id: chrome-devtools-mcp__memory-leak-debugging
name: memory-leak-debugging
version: 1.0.0
description: >-
  Diagnoses and resolves memory leaks in JavaScript/Node.js applications. Use when a user reports high memory usage, OOM errors, or wants to capture, compare, or inspect heap snapshots with Chrome DevTools MCP memory tools.
role: memory-leak-debugging
category: meta
triggers:
  - memory leak debugging
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
sources:
  - research/chrome-devtools-mcp/skills/memory-leak-debugging/SKILL.md
harness: any
upstream_repo: chrome-devtools-mcp
upstream_skill: memory-leak-debugging
---

# memory-leak-debugging

## Role

Portable distillation of upstream skill `memory-leak-debugging` from `chrome-devtools-mcp`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Diagnoses and resolves memory leaks in JavaScript/Node.js applications. Use when a user reports high memory usage, OOM errors, or wants to capture, compare, or inspect heap snapshots with Chrome DevTools MCP memory tools.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
