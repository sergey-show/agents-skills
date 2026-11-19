# Approaches — repos

> Ported from `research/TokenEconomizer/plugin/codex-skills/repos/SKILL.md`. Host-specific wiring stripped or generalized.

# TokenEconomizer: repos

Run this command in the repository's root directory:

```
"${TOKENECONOMIZER_HOME:-$HOME/.tokeneconomizer}/bin/te" --host codex --cwd "$(pwd)" repos ARGS
```

Use `list` as ARGS unless the user asked to `migrate`, or to `merge KEY [INTO]` (keys as the list shows them; INTO defaults to this repository). Never run `migrate` or `merge` unless the user asked for it. Show the output verbatim in a code block.

`migrate` and `merge` move state between repositories; that writes TokenEconomizer's own state under `~/.tokeneconomizer`, outside the workspace, which the sandbox keeps read-only: run that command with `sandbox_permissions` set to `"require_escalated"` and a one-line `justification`, so that Codex asks the user to approve it. `list` reads only and needs no approval.

The command reads and writes only TokenEconomizer's own state (under `~/.tokeneconomizer`);
it makes no model call, and a merge keeps the old state directory under
`~/.tokeneconomizer/merged/`. If it reports that the launcher does not exist, the plugin has
not run in a session yet: ask the user to start a new Codex session in this repository first.

