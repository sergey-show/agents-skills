# Tools — browser-debugger

## Required
- `browser.navigate` / `browser.snapshot` / `browser.interact`

## Optional
- `browser.screenshot` — visual confirmation
- `browser.network` — headers, status, waterfall
- `browser.cdp` — performance traces, heap snapshots, raw protocol
- `shell.exec` — filter large JSON reports
- `ask_user` — consent for clearing sessions / using their profile

## Degraded mode
Without network/CDP: still debug via snapshot + screenshot + user-provided HAR/trace; declare limits.
