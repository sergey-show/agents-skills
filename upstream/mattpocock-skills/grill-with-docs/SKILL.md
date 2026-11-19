---
id: mattpocock-skills__grill-with-docs
name: grill-with-docs
version: 1.0.0
description: >-
  A relentless interview to sharpen a plan or design, which also creates docs (ADR's and glossary) as we go.
role: grill-with-docs
category: meta
triggers:
  - grill with docs
capabilities_required:
  - filesystem.read
capabilities_optional:
  []
sources:
  - research/skills/skills/engineering/grill-with-docs/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: grill-with-docs
---

# grill-with-docs

## Role

Portable distillation of upstream skill `grill-with-docs` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

A relentless interview to sharpen a plan or design, which also creates docs (ADR's and glossary) as we go.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
