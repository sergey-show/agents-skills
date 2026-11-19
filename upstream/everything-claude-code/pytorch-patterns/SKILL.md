---
id: everything-claude-code__pytorch-patterns
name: pytorch-patterns
version: 1.0.0
description: >-
  PyTorch deep learning patterns and best practices for building robust, efficient, and reproducible training pipelines, model architectures, and data loading. Use when writing or reviewing PyTorch training loops, model architectures, or data loading, or when a run will not reproduce.
role: pytorch-patterns
category: meta
triggers:
  - pytorch patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/pytorch-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: pytorch-patterns
---

# pytorch-patterns

## Role

Portable distillation of upstream skill `pytorch-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

PyTorch deep learning patterns and best practices for building robust, efficient, and reproducible training pipelines, model architectures, and data loading. Use when writing or reviewing PyTorch training loops, model architectures, or data loading, or when a run will not reproduce.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
