# Approaches — git-workflow

Distilled from agent-skills git-workflow-and-versioning.

## Trunk-based (recommended default)
Keep main deployable. Feature branches merge in 1–3 days. Dev branches are costs. Release branches OK for stabilize. Feature flags > weeks-long branches. Adapt if team uses gitflow — commit discipline matters more than topology.

## Commit early, often
Implement slice → test → verify → commit → next. Not: giant pile → one commit.

## Atomic commits
One logical thing per commit. Split mixed concerns (feature + drive-by refactor + deps).

## Messages
Explain **why**, not only what. Prefer conventional commits if repo uses them (`feat`/`fix`/`docs`/…). Body for motivation and user impact.

## Splitting a messy tree
1. status/diff inventory
2. group by logical change
3. stage selectively; commit each group
4. leave unrelated dirty files uncommitted or stash explicitly with user OK

## PRs
Small diffs; clear description; test plan checklist; link issues; note risks/rollout. Don't bundle unrelated features.

## Versioning
Semver: MAJOR break, MINOR compatible feature, PATCH fix. Changelog sections: Breaking / Features / Fixes. Tag releases from CI or documented process.

## Safety
No force-push to main/master unless user explicitly demands (and warn). No secrets in commits. Don't amend published commits without explicit request + rules.
