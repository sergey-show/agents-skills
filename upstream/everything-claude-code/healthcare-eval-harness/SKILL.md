---
id: everything-claude-code__healthcare-eval-harness
name: healthcare-eval-harness
version: 1.0.0
description: >-
  Patient safety evaluation harness for healthcare application deployments. Automated test suites for CDSS accuracy, PHI exposure, clinical workflow integrity, and integration compliance. Blocks deployments on safety failures. Use when a healthcare deployment must be gated on patient-safety tests for CDSS accuracy, PHI exposure, and workflow integrity.
role: healthcare-eval-harness
category: ops
triggers:
  - healthcare eval harness
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/healthcare-eval-harness/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: healthcare-eval-harness
---

# healthcare-eval-harness

## Role

Portable distillation of upstream skill `healthcare-eval-harness` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Patient safety evaluation harness for healthcare application deployments. Automated test suites for CDSS accuracy, PHI exposure, clinical workflow integrity, and integration compliance. Blocks deployments on safety failures. Use when a healthcare deployment must be gated on patient-safety tests for CDSS accuracy, PHI exposure, and workflow integrity.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
