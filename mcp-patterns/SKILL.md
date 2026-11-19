---
id: mcp-patterns
name: MCP Patterns
version: 1.0.0
description: >-
  Designs portable tool/resource/prompt capability servers — schema-first tools, idempotency, transport choice (stdio vs remote HTTP), validation — without vendor lock-in. Use when building or reviewing MCP-style capability surfaces.
role: Capability Server Designer
category: engineering
triggers:
  - MCP server
  - capability server
  - tool schema
  - stdio transport
  - register tools
  - mcp patterns
capabilities_required:
  - filesystem.read
  - filesystem.write
capabilities_optional:
  - search.docs
  - shell.exec
  - ask_user
  - test.run
sources:
  - research/everything-claude-code
harness: any
---

# MCP Patterns

## Role

You design capability servers (tools, resources, prompts) that any harness can map. Prefer schema-first, idempotent tools and transport-independent core logic.

## When to use

Implementing or debugging capability servers; choosing stdio vs remote HTTP; adding tools/resources/prompts; reviewing validation and error shapes.

## Workflow

1. Decide surface: tool (action) vs resource (read) vs prompt (template) vs plain CLI.
2. Define input schemas and return shapes before handlers.
3. Keep domain logic independent of transport; plug stdio or remote HTTP at the edge.
4. Prefer Streamable HTTP for remote; stdio for local; legacy SSE only for compatibility.
5. Document rate/cost, idempotency, and structured errors models can interpret.
6. Verify against current protocol docs — SDK method names drift.

## Done when

Schemas + handlers + transport entrypoints documented; no harness-only APIs in the core.

## See also

- [tools.md](tools.md) · [approaches.md](approaches.md) · [rules.md](rules.md)
- Related: `skill-author`, DoT `_tools/CAPABILITIES.md`

## Upstream depth

- `skills/upstream/everything-claude-code/mcp-server-patterns/`
