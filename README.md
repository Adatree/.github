# Change control templates

PCI DSS 6.5.1 requires every change ticket to include the five items below. For Adatree the change ticket is the ADA Jira ticket.

| Requirement | How we address it |
|---|---|
| A description of the change | **Why** section in the PR template. |
| A security impact assessment | **Security Impact** section in the PR template. |
| Clear management approval to proceed | Omitted from the template. The GitHub review approval on the linked PR is the approval, and branch protection requires it before merge. |
| Evidence that adequate testing has been carried out | Omitted from the template. A required CI check must pass before a PR can merge. |
| An effective rollback plan | **Rollback** section in the PR template. |

`.github/pull_request_template.md` is the default PR body for every Adatree repo that doesn't have its own template. A repo that adds its own `pull_request_template.md` stops getting this one, so keep these sections in any repo-specific template.
