---
id: everything-claude-code__ecc-tools-cost-audit
name: ecc-tools-cost-audit
version: 1.0.0
description: >-
  Evidence-first ECC Tools burn and billing audit workflow. Use when investigating runaway PR creation, quota bypass, premium-model leakage, duplicate jobs, or GitHub App cost spikes in the ECC Tools repo.
role: ecc-tools-cost-audit
category: meta
triggers:
  - ecc tools cost audit
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/ecc-tools-cost-audit/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ecc-tools-cost-audit
---

# ecc-tools-cost-audit

## Role

Portable distillation of upstream skill `ecc-tools-cost-audit` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Evidence-first ECC Tools burn and billing audit workflow. Use when investigating runaway PR creation, quota bypass, premium-model leakage, duplicate jobs, or GitHub App cost spikes in the ECC Tools repo.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
