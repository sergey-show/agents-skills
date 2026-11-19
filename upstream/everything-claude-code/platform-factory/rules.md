# Rules (extracted)

1. **Freeze before build.** Any change to a dependency manifest makes `.platform-factory/freeze.lock.json` stale. Run `pf project freeze`, then `pf build`.
2. **Treat `pf verify` as the gate.** A build is not done until `verify` passes.
3. **Inspect plugins before directory detection.** Native executable classification does not run the target, but directory detection invokes loaded language plugins. Review those plugins and project commands as executable configuration before `detect`, `plan`, `freeze`, or `build`.
4. **Ambiguity is an error.** `pf detect` exits with code 2 when a directory matches several ecosystems. Pass `--accept-ambiguous` only when the user confirmed the choice.
5. **Never add secrets to build inputs.** Inputs end up in the image and its evidence.
6. **Callbacks are opt-in.** `pf` hooks (CLI/MCP callbacks) only run when `PLATFORM_FACTORY_HOOKS_CONFIG` points to an explicit absolute file, so a cloned repository cannot activate executables.
7. **Keep execution within the user's authorization.** Before publishing, deploying, launching, or running a workload, identify its target, image reference, and effects. Reuse explicit authorization already given for that scope; ask only when the action exceeds it. Use `--dry-run` where available before the authorized mutation. Do not add `--yes` to bypass an approval the user has not given.
