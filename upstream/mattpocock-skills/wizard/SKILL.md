---
id: mattpocock-skills__wizard
name: wizard
version: 1.0.0
description: >-
  Generate an interactive bash wizard that walks a human through steps only they can perform. Use when provisioning infrastructure, setting up credentials or CI secrets, walking an unfamiliar third-party dashboard, or running a one-off migration or cutover. Don't invoke this for steps the agent can perform itself.
role: wizard
category: engineering
triggers:
  - wizard
capabilities_required:
  - filesystem.edit
  - filesystem.read
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - shell.exec
  - test.run
sources:
  - research/skills/skills/engineering/wizard/SKILL.md
harness: any
upstream_repo: mattpocock-skills
upstream_skill: wizard
---

# wizard

## Role

Portable distillation of upstream skill `wizard` from `mattpocock-skills`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Generate an interactive bash wizard that walks a human through steps only they can perform. Use when provisioning infrastructure, setting up credentials or CI secrets, walking an unfamiliar third-party dashboard, or running a one-off migration or cutover. Don't invoke this for steps the agent can perform itself.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
