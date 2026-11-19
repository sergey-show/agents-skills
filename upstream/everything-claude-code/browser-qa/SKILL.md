---
id: everything-claude-code__browser-qa
name: browser-qa
version: 1.0.0
description: >-
  Run automated post-deploy UI verification with a browser automation MCP (claude-in-chrome, Playwright, or Puppeteer): console-error and Core Web Vitals smoke checks, form and auth-flow interaction tests, screenshot visual regression across three breakpoints, and axe-core accessibility audits ending in a SHIP / DO-NOT-SHIP verdict. Use when testing a deployed feature on staging or preview, before shipping frontend changes, reviewing a frontend PR, or checking responsive layout and accessibility.
role: browser-qa
category: design
triggers:
  - browser qa
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - git.ops
  - test.run
sources:
  - research/everything-claude-code/skills/browser-qa/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: browser-qa
---

# browser-qa

## Role

Portable distillation of upstream skill `browser-qa` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Run automated post-deploy UI verification with a browser automation MCP (claude-in-chrome, Playwright, or Puppeteer): console-error and Core Web Vitals smoke checks, form and auth-flow interaction tests, screenshot visual regression across three breakpoints, and axe-core accessibility audits ending in a SHIP / DO-NOT-SHIP verdict. Use when testing a deployed feature on staging or preview, before shipping frontend changes, reviewing a frontend PR, or checking responsive layout and accessibility.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
