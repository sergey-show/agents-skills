---
id: mattpocock-skills__to-spec
name: to-spec
version: 1.0.0
description: >-
  Turn the current conversation into a spec and publish it to the project issue tracker: no interview, just synthesis of what you've already discussed.
role: to-spec
category: meta
triggers:
  - to spec
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - test.run
sources:
  - research/skills/skills/engineering/to-spec/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: to-spec
---

# to-spec

## Role

Portable distillation of upstream skill `to-spec` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Turn the current conversation into a spec and publish it to the project issue tracker: no interview, just synthesis of what you've already discussed.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
