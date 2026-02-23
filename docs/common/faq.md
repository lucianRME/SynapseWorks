# FAQ

## Purpose
Answer common cross-product questions for Synapse, Decision Register, and the Synapse platform pages.

## Who it is for
- Jira administrators
- Product owners and delivery managers
- Security and compliance reviewers

## Prerequisites
- Access to this documentation set
- Access to your Jira site for product checks

## Steps
1. Check product scope first: Synapse and Decision Register are Marketplace apps, while `docs/saas/*` describes the Synapse platform track.
2. Match your question to setup, workflow, export, or security/data topics.
3. If unresolved, follow the support process in [Support](support.md).

## FAQ
### Does Synapse replace Atlassian AI or Rovo?
No. Synapse complements Atlassian AI/Rovo by enforcing consistent execution structure through subtasks and validation, instead of only providing suggestions.

### Which app is read-only in Jira?
Decision Register is read-only against Jira issue data and change history.

### Which app can create Jira artefacts?
Synapse can create subtasks from generated requirement previews.

### Where are user preferences stored?
- Decision Register: per-user preferences in Forge storage (`storage:app`).
- Synapse: auto-generate-on-open preference in browser `localStorage`.

### Are Jira credentials stored by SynapseWorks apps?
No. Jira credentials are not stored.

## Common issues
- "Feature mismatch": verify whether you are reading app docs (`docs/synapse/*`, `docs/decision-register/*`) or platform docs (`docs/saas/*`).
- "Permission errors": confirm Jira project permissions and app installation state.

## Related pages
- [Documentation index](../index.md)
- [Support](support.md)
- [Synapse security and data](../synapse/security-data.md)
- [Decision Register security and data](../decision-register/security-data.md)
- [Platform security and data](../saas/security-data.md)
