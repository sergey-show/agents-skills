---
id: everything-claude-code__hookify-rules
name: hookify-rules
version: 1.0.0
description: >-
  Create and configure hookify rules — markdown files with YAML frontmatter that match bash, file, prompt, or stop events by regex or conditions and show warn/block messages to the agent. Use when creating a hookify rule, writing hook rule syntax, configuring hookify, or adding pattern guardrails such as blocking dangerous commands, .env edits, or debug code.
role: hookify-rules
category: meta
triggers:
  - hookify rules
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/hookify-rules/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: hookify-rules
---

# hookify-rules

## Role

Portable distillation of upstream skill `hookify-rules` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Create and configure hookify rules — markdown files with YAML frontmatter that match bash, file, prompt, or stop events by regex or conditions and show warn/block messages to the agent. Use when creating a hookify rule, writing hook rule syntax, configuring hookify, or adding pattern guardrails such as blocking dangerous commands, .env edits, or debug code.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
