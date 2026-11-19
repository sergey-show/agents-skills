---
id: everything-claude-code__configure-ecc
name: configure-ecc
version: 1.0.0
description: >-
  Run the conversational ECC setup wizard inside the current harness: inventory the install, collect scope (user/project/local) and hook mode (off/minimal/standard/strict) in the coding agent, use Codex's native plugin lifecycle, or install the project surface under ./.kimi-code, then preview, apply, and verify. Use when installing, updating, reconfiguring, or repairing an ECC installation, changing hook profiles, or moving ECC between install scopes.
role: configure-ecc
category: engineering
triggers:
  - configure ecc
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/configure-ecc/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: configure-ecc
---

# configure-ecc

## Role

Portable distillation of upstream skill `configure-ecc` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Run the conversational ECC setup wizard inside the current harness: inventory the install, collect scope (user/project/local) and hook mode (off/minimal/standard/strict) in the coding agent, use Codex's native plugin lifecycle, or install the project surface under ./.kimi-code, then preview, apply, and verify. Use when installing, updating, reconfiguring, or repairing an ECC installation, changing hook profiles, or moving ECC between install scopes.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
