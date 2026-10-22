## Why

<!-- Jira ticket (e.g. ADA-1234) and, if this is one PR of several, which step it is.
Then 1-3 sentences on motivation or scope. Don't recap the diff.
The ticket must carry the same items (description, security impact, approval, testing, rollback);
approving this PR is the ticket's approval. -->

## Security Impact

<!-- Required. Say what you checked and what you found: auth and permissions,
consumer data or CDR tokens in logs or storage, new inputs, new outbound calls.
"No security impact. Only changes X; touches no auth, consumer data or external input." is fine when true.
A bare "None" is not an assessment. -->

## Rollback

<!-- Required. Default: "Revert this PR and redeploy the previous version via adr-platform-deploy."
If the PR has a Liquibase migration or changes data, say what a revert leaves behind and how to clean it up. -->

## Testing

<!-- Required. Evidence, not a claim. Name what ran and the result,
e.g. "`./gradlew test` passes locally; CI green." or a short checklist of manual checks and outcomes. -->
