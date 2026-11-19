---
id: everything-claude-code__esign-field-placement
name: esign-field-placement
version: 1.0.0
description: >-
  Deterministic method for placing signature, date, and text fields in a web e-signature composer through a browser automation session, using a fixed signature page, numeric Location panel coordinates instead of drag, and a save-as-draft default. Use when automating envelope preparation for generated agreements and you need repeatable field positions, correct per-recipient ownership, and a hard gate before anything is sent or signed.
role: esign-field-placement
category: ops
triggers:
  - esign field placement
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/esign-field-placement/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: esign-field-placement
---

# esign-field-placement

## Role

Portable distillation of upstream skill `esign-field-placement` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Deterministic method for placing signature, date, and text fields in a web e-signature composer through a browser automation session, using a fixed signature page, numeric Location panel coordinates instead of drag, and a save-as-draft default. Use when automating envelope preparation for generated agreements and you need repeatable field positions, correct per-recipient ownership, and a hard gate before anything is sent or signed.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
