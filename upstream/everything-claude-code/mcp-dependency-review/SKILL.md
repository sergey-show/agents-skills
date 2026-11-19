---
id: everything-claude-code__mcp-dependency-review
name: mcp-dependency-review
version: 1.0.0
description: >-
  Statically review MCP configuration for mutable package references before approval or CI, without executing discovered MCP servers. Use when reviewing .mcp.json, the coding agent, VS Code, Claude, Windsurf, or other repo-scoped MCP config.
role: mcp-dependency-review
category: meta
triggers:
  - mcp dependency review
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/mcp-dependency-review/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: mcp-dependency-review
---

# mcp-dependency-review

## Role

Portable distillation of upstream skill `mcp-dependency-review` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Statically review MCP configuration for mutable package references before approval or CI, without executing discovered MCP servers. Use when reviewing .mcp.json, the coding agent, VS Code, Claude, Windsurf, or other repo-scoped MCP config.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
