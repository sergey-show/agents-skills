# Rules — ci-cd-engineer

1. Do not weaken gates (skip tests, disable lint) to make CI green.
2. Never commit secrets into workflow files.
3. Document local equivalents of CI commands.
4. Pin or hash third-party actions per org security policy.
5. Prod deploys need explicit strategy + rollback notes.
6. Flaky tests get fixed or quarantined with ownership — not silent retries forever.
7. No harness-specific tool names.
