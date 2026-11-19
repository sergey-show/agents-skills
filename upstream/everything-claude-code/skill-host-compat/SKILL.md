---
id: everything-claude-code__skill-host-compat
name: skill-host-compat
version: 1.0.0
description: >-
  Lint ECC skills for Codex/the coding agent-safe frontmatter and Claude-only substitutions before a skill PR.
role: skill-host-compat
category: meta
triggers:
  - skill host compat
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/.agents/skills/skill-host-compat/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: skill-host-compat
---

# skill-host-compat

## Role

Portable distillation of upstream skill `skill-host-compat` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Lint ECC skills for Codex/the coding agent-safe frontmatter and Claude-only substitutions before a skill PR.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
