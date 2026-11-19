# Approaches — tdd-engineer

Distilled from Superpowers TDD, agent-skills TDD, Matt Pocock tdd skill (portable parts).

## Iron law
```
NO PRODUCTION CODE WITHOUT A FAILING TEST FIRST
```
Wrote code first? Delete it. Start over. No keep-as-reference / adapt-while-testing.

## Discover the stack first
Before first test: language/build files; checked-in wrappers; framework + how to run one test vs suite; neighboring test layout; README/CI commands. Never assume `npm test`.

## Cycle
RED → verify fail correctly → GREEN minimal → verify pass (focused + suite discipline) → REFACTOR stay green → next.

### RED
One behavior; clear name; real code (mocks only if unavoidable). Name the production change that would make the test fail — before writing it.

### Verify RED (mandatory)
Fails (not errors) for expected reason (feature missing, not typo). Passes immediately → testing existing behavior — fix test. Errors → fix harness until clean fail.

### GREEN
Simplest code to pass. No extra features, no drive-by refactors, no YAGNI options.

### Verify GREEN
Focused pass; then project's suite command before calling the change done. Any failure the suite shows goes in the report by name — omission falsifies the report. Fix code not tests when the new test fails; fix broken others now.

### REFACTOR
Only on green: names, duplication, helpers. No new behavior.

## Good tests
| Quality | Good | Bad |
|---------|------|-----|
| Minimal | One thing; "and" in name → split | validates A and B and C |
| Clear | Behavior in name | test1 |
| Intent | Shows desired API | Obscures |

Assert real behavior, never mock behavior. Keep test-only helpers out of production.

## Bug fix = prove-it
Failing test reproducing bug → red → fix → green. Never fix without a test.

## Rationalizations (all mean: delete & restart)
Too simple; test after; spirit not ritual; already manually tested; deleting hours is wasteful; keep as reference; need to explore first (OK explore then throw away); TDD slows me down; existing code has no tests (still add for your change).

## When stuck
Hard to test → simplify design/API. Must mock everything → too coupled. Huge setup → extract helpers or simplify.
