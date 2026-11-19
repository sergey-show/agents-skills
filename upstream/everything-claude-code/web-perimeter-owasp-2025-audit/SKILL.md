---
id: everything-claude-code__web-perimeter-owasp-2025-audit
name: web-perimeter-owasp-2025-audit
version: 1.0.0
description: >-
  Passive, non-destructive web perimeter security auditing mapped to OWASP Top 10:2025 surface leads, CDN Unkeyed Header Web Cache Poisoning (X-Forwarded-Host), supply chain manifest exposure, git object dumping prevention (/.git/HEAD), cryptographic headers, and AI crawler boundary governance (llms.txt, robots.txt). Use when auditing production domains, configuring Cloudflare/Vercel/Nginx edge security, or preparing pre-launch perimeter checks.
role: web-perimeter-owasp-2025-audit
category: security
triggers:
  - web perimeter owasp 2025 audit
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
  - shell.exec
  - test.run
sources:
  - research/everything-claude-code/skills/web-perimeter-owasp-2025-audit/SKILL.md
harness: any
upstream_repo: everything-claude-code
upstream_skill: web-perimeter-owasp-2025-audit
---

# web-perimeter-owasp-2025-audit

## Role

Portable distillation of upstream skill `web-perimeter-owasp-2025-audit` from `everything-claude-code`. Behavior is harness-agnostic; map capabilities in adapters.

## When to use

Passive, non-destructive web perimeter security auditing mapped to OWASP Top 10:2025 surface leads, CDN Unkeyed Header Web Cache Poisoning (X-Forwarded-Host), supply chain manifest exposure, git object dumping prevention (/.git/HEAD), cryptographic headers, and AI crawler boundary governance (llms.txt, robots.txt). Use when auditing production domains, configuring Cloudflare/Vercel/Nginx edge security, or preparing pre-launch perimeter checks.

## Workflow

Follow [approaches.md](approaches.md). Obey [rules.md](rules.md). Use only declared capabilities from [tools.md](tools.md).

## Done when

The upstream skill's success criteria are met with evidence (commands, diffs, or artifacts), not claims.

## See also

- [approaches.md](approaches.md)
- [rules.md](rules.md)
- [tools.md](tools.md)
- [source.md](source.md) — full agnosticized upstream body
