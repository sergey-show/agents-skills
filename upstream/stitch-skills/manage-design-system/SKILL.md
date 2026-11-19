---
id: stitch-skills__manage-design-system
name: stitch::manage-design-system
version: 1.0.0
description: >-
  Manage design systems in Stitch using MCP tools. Includes retrieval of assets, creating/updating design systems in Stitch, and applying them to screens.
role: stitch::manage-design-system
category: design
triggers:
  - manage design system
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - shell.exec
sources:
  - research/stitch-skills/plugins/stitch-design/skills/manage-design-system/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: manage-design-system
---

# stitch::manage-design-system

## Role

Portable distillation of upstream skill `manage-design-system` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Manage design systems in Stitch using MCP tools. Includes retrieval of assets, creating/updating design systems in Stitch, and applying them to screens.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
