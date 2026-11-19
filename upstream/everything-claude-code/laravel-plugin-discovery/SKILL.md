---
id: everything-claude-code__laravel-plugin-discovery
name: laravel-plugin-discovery
version: 1.0.0
description: >-
  Discover and evaluate Laravel packages via LaraPlugins.io MCP. Use when the user wants to find plugins, check package health, or assess Laravel/PHP compatibility.
role: laravel-plugin-discovery
category: meta
triggers:
  - laravel plugin discovery
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
  - test.run
sources:
  - research/everything-claude-code/skills/laravel-plugin-discovery/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: laravel-plugin-discovery
---

# laravel-plugin-discovery

## Role

Portable distillation of upstream skill `laravel-plugin-discovery` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Discover and evaluate Laravel packages via LaraPlugins.io MCP. Use when the user wants to find plugins, check package health, or assess Laravel/PHP compatibility.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
