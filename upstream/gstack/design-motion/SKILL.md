---
id: gstack__design-motion
name: design-motion
version: 1.0.0
description: >-
  Design motion: animate an approved design into a seamless MP4 and GIF loop. Use for: animate this design, make a showcase loop. (gstack)
role: design-motion
category: design
triggers:
  - design motion
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/gstack/design-motion/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: design-motion
---

# design-motion

## Role

Portable distillation of upstream skill `design-motion` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Design motion: animate an approved design into a seamless MP4 and GIF loop. Use for: animate this design, make a showcase loop. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
