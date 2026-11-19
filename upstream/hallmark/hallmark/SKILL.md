---
id: hallmark__hallmark
name: hallmark
version: 1.0.0
description: >-
  Design skill for websites and new pages that look designed, not generated. Use when the user asks to build or design something new, or names Hallmark. Never use it on an existing design unless the user names Hallmark, as in `/hallmark redesign <path>`.
role: hallmark
category: design
triggers:
  - hallmark
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/hallmark/skills/hallmark/SKILL.md
harness: any
upstream_repo: hallmark
upstream_skill: hallmark
---

# hallmark

## Role

Portable distillation of upstream skill `hallmark` from `hallmark`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Design skill for websites and new pages that look designed, not generated. Use when the user asks to build or design something new, or names Hallmark. Never use it on an existing design unless the user names Hallmark, as in `/hallmark redesign <path>`.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
