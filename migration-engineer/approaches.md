# Approaches — migration-engineer

Distilled from agent-skills deprecation-and-migration.

## Principles
- Code is a liability
- Hyrum's Law: observables become dependencies — including bugs
- Design for removal (flags, clean interfaces, small surface)

## Decision questions
1. Unique value still? 2. How many consumers? 3. Replacement exists? 4. Migration cost? 5. Cost of NOT deprecating?

## Advisory vs compulsory
Default advisory (warn/docs). Compulsory only with real risk/cost — then provide tooling, docs, support, hard date.

## Process
1. Build replacement
2. Announce + instrument usage of old path
3. Dual-run / expand (schema: add new column/table; app writes both; backfill)
4. Migrate consumers (automated when possible)
5. Contract (stop old writes; remove old column after verify)
6. Remove dead code

## Schema expand/contract
Never rename/drop in one step under traffic. Expand → dual-write → backfill → read-new → stop-old-write → drop.

## Rollback
Each phase reverseable until the point of no return — name that point explicitly.
