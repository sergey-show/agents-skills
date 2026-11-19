---
id: everything-claude-code__mailtrap-email-integration
name: mailtrap-email-integration
version: 1.0.0
description: >-
  Guides agents through integrating transactional email sending via Mailtrap's Email API, including sandbox testing, domain verification, and API authentication. Use when implementing email-sending features, debugging delivery issues, or setting up safe dev/staging email testing.
role: mailtrap-email-integration
category: engineering
triggers:
  - mailtrap email integration
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - git.ops
  - search.web
  - test.run
sources:
  - research/everything-claude-code/skills/mailtrap-email-integration/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: mailtrap-email-integration
---

# mailtrap-email-integration

## Role

Portable distillation of upstream skill `mailtrap-email-integration` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Guides agents through integrating transactional email sending via Mailtrap's Email API, including sandbox testing, domain verification, and API authentication. Use when implementing email-sending features, debugging delivery issues, or setting up safe dev/staging email testing.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
