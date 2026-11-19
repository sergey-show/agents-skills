---
id: everything-claude-code__workspace-surface-audit
name: workspace-surface-audit
version: 1.0.0
description: >-
  Audit the active repo, MCP servers, plugins, connectors, env surfaces, and harness setup, then recommend the highest-value ECC-native skills, hooks, agents, and operator workflows. Use when the user wants help setting up the coding agent or understanding what capabilities are actually available in their environment.
role: workspace-surface-audit
category: meta
triggers:
  - workspace surface audit
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/skills/workspace-surface-audit/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: workspace-surface-audit
---

# workspace-surface-audit

## Role

Portable distillation of upstream skill `workspace-surface-audit` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Audit the active repo, MCP servers, plugins, connectors, env surfaces, and harness setup, then recommend the highest-value ECC-native skills, hooks, agents, and operator workflows. Use when the user wants help setting up the coding agent or understanding what capabilities are actually available in their environment.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
