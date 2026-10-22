# Change control templates

PCI DSS 6.5.1 requires every change ticket to include the five items below. For Adatree the change ticket is the ADA Jira ticket.

| Requirement | How we address it |
|---|---|
| A description of the change | **Description** section in the Jira ticket template, **Why** section in the PR template. |
| A security impact assessment | **Security impact** section in both templates. |
| Clear management approval to proceed | Omitted from the templates. The GitHub review approval on the linked PR is the approval, and branch protection requires it before merge. |
| Evidence that adequate testing has been carried out | Omitted from the templates. A required CI check must pass before a PR can merge. |
| An effective rollback plan | **Rollback** section in both templates. |

`.github/pull_request_template.md` is the default PR body for every Adatree repo that doesn't have its own template. A repo that adds its own `pull_request_template.md` stops getting this one, so keep these sections in any repo-specific template.

## Jira change ticket template

Copy this into the ADA ticket description:

```
## Description

<What changes and why. Frame it as a requirement: "We need X because Y.">

## Security impact

<What you checked and what you found: auth and permissions, consumer data or CDR tokens in logs or storage, new inputs, new outbound calls. "No security impact. Only changes X; touches no auth, consumer data or external input." is fine when true. A bare "None" is not an assessment.>

## Rollback plan

<Default: "Revert the PR and redeploy the previous version via adr-platform-deploy." If there is a Liquibase migration or a data change, say what a revert leaves behind and how to clean it up.>
```
