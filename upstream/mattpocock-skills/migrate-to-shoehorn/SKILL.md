---
id: mattpocock-skills__migrate-to-shoehorn
name: migrate-to-shoehorn
version: 1.0.0
description: >-
  Migrate test files from `as` type assertions to @total-typescript/shoehorn. Use when user mentions shoehorn, wants to replace `as` in tests, or needs partial test data.
role: migrate-to-shoehorn
category: engineering
triggers:
  - migrate to shoehorn
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/skills/skills/misc/migrate-to-shoehorn/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: migrate-to-shoehorn
---

# migrate-to-shoehorn

## Role

Portable distillation of upstream skill `migrate-to-shoehorn` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Migrate test files from `as` type assertions to @total-typescript/shoehorn. Use when user mentions shoehorn, wants to replace `as` in tests, or needs partial test data.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
