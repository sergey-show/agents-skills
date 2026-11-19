---
id: everything-claude-code__hipaa-compliance
name: hipaa-compliance
version: 1.0.0
description: >-
  HIPAA-specific entrypoint for healthcare privacy and security work. Use when a task is explicitly framed around HIPAA, PHI handling, covered entities, BAAs, breach posture, or US healthcare compliance requirements.
role: hipaa-compliance
category: security
triggers:
  - hipaa compliance
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
sources:
  - research/everything-claude-code/skills/hipaa-compliance/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: hipaa-compliance
---

# hipaa-compliance

## Role

Portable distillation of upstream skill `hipaa-compliance` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

HIPAA-specific entrypoint for healthcare privacy and security work. Use when a task is explicitly framed around HIPAA, PHI handling, covered entities, BAAs, breach posture, or US healthcare compliance requirements.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
