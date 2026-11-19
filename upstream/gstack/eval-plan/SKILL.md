---
id: gstack__eval-plan
name: eval-plan
version: 1.0.0
description: >-
  Preregister a paid eval (bars, arms, decoys, stop rules), dry-run it at zero cost, then run a three-item priced pilot whose spend table gates approval. (gstack)
role: eval-plan
category: meta
triggers:
  - eval plan
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/gstack/eval-plan/SKILL.md
harness: any
upstream_repo: gstack
upstream_skill: eval-plan
---

# eval-plan

## Role

Portable distillation of upstream skill `eval-plan` from `gstack`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Preregister a paid eval (bars, arms, decoys, stop rules), dry-run it at zero cost, then run a three-item priced pilot whose spend table gates approval. (gstack)

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
