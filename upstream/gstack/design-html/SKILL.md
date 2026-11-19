---
id: gstack__design-html
name: design-html
version: 1.0.0
description: >-
  Design finalization: generates production-quality Pretext-native HTML/CSS. Use for: build the design, code the mockup, make design real. (gstack)
role: design-html
category: design
triggers:
  - design html
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/gstack/design-html/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: design-html
---

# design-html

## Role

Portable distillation of upstream skill `design-html` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Design finalization: generates production-quality Pretext-native HTML/CSS. Use for: build the design, code the mockup, make design real. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
