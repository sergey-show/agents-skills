---
id: everything-claude-code__gan-style-harness
name: gan-style-harness
version: 1.0.0
description: >-
  GAN-inspired Generator-Evaluator agent harness for building high-quality applications autonomously. Based on Anthropic's March 2026 harness design paper. Use when a feature should be built autonomously through generator and evaluator iteration until it clears a quality bar.
role: gan-style-harness
category: design
triggers:
  - gan style harness
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/gan-style-harness/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: gan-style-harness
---

# gan-style-harness

## Role

Portable distillation of upstream skill `gan-style-harness` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

GAN-inspired Generator-Evaluator agent harness for building high-quality applications autonomously. Based on Anthropic's March 2026 harness design paper. Use when a feature should be built autonomously through generator and evaluator iteration until it clears a quality bar.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
