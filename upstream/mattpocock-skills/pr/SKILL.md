---
id: mattpocock-skills__pr
name: pr
version: 1.0.0
description: >-
  Use when writing a PR body.
role: pr
category: engineering
triggers:
  - pr
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/skills/skills/engineering/pr/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: pr
---

# pr

## Role

Portable distillation of upstream skill `pr` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use when writing a PR body.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
