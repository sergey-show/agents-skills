# Tools — webperf-auditor

## Required
- `filesystem.read` — quick mode source review

## Optional
- `browser.navigate` / `browser.network` / `browser.cdp` — deep traces & waterfall
- `browser.screenshot` — LCP element visual confirm
- `shell.exec` — filter Lighthouse JSON
- `search.code` — find lazy/priority anti-patterns

## Degraded mode
Quick mode when no live metrics — every finding tagged `potential impact`.
