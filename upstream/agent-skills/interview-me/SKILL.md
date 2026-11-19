---
id: agent-skills__interview-me
name: interview-me
version: 1.0.0
description: >-
  Extracts what the user actually wants instead of what they think they should want. Achieves this through one-question-at-a-time interview until ~95% confidence about the underlying intent. Use when an ask is underspecified ("build me X" without "for whom" or "why now"), when the user explicitly invokes ("interview me", "grill me", "are we sure?", "stress-test my thinking"), or when you catch yourself silently filling in ambiguous requirements before any plan, spec, or code exists.
role: interview-me
category: engineering
triggers:
  - interview me
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/agent-skills/skills/interview-me/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: interview-me
---

# interview-me

## Role

Portable distillation of upstream skill `interview-me` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Extracts what the user actually wants instead of what they think they should want. Achieves this through one-question-at-a-time interview until ~95% confidence about the underlying intent. Use when an ask is underspecified ("build me X" without "for whom" or "why now"), when the user explicitly invokes ("interview me", "grill me", "are we sure?", "stress-test my thinking"), or when you catch yourself silently filling in ambiguous requirements before any plan, spec, or code exists.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
