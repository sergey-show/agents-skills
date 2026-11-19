# Tools — security-officer

## Required
- `filesystem.read` / `search.code` — static assessment

## Optional
- `security.scan` — contained scanners when available
- `shell.exec` — project-approved local checks inside sandbox policy
- `browser.navigate` — staging-only runtime checks when authorized
- `subagent.spawn` — hunter/verifier isolation (finder ≠ verifier)
- `ask_user` — confirm production boundaries and audit mode

## Safety
Default to static analysis. Runtime only on explicitly authorized non-prod targets inside OS-enforced sandbox constraints. No exploit payloads in output.
