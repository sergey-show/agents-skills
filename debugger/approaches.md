# Approaches — debugger

Distilled from Superpowers systematic-debugging and agent-skills debugging-and-error-recovery.

## Iron law
```
NO FIXES WITHOUT ROOT CAUSE INVESTIGATION FIRST
```
If Phase 1 incomplete, do not propose fixes.

## Stop-the-line
1. STOP adding features/changes
2. PRESERVE evidence
3. DIAGNOSE via triage
4. FIX root cause
5. GUARD recurrence (regression test/monitor)
6. RESUME only after verification

## Phase 1 — Root cause investigation
1. Read error messages/stack traces completely (lines, codes, paths).
2. Reproduce consistently; if not → gather data, don't guess.
3. Check recent changes (diff, deps, config, env).
4. Multi-component systems: add diagnostic instrumentation at **each boundary** (in/out/env/state); run once to see WHERE it breaks; then zoom in.
5. Deep stack: trace bad value backward to origin; fix at source.

## Phase 2 — Pattern analysis
Find working examples; read reference implementations completely; list every difference; understand dependencies/assumptions.

## Phase 3 — Hypothesis and testing
One hypothesis: "X is root cause because Y." Smallest change to test one variable. Worked → Phase 4. Didn't → new hypothesis, don't stack fixes. Say when you don't know.

## Phase 4 — Implementation
1. Create failing test/repro (TDD) before fixing.
2. Single fix for root cause — no drive-by refactors.
3. Verify: test passes; suite not broken; original symptom gone.
4. <3 failed fixes: return to Phase 1 with new info. ≥3: STOP — question architecture with human (shared state/coupling; pattern unsound?).

## Triage checklist (agent-skills)
Reproduce → Localize layer (UI/API/DB/build/external/test) → Isolate (bisect, binary search, disable halves) → Identify cause → Minimal fix → Verify → Guard.

Non-reproducible: timing (logs/delays/load), environment (versions/env/data/CI), state (leaks/globals), else defensive logging + alert signature.

## Red flags → return to Phase 1
Quick fix now investigate later; try changing X; multiple changes at once; skip test; "probably X"; don't understand but might work; "one more fix" after 2+.

## When "no root cause"
Document investigation; implement handling (retry/timeout/message); add monitoring. 95% of "no root cause" is incomplete investigation.
