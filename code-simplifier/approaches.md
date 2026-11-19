# Approaches — code-simplifier

Distilled from agent-skills code-simplification and ponytail lean rules.

## Preconditions
Know current behavior. Prefer existing tests; add characterization tests before risky deletes.

## Operators (in order)
1. **Delete** — dead code, unused options/flags, speculative features, commented-out blocks
2. **Reuse** — repo already has the helper (name the path); remove the duplicate
3. **Stdlib / native / installed dep** — don't hand-roll or add deps for a few lines
4. **YAGNI** — interface with one impl; factory with one product; pass-through wrappers; config nobody sets
5. **Merge** — near-copies that must change together
6. **Split** — one function doing unrelated jobs (by job, never by line count; never extract helpers only to shorten)

## Behavior lock
Simplification is not a sneaky feature change. If behavior must change, say so and get OK.

## Review output
List deletions/merges with blast radius; note anything skipped (unclear callers, missing tests).
