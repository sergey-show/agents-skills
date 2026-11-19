# Tools — design-auditor

## Required
- `filesystem.read` — source review

## Optional
- `browser.navigate` / `browser.screenshot` / `browser.snapshot` — live evidence
- `search.code` — token/drift scans
- `subagent.spawn` — isolate Assessment A from B
- `ask_user` — close with prioritized next-step question

## Degraded mode
Lead with `DEGRADED: single-context (<reason>)` when A/B cannot be isolated or browser evidence is unavailable.
