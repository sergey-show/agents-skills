---
id: everything-claude-code__security-review
name: security-review
version: 1.0.0
description: >-
  Security review checklist and patterns for adding authentication, handling user input, managing secrets, creating API endpoints, or implementing payment and sensitive features.
role: security-review
category: security
triggers:
  - security review
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/security-review/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: security-review
---

# security-review

## Role

Portable distillation of upstream skill `security-review` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Security review checklist and patterns for adding authentication, handling user input, managing secrets, creating API endpoints, or implementing payment and sensitive features.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
