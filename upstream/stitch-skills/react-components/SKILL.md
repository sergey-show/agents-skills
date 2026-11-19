---
id: stitch-skills__react-components
name: stitch::react-components
version: 1.0.0
description: >-
  Converts Stitch designs into modular Vite and React components, or syncs/updates existing React components to align with the latest Stitch designs, using system-level networking and AST-based validation.
role: stitch::react-components
category: design
triggers:
  - react components
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - test.run
sources:
  - research/stitch-skills/plugins/stitch-build/skills/react-components/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: react-components
---

# stitch::react-components

## Role

Portable distillation of upstream skill `react-components` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Converts Stitch designs into modular Vite and React components, or syncs/updates existing React components to align with the latest Stitch designs, using system-level networking and AST-based validation.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
