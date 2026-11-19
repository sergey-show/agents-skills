---
id: mattpocock-skills__domain-modeling
name: domain-modeling
version: 1.0.0
description: >-
  Build and sharpen a project's domain model. Use when discussing codebase terminology, writing or editing a GLOSSARY.md, or recording or editing an ADR.
role: domain-modeling
category: design
triggers:
  - domain modeling
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/skills/skills/engineering/domain-modeling/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: domain-modeling
---

# domain-modeling

## Role

Portable distillation of upstream skill `domain-modeling` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Build and sharpen a project's domain model. Use when discussing codebase terminology, writing or editing a GLOSSARY.md, or recording or editing an ADR.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
