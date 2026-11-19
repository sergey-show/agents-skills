# Approaches — design-builder

## Build loop (Hallmark + Taste portable)

```
preflight → ask/direction → picks → hero build → hero check →
page build → sweep/gate rounds → finish review → material ask
```

### Hero first
Write nav + hero only. Verify at 1280×800: headline, one sentence, primary action, focal visual. Only then build below-the-fold sections (one idea each, mass over word count).

### Page invariants
One primary button style, one container width, one column gap below hero, one radius per nesting level; prefer left-aligned heads over centered stacks.

### Tokens first
Every colour and font through tokens. Append-only integration with existing stylesheets when in a real project.

### Imagery honesty
Real captures > library photos > slots. Never drawn fake product when the product runs. Credit library photos. No invented metrics.

## Finish gate (Taste portable concepts)

See [references/finish-gate.md](references/finish-gate.md).

- Arm with start target, kind, category, primary action, round budget (default ~3).
- Each changing run is a round: FAIL → fix → re-run.
- WARNs don't block except house rules elevated to FAIL (e.g. missing hero entrance / missing moment when the system requires them).
- Waivers need check id + target + reason; too many waivers is itself a FAIL.
- Rounds exhausted → OPEN: stop polishing, list remaining FAILs, ship with honesty.
- Only the user can DONE early with their words.

## Craft sweep checklist

Floor → Reflex → Finish (design-director gates). Consistency at 1440 and 390. Basics: names, alt, labels, heading order, Tab walk, lang, head tags. Empty-area: sections >50% empty fail.

## Anti-gaming
Do not detect headless checkers to hide defects. Do not strip aria-hidden en masse to fake a11y. Kit/vendor files should stay unmodified unless intentionally forked.

## Hand-off
Direction fights → `design-director`. System locking → `design-system`. Critique-only → `design-auditor`.
