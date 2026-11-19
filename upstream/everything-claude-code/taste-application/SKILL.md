---
id: everything-claude-code__taste-application
name: taste-application
version: 1.0.0
description: >-
  Generate new video against a distilled style pack and cut it into a finished piece - plan takes from the reference's cut rhythm, generate on fal, grade with the pack's measured LUT, cut at the measured cadence, weave in existing footage, composite overlay plates, mint 3D props, and verify the result numerically. Use when the user wants to make a video in a captured style, supplement existing footage, or assemble generated clips into a real edit.
role: taste-application
category: ops
triggers:
  - taste application
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
sources:
  - research/everything-claude-code/skills/taste-application/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: taste-application
---

# taste-application

## Role

Portable distillation of upstream skill `taste-application` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Generate new video against a distilled style pack and cut it into a finished piece - plan takes from the reference's cut rhythm, generate on fal, grade with the pack's measured LUT, cut at the measured cadence, weave in existing footage, composite overlay plates, mint 3D props, and verify the result numerically. Use when the user wants to make a video in a captured style, supplement existing footage, or assemble generated clips into a real edit.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
