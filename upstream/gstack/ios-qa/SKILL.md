---
id: gstack__ios-qa
name: ios-qa
version: 1.0.0
description: >-
  Live-device iOS QA for SwiftUI apps. Use for: ios qa, test the iphone app, test the ipad app. (gstack)
role: ios-qa
category: meta
triggers:
  - ios qa
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/gstack/ios-qa/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: ios-qa
---

# ios-qa

## Role

Portable distillation of upstream skill `ios-qa` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Live-device iOS QA for SwiftUI apps. Use for: ios qa, test the iphone app, test the ipad app. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
