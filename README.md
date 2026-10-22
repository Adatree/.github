# Change control templates (draft)

PCI DSS 6.5.1: every change ticket must carry a description, a security impact assessment, approval to proceed, testing evidence and a rollback plan. A change missing any of them is rejected until it's filled in.

For Adatree the change ticket is the ADA Jira ticket. Approval is the GitHub approval on the linked PR.

- `jira-change-ticket-template.md`: the five sections for the ADA ticket description. This is the record auditors sample.
- `.github/pull_request_template.md`: committed to each repo. Mirrors the ticket so reviewers see the same items, and the PR approval is the ticket's approval.
