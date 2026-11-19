---
id: stitch-skills__stitch-loop
name: stitch-loop
version: 1.0.0
description: >-
  Teaches agents to iteratively build websites using Stitch with an autonomous baton-passing loop pattern
role: stitch-loop
category: design
triggers:
  - stitch loop
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - subagent.spawn
sources:
  - research/stitch-skills/plugins/stitch-utilities/skills/stitch-loop/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: stitch-loop
---

# stitch-loop

## Role

Portable distillation of upstream skill `stitch-loop` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Teaches agents to iteratively build websites using Stitch with an autonomous baton-passing loop pattern

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
