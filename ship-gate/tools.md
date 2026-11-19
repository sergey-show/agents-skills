# Tools — ship-gate

## Required
- `filesystem.read` / `git.ops` / `test.run` — know the change and its checks

## Optional
- `subagent.spawn` — parallel specialist fan-out (preferred)
- `search.code` — risk hotspot scan
- `browser.navigate` — smoke evidence
- `ask_user` — accept residual risk
- `shell.exec` — CI status scripts

## Degraded mode
Without subagents: run lenses sequentially in-main; still merge with the same decision template.
