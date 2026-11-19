# Approaches — config

> Ported from `research/TokenEconomizer/plugin/codex-skills/config/SKILL.md`. Host-specific wiring stripped or generalized.

# TokenEconomizer: config

Run this command in the repository's root directory:

```
"${TOKENECONOMIZER_HOME:-$HOME/.tokeneconomizer}/bin/te" --host codex --cwd "$(pwd)" config ARGS
```

Use `show` as ARGS unless the user asked to change a setting; then `set KEY=VALUE ...` or `unset KEY ...`, adding `--global` only if they asked for every repository. Show the output verbatim in a code block; if a setting was rejected, say why in one sentence.

Changing a setting (`set`, `unset`) writes TokenEconomizer's own state under `~/.tokeneconomizer`, outside the workspace, which the sandbox keeps read-only: run that command with `sandbox_permissions` set to `"require_escalated"` and a one-line `justification`, so that Codex asks the user to approve it. `show` reads only and needs no approval.

The command reads and writes only TokenEconomizer's own state (under `~/.tokeneconomizer`); it
makes no model call. If it reports that the launcher does not exist, the plugin has not run in a session yet:
ask the user to start a new Codex session in this repository first.

