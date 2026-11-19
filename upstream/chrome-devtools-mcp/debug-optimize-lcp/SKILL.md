---
id: chrome-devtools-mcp__debug-optimize-lcp
name: debug-optimize-lcp
version: 1.0.0
description: >-
  Guides debugging and optimizing Largest Contentful Paint (LCP) using Chrome DevTools MCP tools. Use this skill whenever the user asks about LCP performance, slow page loads, Core Web Vitals optimization, or wants to understand why their page's main content takes too long to appear. Also use when the user mentions "largest contentful paint", "page load speed", "CWV", or wants to improve how fast their hero image or main content renders.
role: debug-optimize-lcp
category: engineering
triggers:
  - debug optimize lcp
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - browser.navigate
  - browser.snapshot
  - test.run
sources:
  - research/chrome-devtools-mcp/skills/debug-optimize-lcp/SKILL.md
harness: any
upstream_repo: chrome-devtools-mcp
upstream_skill: debug-optimize-lcp
---

# debug-optimize-lcp

## Role

Portable distillation of upstream skill `debug-optimize-lcp` from `chrome-devtools-mcp`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Guides debugging and optimizing Largest Contentful Paint (LCP) using Chrome DevTools MCP tools. Use this skill whenever the user asks about LCP performance, slow page loads, Core Web Vitals optimization, or wants to understand why their page's main content takes too long to appear. Also use when the user mentions "largest contentful paint", "page load speed", "CWV", or wants to improve how fast their hero image or main content renders.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
