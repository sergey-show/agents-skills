---
id: everything-claude-code__osint-investigation
name: osint-investigation
version: 1.0.0
description: >-
  Sparse-clue OSINT investigation methodology for extracting overlooked leads, connecting fragmented evidence, and testing explanations across sources. Use for multi-step CTF challenges, image/video geolocation, event reconstruction, public-account and entity verification, artifact interpretation, infrastructure research, or stalled investigations.
role: osint-investigation
category: engineering
triggers:
  - osint investigation
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - test.run
sources:
  - research/everything-claude-code/skills/osint-investigation/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: osint-investigation
---

# osint-investigation

## Role

Portable distillation of upstream skill `osint-investigation` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Sparse-clue OSINT investigation methodology for extracting overlooked leads, connecting fragmented evidence, and testing explanations across sources. Use for multi-step CTF challenges, image/video geolocation, event reconstruction, public-account and entity verification, artifact interpretation, infrastructure research, or stalled investigations.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
