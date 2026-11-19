# Approaches — verification-loop

Distilled from ECC verification-loop + Superpowers verification-before-completion.

## Iron law
```
NO COMPLETION CLAIMS WITHOUT FRESH VERIFICATION EVIDENCE
```
If you haven't run the proving command in this turn, you cannot claim it passes.

## Gate function
1. IDENTIFY proving command
2. RUN full/fresh
3. READ exit code + failures
4. VERIFY output confirms claim
5. ONLY THEN claim — with evidence

## Phases (adapt to repo)
1. **Build** — fail → stop and fix
2. **Typecheck** — report errors; fix critical before continue
3. **Lint** — consume full stream; limit display if needed without breaking pipefail
4. **Tests** — counts passed/failed; coverage if project tracks it
5. **Security hygiene** — secret patterns, obvious debug leftovers per project norms
6. **Diff review** — unintended changes, missing error handling, edge cases

## Acceptance
Local PASS ≠ production acceptance. Report target-env verification separately when deploy matters.

## Red flags
"should/probably/seems"; celebrating before running; trusting subagent "success"; partial checks; synonym games to dodge the rule.

## Regression tests
For bug fixes: prove red (revert or pre-fix fail) then green — not only a passing test after the fact.
