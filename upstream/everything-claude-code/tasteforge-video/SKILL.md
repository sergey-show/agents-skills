---
id: everything-claude-code__tasteforge-video
name: tasteforge-video
version: 1.0.0
description: >-
  Use for file-driven multimodal image, video, and 3D-asset discovery; taste interviews; distill or apply workflows; style-pack validation; editable EDL/FCPXML export; provenance audits; and offline planning that must fail closed before provider generation.
role: tasteforge-video
category: ops
triggers:
  - tasteforge video
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/tasteforge-video/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: tasteforge-video
---

# tasteforge-video

## Role

Portable distillation of upstream skill `tasteforge-video` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Use for file-driven multimodal image, video, and 3D-asset discovery; taste interviews; distill or apply workflows; style-pack validation; editable EDL/FCPXML export; provenance audits; and offline planning that must fail closed before provider generation.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
