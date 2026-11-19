---
id: everything-claude-code__living-docs-governance
name: living-docs-governance
version: 1.0.0
description: >-
  Keep a long-lived project's documentation from rotting by assigning existing project docs clear constitution, map, status, and history roles, then wiring the active agent harness to those canonical sources. Use in the maintain phase when docs drift from code, agents lose context between sessions, or intentional removals keep being recreated. Prefer adopting the repository's current docs structure over creating new root files. 中文触发：文档治理、活文档、项目状态追踪、防文档漂移、项目地图、健康仪表盘、删除区、长期项目治理
role: living-docs-governance
category: ops
triggers:
  - living docs governance
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/living-docs-governance/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: living-docs-governance
---

# living-docs-governance

## Role

Portable distillation of upstream skill `living-docs-governance` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Keep a long-lived project's documentation from rotting by assigning existing project docs clear constitution, map, status, and history roles, then wiring the active agent harness to those canonical sources. Use in the maintain phase when docs drift from code, agents lose context between sessions, or intentional removals keep being recreated. Prefer adopting the repository's current docs structure over creating new root files. 中文触发：文档治理、活文档、项目状态追踪、防文档漂移、项目地图、健康仪表盘、删除区、长期项目治理

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
