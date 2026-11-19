---
id: everything-claude-code__repo-scan
name: repo-scan
version: 1.0.0
description: >-
  Bootstrap pointer that installs the external repo-scan skill from a pinned, reviewable commit. Use when repo-scan must be installed before running its cross-stack source-code asset audit; this ECC pointer does not perform the audit itself.
role: repo-scan
category: engineering
triggers:
  - repo scan
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
sources:
  - research/everything-claude-code/skills/repo-scan/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: repo-scan
---

# repo-scan

## Role

Portable distillation of upstream skill `repo-scan` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Bootstrap pointer that installs the external repo-scan skill from a pinned, reviewable commit. Use when repo-scan must be installed before running its cross-stack source-code asset audit; this ECC pointer does not perform the audit itself.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
