# Approaches — ci-cd-engineer

Distilled from agent-skills ci-cd-and-automation. Examples are illustrative — adapt to GitHub/GitLab/etc. without baking one host into rules.

## Quality gate pipeline (typical)
PR → lint → typecheck → unit tests → build → integration → optional e2e → security audit → bundle budget → ready for review.
**No gate skipped.** Fix the failure; don't disable the rule or skip the test to go green.

## Shift left / faster is safer
Catch issues earliest cheapest. Small batches + frequent deploys reduce risk.

## Pipeline as code
Version workflows with the repo. Pin action/versions responsibly. Cache deps. Parallelize independent jobs. Keep secrets in the secret store — never in YAML.

## Deploy strategies
Choose consciously: rolling, blue/green, canary, or manual approve for prod. Document rollback. Prefer same artifact promoted across envs.

## Debugging CI
Reproduce locally with the same commands. Read logs fully. Flakes: quarantine with ticket, don't ignore. Clock/time, order dependence, shared state are usual villains.

## Alignment with CONSTRAINTS
If `CONSTRAINTS.md` / process-engineer constraints exist, CI must enforce those numbers — not a weaker bar.
