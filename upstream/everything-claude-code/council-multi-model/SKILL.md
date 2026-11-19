---
id: everything-claude-code__council-multi-model
name: council-multi-model
version: 1.0.0
description: >-
  Add one optional external Codex critique after the existing council has produced a decision draft. Use when an ambiguous, high-consequence decision would benefit from a separate model invocation's attempt to break the synthesis. Requires explicit consent before sending the compact draft and disagreement to OpenAI, labels same-provider reviews honestly, and marks the review absent when the adapter is unavailable.
role: council-multi-model
category: meta
triggers:
  - council multi model
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/council-multi-model/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: council-multi-model
---

# council-multi-model

## Role

Portable distillation of upstream skill `council-multi-model` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Add one optional external Codex critique after the existing council has produced a decision draft. Use when an ambiguous, high-consequence decision would benefit from a separate model invocation's attempt to break the synthesis. Requires explicit consent before sending the compact draft and disagreement to OpenAI, labels same-provider reviews honestly, and marks the review absent when the adapter is unavailable.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
