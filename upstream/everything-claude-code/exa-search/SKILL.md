---
id: everything-claude-code__exa-search
name: exa-search
version: 1.0.0
description: >-
  Neural search via Exa MCP for web, code, and company research. Use when the user needs web search, code examples, company intel, people lookup, or AI-powered deep research with Exa's neural search engine.
role: exa-search
category: research
triggers:
  - exa search
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/exa-search/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: exa-search
---

# exa-search

## Role

Portable distillation of upstream skill `exa-search` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Neural search via Exa MCP for web, code, and company research. Use when the user needs web search, code examples, company intel, people lookup, or AI-powered deep research with Exa's neural search engine.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
