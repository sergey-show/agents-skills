---
id: rea__rea-tool-design
name: rea-tool-design
version: 1.0.0
description: >-
  Audit, investigate, design, or change REA investigation tools, CLI/MCP contracts, provider capabilities, and Evidence semantics.
role: rea-tool-design
category: design
triggers:
  - rea tool design
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/rea/.agents/skills/rea-tool-design/SKILL.md
harness: any
upstream_repo: rea
upstream_skill: rea-tool-design
---

# rea-tool-design

## Role

Portable distillation of upstream skill `rea-tool-design` from `rea`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Audit, investigate, design, or change REA investigation tools, CLI/MCP contracts, provider capabilities, and Evidence semantics.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
