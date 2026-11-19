# Approaches — observability-engineer

Distilled from agent-skills observability-and-instrumentation.

## Define questions first
Example: payment retry → success vs retry fraction; permanent failure reasons; provider latency. Every signal answers one question. Can't name questions → not ready to instrument.

## Signal choice
| Signal | Answers | Notes |
|--------|---------|-------|
| Structured log | What happened in this case | Per-event cost |
| Metric | How often/how fast | Cheap aggregate |
| Trace | Where time went | Sampled cross-service |

## Structured logging
Stable `event` name + fields; not string interpolation. Levels: error (act), warn (degraded/handled), info (business), debug (off by default in prod). **Correlation IDs mandatory** across logs/spans/outbound calls.

## Cardinality
Avoid unbounded label values (user ids, URLs with ids) on metrics. High cardinality → cost + broken dashboards.

## Alerting
Alert on symptoms users feel (error rate, latency SLO burn). Each alert needs a runbook link. Page sparingly; ticket the rest.

## Privacy
No secrets/PII in logs (tokens, raw cards, passwords). Redact at the edge.

## Not this skill
Active debugging now → `debugger`. Measured slowness optimization → `performance-engineer`.
