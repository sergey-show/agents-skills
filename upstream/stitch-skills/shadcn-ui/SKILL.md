---
id: stitch-skills__shadcn-ui
name: shadcn-ui
version: 1.0.0
description: >-
  Expert guidance for integrating and building applications with shadcn/ui components, including component discovery, installation, customization, and best practices.
role: shadcn-ui
category: design
triggers:
  - shadcn ui
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/stitch-skills/plugins/stitch-build/skills/shadcn-ui/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: shadcn-ui
---

# shadcn-ui

## Role

Portable distillation of upstream skill `shadcn-ui` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Expert guidance for integrating and building applications with shadcn/ui components, including component discovery, installation, customization, and best practices.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
