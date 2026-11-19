---
id: everything-claude-code__ito-inference
name: ito-inference
version: 1.0.0
description: >-
  Inspect the availability of model serving on a completed Itô compute booking and, when the canonical backend becomes available, hand off an explicitly confirmed serving manifest. Use after ito-compute has booked GPU nodes and the user asks for an OpenAI-compatible endpoint, ito-serve, hosted Kimi, or self-hosted open-weights inference. ECC implements no serving stack of its own.
role: ito-inference
category: meta
triggers:
  - ito inference
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/ito-inference/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: ito-inference
---

# ito-inference

## Role

Portable distillation of upstream skill `ito-inference` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Inspect the availability of model serving on a completed Itô compute booking and, when the canonical backend becomes available, hand off an explicitly confirmed serving manifest. Use after ito-compute has booked GPU nodes and the user asks for an OpenAI-compatible endpoint, ito-serve, hosted Kimi, or self-hosted open-weights inference. ECC implements no serving stack of its own.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
