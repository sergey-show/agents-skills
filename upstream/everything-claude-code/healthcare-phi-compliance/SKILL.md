---
id: everything-claude-code__healthcare-phi-compliance
name: healthcare-phi-compliance
version: 1.0.0
description: >-
  Protected Health Information (PHI) and PII compliance patterns for healthcare applications: data classification, row-level access control, tamper-proof audit trails, schema tagging, and common leak vectors such as logs, URLs, and browser storage. Use when code touches patient or clinician data, when implementing HIPAA or GDPR access controls, or when auditing a healthcare system for data exposure.
role: healthcare-phi-compliance
category: design
triggers:
  - healthcare phi compliance
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/healthcare-phi-compliance/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: healthcare-phi-compliance
---

# healthcare-phi-compliance

## Role

Portable distillation of upstream skill `healthcare-phi-compliance` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Protected Health Information (PHI) and PII compliance patterns for healthcare applications: data classification, row-level access control, tamper-proof audit trails, schema tagging, and common leak vectors such as logs, URLs, and browser storage. Use when code touches patient or clinician data, when implementing HIPAA or GDPR access controls, or when auditing a healthcare system for data exposure.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
