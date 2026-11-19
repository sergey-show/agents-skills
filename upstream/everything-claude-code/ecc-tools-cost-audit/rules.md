# Rules (extracted)

- do not mutate unrelated billing, checkout, or UI flows while tracing analysis burn
- do not begin with broad repo wandering; settle webhook -> queue -> worker first
- do not mix customer billing inference with code-backed product truth
- do not fix lower-value quality issues before the highest-burn path is contained
- do not claim burn is fixed until the narrow proving step was rerun
- do not push or deploy unless the user asked
- do not touch unrelated repo-local changes if they are already in progress
