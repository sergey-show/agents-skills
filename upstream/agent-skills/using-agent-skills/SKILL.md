---
id: agent-skills__using-agent-skills
name: using-agent-skills
version: 1.0.0
description: >-
  Discovers and invokes agent skills. Use when starting a session, or when you need to decide which skill or workflow applies to the piece of work at hand. This is the meta-skill that governs how all other skills are discovered and invoked.
role: using-agent-skills
category: meta
triggers:
  - using agent skills
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - test.run
sources:
  - research/agent-skills/skills/using-agent-skills/SKILL.md
harness: any
upstream_repo: agent-skills
upstream_skill: using-agent-skills
---

# using-agent-skills

## Role

Portable distillation of upstream skill `using-agent-skills` from `agent-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Discovers and invokes agent skills. Use when starting a session, or when you need to decide which skill or workflow applies to the piece of work at hand. This is the meta-skill that governs how all other skills are discovered and invoked.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
