---
id: mattpocock-skills__scaffold-exercises
name: scaffold-exercises
version: 1.0.0
description: >-
  Create exercise directory structures with sections, problems, solutions, and explainers that pass linting. Use when user wants to scaffold exercises, create exercise stubs, or set up a new course section.
role: scaffold-exercises
category: meta
triggers:
  - scaffold exercises
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
sources:
  - research/skills/skills/misc/scaffold-exercises/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: scaffold-exercises
---

# scaffold-exercises

## Role

Portable distillation of upstream skill `scaffold-exercises` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Create exercise directory structures with sections, problems, solutions, and explainers that pass linting. Use when user wants to scaffold exercises, create exercise stubs, or set up a new course section.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
