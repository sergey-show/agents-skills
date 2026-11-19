---
id: everything-claude-code__lead-intelligence
name: lead-intelligence
version: 1.0.0
description: >-
  AI-native lead intelligence and outreach pipeline. Replaces Apollo, Clay, and ZoomInfo with agent-powered signal scoring, mutual ranking, warm path discovery, source-derived voice modeling, and channel-specific outreach across email, LinkedIn, and X. Use when the user wants to find, qualify, and reach high-value contacts.
role: lead-intelligence
category: research
triggers:
  - lead intelligence
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - search.web
  - shell.exec
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/lead-intelligence/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: lead-intelligence
---

# lead-intelligence

## Role

Portable distillation of upstream skill `lead-intelligence` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

AI-native lead intelligence and outreach pipeline. Replaces Apollo, Clay, and ZoomInfo with agent-powered signal scoring, mutual ranking, warm path discovery, source-derived voice modeling, and channel-specific outreach across email, LinkedIn, and X. Use when the user wants to find, qualify, and reach high-value contacts.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
