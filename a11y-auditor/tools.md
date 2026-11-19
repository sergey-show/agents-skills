# Tools — a11y-auditor

## Required
- `filesystem.read`

## Optional
- `browser.snapshot` / `browser.interact` / `browser.navigate` — tree + keyboard
- `browser.screenshot` — visual order vs DOM order
- `browser.cdp` — evaluate snippets for contrast/tap targets
- `search.code` — anti-pattern grep
- `shell.exec` — filter axe/Lighthouse JSON

## Degraded mode
Quick source scan; label as incomplete without runtime tree evidence.
