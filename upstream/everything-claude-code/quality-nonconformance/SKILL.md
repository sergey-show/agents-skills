---
id: everything-claude-code__quality-nonconformance
name: quality-nonconformance
version: 1.0.0
description: >-
  Quality control and non-conformance management for regulated manufacturing (FDA 21 CFR 820, IATF 16949, AS9100): NCR lifecycle and disposition, 5-Why/Ishikawa/fault-tree/8D root cause analysis, CAPA systems, SPC interpretation, AQL sampling, and supplier quality audits. Use when investigating non-conformances, performing root cause analysis, managing CAPAs, interpreting SPC data, or handling supplier quality issues.
role: quality-nonconformance
category: engineering
triggers:
  - quality nonconformance
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/quality-nonconformance/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: quality-nonconformance
---

# quality-nonconformance

## Role

Portable distillation of upstream skill `quality-nonconformance` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Quality control and non-conformance management for regulated manufacturing (FDA 21 CFR 820, IATF 16949, AS9100): NCR lifecycle and disposition, 5-Why/Ishikawa/fault-tree/8D root cause analysis, CAPA systems, SPC interpretation, AQL sampling, and supplier quality audits. Use when investigating non-conformances, performing root cause analysis, managing CAPAs, interpreting SPC data, or handling supplier quality issues.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
