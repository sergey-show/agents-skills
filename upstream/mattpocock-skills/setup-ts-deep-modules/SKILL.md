---
id: mattpocock-skills__setup-ts-deep-modules
name: setup-ts-deep-modules
version: 1.0.0
description: >-
  Wire dependency-cruiser into a TypeScript repo so each package is a deep module, with implementation hidden in subfolders and reachable only through its entry-point files. User-invoked.
role: setup-ts-deep-modules
category: meta
triggers:
  - setup ts deep modules
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/skills/skills/in-progress/setup-ts-deep-modules/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: setup-ts-deep-modules
---

# setup-ts-deep-modules

## Role

Portable distillation of upstream skill `setup-ts-deep-modules` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Wire dependency-cruiser into a TypeScript repo so each package is a deep module, with implementation hidden in subfolders and reachable only through its entry-point files. User-invoked.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
