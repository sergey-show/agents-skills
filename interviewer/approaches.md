# Approaches — interviewer

Distilled from agent-skills interview-me and Matt Pocock grilling/grill-me.

## Mode A — Interview-me (default for fuzzy product/feature asks)

### Step 1: Hypothesis + confidence
One sentence + 0–100% confidence. Below ~70% note what's missing.

### Step 2: One question at a time with GUESS
```
Q: ...
GUESS: ... (reasoning)
```
Wait for reaction. Batches encourage skim and lock wrong framing. Guesses surface your assumptions; be willing to be wrong.

### Step 3: Want vs should-want
Watch for best-practice karaoke, convention deferral, "I should probably…", buzzwords-as-goals. Ask: *If you didn't have to justify this to anyone, what would you actually want?*

### Step 4: Restate intent
5–8 lines in their language; line-by-line confirmable.

### Stop ~95%
You can predict their answers to the next three questions. If not, confidence is fake — keep going. Don't interview mechanical/unambiguous tasks or when user demanded speed over verification. Non-interactive contexts: flag blocker instead of guessing.

## Mode B — Grilling design tree
Map decisions as a tree. **Frontier** = decisions whose prerequisites are settled. Each round: ask whole frontier, numbered, each with recommended answer (worded so "yes" accepts recommendation). Wait for answers; recompute frontier. Facts are the agent's job (spawn fresh fact-finders); decisions are the user's. Done when frontier empty — do not act until user confirms shared understanding.

## Handoff
Confirmed intent → `spec-author` (to-spec) or `product-ceo` (wedge) or `process-engineer` (design gate).
