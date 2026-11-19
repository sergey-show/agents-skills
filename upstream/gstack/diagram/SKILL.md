---
id: gstack__diagram
name: diagram
version: 1.0.0
description: >-
  Turn an English description (or mermaid source) into a diagram triplet: the source, an editable .excalidraw file you can open on excalidraw.com, and rendered SVG + PNG. Use for: make a diagram, draw a diagram. (gstack)
role: diagram
category: meta
triggers:
  - diagram
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/gstack/diagram/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: diagram
---

# diagram

## Role

Portable distillation of upstream skill `diagram` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Turn an English description (or mermaid source) into a diagram triplet: the source, an editable .excalidraw file you can open on excalidraw.com, and rendered SVG + PNG. Use for: make a diagram, draw a diagram. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
