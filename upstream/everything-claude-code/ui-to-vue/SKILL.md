---
id: everything-claude-code__ui-to-vue
name: ui-to-vue
version: 1.0.0
description: >-
  Use when the user has UI screenshots or design exports that need batch conversion into Vue 3 components, especially with Vant, Element Plus, or Ant Design Vue.
role: ui-to-vue
category: design
triggers:
  - ui to vue
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/ui-to-vue/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ui-to-vue
---

# ui-to-vue

## Role

Portable distillation of upstream skill `ui-to-vue` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when the user has UI screenshots or design exports that need batch conversion into Vue 3 components, especially with Vant, Element Plus, or Ant Design Vue.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
