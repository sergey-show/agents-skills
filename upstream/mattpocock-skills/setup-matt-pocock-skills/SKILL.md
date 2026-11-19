---
id: mattpocock-skills__setup-matt-pocock-skills
name: setup-matt-pocock-skills
version: 1.0.0
description: >-
  Configure this repo for the engineering skills: set up its issue tracker, triage label vocabulary, and domain doc layout. Run once before first use of the other engineering skills.
role: setup-matt-pocock-skills
category: meta
triggers:
  - setup matt pocock skills
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - search.web
sources:
  - research/skills/skills/engineering/setup-matt-pocock-skills/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: setup-matt-pocock-skills
---

# setup-matt-pocock-skills

## Role

Portable distillation of upstream skill `setup-matt-pocock-skills` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Configure this repo for the engineering skills: set up its issue tracker, triage label vocabulary, and domain doc layout. Run once before first use of the other engineering skills.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
