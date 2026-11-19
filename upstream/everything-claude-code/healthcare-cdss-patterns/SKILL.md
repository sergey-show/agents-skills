---
id: everything-claude-code__healthcare-cdss-patterns
name: healthcare-cdss-patterns
version: 1.0.0
description: >-
  Clinical Decision Support System (CDSS) development patterns. Drug interaction checking, dose validation, clinical scoring (NEWS2, qSOFA), alert severity classification, and integration into EMR workflows. Use when building clinical decision support — drug interaction checks, dose validation, clinical scoring, or alert severity.
role: healthcare-cdss-patterns
category: design
triggers:
  - healthcare cdss patterns
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - test.run
sources:
  - research/everything-claude-code/skills/healthcare-cdss-patterns/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: healthcare-cdss-patterns
---

# healthcare-cdss-patterns

## Role

Portable distillation of upstream skill `healthcare-cdss-patterns` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Clinical Decision Support System (CDSS) development patterns. Drug interaction checking, dose validation, clinical scoring (NEWS2, qSOFA), alert severity classification, and integration into EMR workflows. Use when building clinical decision support — drug interaction checks, dose validation, clinical scoring, or alert severity.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
