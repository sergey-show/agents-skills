---
id: everything-claude-code__ios-icon-gen
name: ios-icon-gen
version: 1.0.0
description: >-
  Generate iOS app icons as PNG imagesets for Xcode asset catalogs from SF Symbols (5000+ Apple-native) or Iconify API (275k+ open source icons from 200+ collections). Use when generating icons, creating icon assets, adding icons to asset catalog, or searching for icons for iOS projects.
role: ios-icon-gen
category: engineering
triggers:
  - ios icon gen
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/skills/ios-icon-gen/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ios-icon-gen
---

# ios-icon-gen

## Role

Portable distillation of upstream skill `ios-icon-gen` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Generate iOS app icons as PNG imagesets for Xcode asset catalogs from SF Symbols (5000+ Apple-native) or Iconify API (275k+ open source icons from 200+ collections). Use when generating icons, creating icon assets, adding icons to asset catalog, or searching for icons for iOS projects.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
