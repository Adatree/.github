## Description

<What changes and why. Frame it as a requirement: "We need X because Y.">

## Security impact

<What you checked and what you found: auth and permissions, consumer data or CDR tokens in logs or storage, new inputs, new outbound calls. "No security impact. Only changes X; touches no auth, consumer data or external input." is fine when true. A bare "None" is not an assessment.>

## Approval

The GitHub approval on the linked PR(s): <PR link(s)>

## Testing evidence

<What ran and the result, e.g. "`./gradlew test` passes, CI green on <PR>, verified in dev by <check>." "Covered by tests" with nothing named is not evidence.>

## Rollback plan

<Default: "Revert the PR and redeploy the previous version via adr-platform-deploy." If there is a Liquibase migration or a data change, say what a revert leaves behind and how to clean it up.>
