---
id: gstack__ios-design-review
name: ios-design-review
version: 1.0.0
description: >-
  Visual design audit for iOS apps on real hardware. Use for: review the ios design, audit the iphone app visuals. (gstack)
role: ios-design-review
category: design
triggers:
  - ios design review
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
  - research/gstack/ios-design-review/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: ios-design-review
---

# ios-design-review

## Role

Portable distillation of upstream skill `ios-design-review` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Visual design audit for iOS apps on real hardware. Use for: review the ios design, audit the iphone app visuals. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
