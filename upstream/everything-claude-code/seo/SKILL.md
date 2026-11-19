---
id: everything-claude-code__seo
name: seo
version: 1.0.0
description: >-
  Audit, plan, and implement SEO improvements across technical SEO, on-page optimization, structured data, Core Web Vitals, and content strategy. Use when the user wants better search visibility, SEO remediation, schema markup, sitemap/robots work, or keyword mapping.
role: seo
category: research
triggers:
  - seo
capabilities_required:
  - filesystem.edit
  - filesystem.read
  - search.code
capabilities_optional:
  - search.web
sources:
  - research/everything-claude-code/skills/seo/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: seo
---

# seo

## Role

Portable distillation of upstream skill `seo` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Audit, plan, and implement SEO improvements across technical SEO, on-page optimization, structured data, Core Web Vitals, and content strategy. Use when the user wants better search visibility, SEO remediation, schema markup, sitemap/robots work, or keyword mapping.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
