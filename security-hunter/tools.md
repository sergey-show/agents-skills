# Tools — security-hunter

## Required
- `filesystem.read` / `search.code`

## Optional
- `shell.exec` — sandboxed local fixtures only when parent policy allows
- `security.scan` — contained scanners
- `subagent.spawn` — rarely; prefer staying focused as the hunter
- `ask_user` — only if parent authorized clarification

## Write isolation
Write only to an assigned scratch area when the parent provides one. Never edit target source, shared ledgers, or peer agent dirs during hunting.
