---
id: everything-claude-code__healthcare-emr-patterns
name: healthcare-emr-patterns
version: 1.0.0
description: >-
  EMR/EHR development patterns for healthcare applications. Clinical safety, encounter workflows, prescription generation, clinical decision support integration, and accessibility-first UI for medical data entry. Use when building EMR or EHR features such as encounter workflows, prescription generation, or clinical data entry UI.
role: healthcare-emr-patterns
category: design
triggers:
  - healthcare emr patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
sources:
  - research/everything-claude-code/skills/healthcare-emr-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: healthcare-emr-patterns
---

# healthcare-emr-patterns

## Role

Portable distillation of upstream skill `healthcare-emr-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

EMR/EHR development patterns for healthcare applications. Clinical safety, encounter workflows, prescription generation, clinical decision support integration, and accessibility-first UI for medical data entry. Use when building EMR or EHR features such as encounter workflows, prescription generation, or clinical data entry UI.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
