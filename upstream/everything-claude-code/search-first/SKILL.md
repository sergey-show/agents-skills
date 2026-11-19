---
id: everything-claude-code__search-first
name: search-first
version: 1.0.0
description: >-
  Research-before-coding workflow: search npm/PyPI, MCP servers, skills, and GitHub for existing tools before writing custom code, then adopt, extend, or build. Launches the researcher agent for non-trivial needs. Use when starting a feature, adding a dependency or integration, or about to write a utility that may already exist.
role: search-first
category: research
triggers:
  - search first
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/search-first/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: search-first
---

# search-first

## Role

Portable distillation of upstream skill `search-first` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Research-before-coding workflow: search npm/PyPI, MCP servers, skills, and GitHub for existing tools before writing custom code, then adopt, extend, or build. Launches the researcher agent for non-trivial needs. Use when starting a feature, adding a dependency or integration, or about to write a utility that may already exist.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
