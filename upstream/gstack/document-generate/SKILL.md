---
id: gstack__document-generate
name: document-generate
version: 1.0.0
description: >-
  Generate missing documentation from scratch for a feature, module, or entire project. Use for: write docs for this, generate documentation. (gstack)
role: document-generate
category: meta
triggers:
  - document generate
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/gstack/document-generate/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: document-generate
---

# document-generate

## Role

Portable distillation of upstream skill `document-generate` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Generate missing documentation from scratch for a feature, module, or entire project. Use for: write docs for this, generate documentation. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
