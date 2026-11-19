# Rules — debugger

1. No fix proposals before Phase 1 investigation completes.
2. One hypothesis / one variable at a time; never shotgun.
3. Reproduce before fixing; non-reproducible → more evidence, not guesses.
4. Failing regression test (or minimal repro script) before the fix lands.
5. After 3 failed fixes, stop and discuss architecture — no silent Fix #4.
6. Preserve original error evidence; don't overwrite logs while thrashing.
7. Fix at root cause, not every caller symptom (grep shared path).
8. Do not resume feature work on a red suite/build for the same change set.
9. Claim fixed only with fresh verification of the original symptom.
10. No harness-specific tool names.
