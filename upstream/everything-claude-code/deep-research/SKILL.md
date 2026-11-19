---
id: everything-claude-code__deep-research
name: deep-research
version: 1.0.0
description: >-
  Multi-source deep research using firecrawl and exa MCPs. Searches the web, synthesizes findings, and delivers cited reports with source attribution. Use when the user wants thorough research on any topic with evidence and citations.
role: deep-research
category: research
triggers:
  - deep research
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - subagent.spawn
sources:
  - research/everything-claude-code/.agents/skills/deep-research/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: deep-research
---

# deep-research

## Role

Portable distillation of upstream skill `deep-research` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Multi-source deep research using firecrawl and exa MCPs. Searches the web, synthesizes findings, and delivers cited reports with source attribution. Use when the user wants thorough research on any topic with evidence and citations.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
