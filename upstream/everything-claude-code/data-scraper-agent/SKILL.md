---
id: everything-claude-code__data-scraper-agent
name: data-scraper-agent
version: 1.0.0
description: >-
  Build a fully automated AI-powered data collection agent for any public source — job boards, prices, news, GitHub, sports, anything. Runs on a schedule, enriches data with a free LLM (Gemini Flash), stores results in Notion/Sheets/Supabase, and learns from user feedback. Runs 100% free on GitHub Actions. Use when the user wants to monitor, collect, or track any public data automatically.
role: data-scraper-agent
category: engineering
triggers:
  - data scraper agent
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - ask_user
  - browser.navigate
  - browser.snapshot
  - git.ops
  - search.web
  - subagent.spawn
  - test.run
sources:
  - research/everything-claude-code/skills/data-scraper-agent/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: data-scraper-agent
---

# data-scraper-agent

## Role

Portable distillation of upstream skill `data-scraper-agent` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Build a fully automated AI-powered data collection agent for any public source — job boards, prices, news, GitHub, sports, anything. Runs on a schedule, enriches data with a free LLM (Gemini Flash), stores results in Notion/Sheets/Supabase, and learns from user feedback. Runs 100% free on GitHub Actions. Use when the user wants to monitor, collect, or track any public data automatically.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
