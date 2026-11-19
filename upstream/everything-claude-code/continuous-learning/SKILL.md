---
id: everything-claude-code__continuous-learning
name: continuous-learning
version: 1.0.0
description: >-
  [DEPRECATED - use continuous-learning-v2] Legacy v1 stop-hook skill extractor. v2 is a strict superset with instinct-based, project-scoped, hook-reliable learning. Do not invoke v1: when continuous learning, session learning, or pattern extraction is requested, route to continuous-learning-v2 instead.
role: continuous-learning
category: meta
triggers:
  - continuous learning
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/continuous-learning/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: continuous-learning
---

# continuous-learning

## Role

Portable distillation of upstream skill `continuous-learning` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

[DEPRECATED - use continuous-learning-v2] Legacy v1 stop-hook skill extractor. v2 is a strict superset with instinct-based, project-scoped, hook-reliable learning. Do not invoke v1: when continuous learning, session learning, or pattern extraction is requested, route to continuous-learning-v2 instead.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
