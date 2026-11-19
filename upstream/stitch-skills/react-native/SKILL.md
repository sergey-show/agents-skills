---
id: stitch-skills__react-native
name: stitch::react-native
version: 1.0.0
description: >-
  Convert Stitch HTML designs to React Native components, or syncs/updates existing native components to align with the latest Stitch designs, using StyleSheet.
role: stitch::react-native
category: design
triggers:
  - react native
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - test.run
sources:
  - research/stitch-skills/plugins/stitch-build/skills/react-native/SKILL.md
harness: any
upstream_repo: stitch-skills
upstream_skill: react-native
---

# stitch::react-native

## Role

Portable distillation of upstream skill `react-native` from `stitch-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Convert Stitch HTML designs to React Native components, or syncs/updates existing native components to align with the latest Stitch designs, using StyleSheet.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
