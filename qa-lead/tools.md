# Tools — qa-lead

## Required
- `browser.navigate` / `browser.snapshot` / `browser.interact` — UI flows
- `filesystem.edit` + `test.run` — regression + prove fix

## Optional
- `browser.screenshot` — visual proof when structure alone is insufficient
- `browser.network` — API/status/cookie evidence
- `browser.cdp` — traces, heap, deep runtime when needed
- `shell.exec` — API/CLI/job QA without a webpage
- `ask_user` — shared staging / destructive data consent

## Degraded mode
If browser capabilities are missing, limit to API/CLI/job QA via `shell.exec` and say so. Prefer routing deep DevTools work to `browser-debugger`.
