# Tools — careful-ops

## Required
- `ask_user` — confirm mode, freeze path, destructive overrides

## Optional
- `shell.exec` / `git.ops` / `filesystem.edit` — the operations being guarded
- `memory.persist` — remember freeze boundary across turns when available

## Adapter note
Hosts may implement real PreToolUse hooks; this skill states the behavioral contract either way. Never rely on hooks alone in the DoT core — announce and self-enforce.
