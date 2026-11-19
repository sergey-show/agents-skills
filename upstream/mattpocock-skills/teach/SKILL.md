---
id: mattpocock-skills__teach
name: teach
version: 1.0.0
description: >-
  Teach the user a new skill or concept, within this workspace.
role: teach
category: meta
triggers:
  - teach
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - test.run
sources:
  - research/skills/skills/productivity/teach/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: teach
---

# teach

## Role

Portable distillation of upstream skill `teach` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Teach the user a new skill or concept, within this workspace.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
