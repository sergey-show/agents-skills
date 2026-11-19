---
id: a11y-engineer
name: A11y Engineer
version: 1.0.0
description: >-
  Audits and remediates accessibility to WCAG 2.2 AA: automated checks,
  keyboard, screen reader, contrast. Use before shipping UI or when a11y
  issues are reported.
role: Accessibility Engineer
category: engineering
triggers:
  - accessibility
  - a11y
  - WCAG
  - axe
  - keyboard navigation
  - screen reader
  - contrast
capabilities_required:
  - browser.navigate
  - browser.snapshot
capabilities_optional:
  - browser.interact
  - browser.screenshot
  - shell.exec
  - filesystem.edit
  - ask_user
sources:
  - research/agent-skills/skills/accessibility-engineering
  - research/chrome-devtools-mcp/skills/a11y-debugging
harness: any
---

# A11y Engineer

## Role
Accessibility is engineering quality and often a legal requirement. Audit existing UI, triage real violations, remediate to WCAG 2.2 AA. Construction patterns live in `frontend-engineer`; this skill audits and fixes.

## When to use
Pre-ship UI audit; reported SR/keyboard issues; axe/pa11y triage; remediating verified violations.

## Workflow
1. Automated audit → group by severity → verify each in browser.
2. Manual: keyboard, screen reader, visual (contrast/zoom/motion/focus).
3. Fix in priority order; re-audit.
4. Report residual risk for anything untested.

## Done when
Critical/serious verified issues fixed or explicitly deferred with owner; keyboard path works; re-audit clean or documented.

## See also
- Related: `frontend-engineer`, `qa-lead`

## Upstream depth

- `skills/upstream/agent-skills/accessibility-engineering/`
- `skills/upstream/chrome-devtools-mcp/a11y-debugging/`
