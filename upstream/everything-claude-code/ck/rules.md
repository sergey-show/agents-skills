# Rules (extracted)

- Always expand `~` as `$HOME` in Bash calls.
- Never edit `context.json` or `CONTEXT.md` directly — always use the scripts.
- Commands are case-insensitive: `/CK:SAVE`, `/ck:save`, `/Ck:Save` all work.
- If a script exits with code 1, display its stdout as an error message.
- If `projects.json` is malformed, tell the user and offer to reset it to `{}`.
