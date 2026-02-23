# Synapse Overview

## Purpose
Explain what the Synapse Jira issue panel does and where it fits in delivery workflows.

## Who it is for
- Delivery teams turning Jira issue context into actionable subtasks
- Jira administrators enabling structured execution at scale
- Governance leads who need repeatable requirement quality

## Prerequisites
- Synapse installed on the Jira Cloud site
- Access to Jira issues where the panel is available
- Permission to create subtasks if using create-subtasks mode

## Steps
1. Open a Jira issue and load the embedded Synapse issue panel.
2. Generate a requirements preview using issue context.
3. Review grouped output and executable BDD-style scenarios.
4. Optionally refine titles and BDD content before creation.
5. Run dry-run validation, then create subtasks when ready.

## Capability summary
- Embedded `jira:issuePanel` experience inside Jira issues
- Requirement preview with executable BDD-style scenarios
- Uses Jira context: summary, description (ADF and text), comments, labels, issue type, and project info
- Grouped preview output with UI grouping controls
- `Refine with Synapse` editor for title and BDD editing, reset item, grouping toggle, BDD style toggle
- Guidance shown if refine is opened before generating a preview
- Dry-run mode shows what would be created without creating subtasks
- Create-subtasks mode creates subtasks linked to the current issue and returns created keys or errors
- Auto-generate-on-open preference stored in browser `localStorage`
- Dev-only diagnostics (self-test, payload debug, DEV badge)

## Rovo positioning
Synapse complements Atlassian AI/Rovo by enforcing consistent execution structure (subtasks and validation), not only providing AI suggestions.

## Common issues
- Panel not visible: verify app installation and issue panel availability.
- Creation unavailable: check Jira permissions for creating subtasks.
- Refine opened too early: generate a preview first.

## Related pages
- [Quickstart](quickstart.md)
- [Workflow](workflow.md)
- [Configuration](configuration.md)
- [Security and data](security-data.md)
- [Troubleshooting](troubleshooting.md)
- [Documentation index](../index.md)
