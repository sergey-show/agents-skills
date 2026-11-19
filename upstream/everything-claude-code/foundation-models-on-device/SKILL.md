---
id: everything-claude-code__foundation-models-on-device
name: foundation-models-on-device
version: 1.0.0
description: >-
  Apple FoundationModels framework for on-device LLM — text generation, guided generation with @Generable, tool calling, and snapshot streaming in iOS 26+. Use when adding on-device LLM features with Apple FoundationModels on iOS 26+.
role: foundation-models-on-device
category: engineering
triggers:
  - foundation models on device
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
sources:
  - research/everything-claude-code/skills/foundation-models-on-device/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: foundation-models-on-device
---

# foundation-models-on-device

## Role

Portable distillation of upstream skill `foundation-models-on-device` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Apple FoundationModels framework for on-device LLM — text generation, guided generation with @Generable, tool calling, and snapshot streaming in iOS 26+. Use when adding on-device LLM features with Apple FoundationModels on iOS 26+.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
