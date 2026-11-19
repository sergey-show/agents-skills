---
id: mattpocock-skills__prototype
name: prototype
version: 1.0.0
description: >-
  Build a throwaway prototype to answer a design question. Use when the user wants to sanity-check whether a state model or logic feels right, or explore what a UI should look like.
role: prototype
category: engineering
triggers:
  - prototype
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/skills/skills/engineering/prototype/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: prototype
---

# prototype

## Role

Portable distillation of upstream skill `prototype` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Build a throwaway prototype to answer a design question. Use when the user wants to sanity-check whether a state model or logic feels right, or explore what a UI should look like.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
