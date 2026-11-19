---
id: everything-claude-code__mcp-server-patterns
name: mcp-server-patterns
version: 1.0.0
description: >-
  Build MCP servers with Node/TypeScript SDK — tools, resources, prompts, Zod validation, stdio vs Streamable HTTP. Use Context7 or official MCP docs for latest API. Use when building or debugging an MCP server — tools, resources, prompts, validation, or transport choice.
role: mcp-server-patterns
category: meta
triggers:
  - mcp server patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/.agents/skills/mcp-server-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: mcp-server-patterns
---

# mcp-server-patterns

## Role

Portable distillation of upstream skill `mcp-server-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Build MCP servers with Node/TypeScript SDK — tools, resources, prompts, Zod validation, stdio vs Streamable HTTP. Use Context7 or official MCP docs for latest API. Use when building or debugging an MCP server — tools, resources, prompts, validation, or transport choice.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
