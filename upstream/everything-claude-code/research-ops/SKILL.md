---
id: everything-claude-code__research-ops
name: research-ops
version: 1.0.0
description: >-
  Evidence-first current-state research workflow for ECC. Use when the user wants fresh facts, comparisons, enrichment, or a recommendation built from current public evidence and any supplied local context.
role: research-ops
category: research
triggers:
  - research ops
capabilities_required:
  - filesystem.read
  - search.code
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/skills/research-ops/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: research-ops
---

# research-ops

## Role

Portable distillation of upstream skill `research-ops` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Evidence-first current-state research workflow for ECC. Use when the user wants fresh facts, comparisons, enrichment, or a recommendation built from current public evidence and any supplied local context.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
