---
id: everything-claude-code__automation-audit-ops
name: automation-audit-ops
version: 1.0.0
description: >-
  Evidence-first automation inventory and overlap audit workflow for ECC. Use when the user wants to know which jobs, hooks, connectors, MCP servers, or wrappers are live, broken, redundant, or missing before fixing anything.
role: automation-audit-ops
category: meta
triggers:
  - automation audit ops
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
sources:
  - research/everything-claude-code/skills/automation-audit-ops/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: automation-audit-ops
---

# automation-audit-ops

## Role

Portable distillation of upstream skill `automation-audit-ops` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Evidence-first automation inventory and overlap audit workflow for ECC. Use when the user wants to know which jobs, hooks, connectors, MCP servers, or wrappers are live, broken, redundant, or missing before fixing anything.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
