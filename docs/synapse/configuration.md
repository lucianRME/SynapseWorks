# Synapse Configuration

## Purpose
Define runtime options and user preferences that shape Synapse behaviour.

## Who it is for
- Jira administrators
- Team leads defining delivery conventions
- Users tuning personal panel behaviour

## Prerequisites
- Synapse installed in Jira
- Access to the panel in a Jira issue

## Steps
1. Decide whether to enable auto-generate-on-open for your workflow.
2. Store auto-generate preference in browser `localStorage` on each user device.
3. During refine, configure output style:
   - Toggle grouping
   - Toggle BDD style
   - Edit titles and BDD text
   - Reset individual items when required
4. Use dry-run as a default guardrail before create-subtasks mode.
5. In development contexts, use diagnostics (self-test, payload debug, DEV badge) for targeted checks.

## Configuration reference
- Auto-generate-on-open: user-level browser setting (`localStorage`)
- Refine controls: per-session editing and toggles in panel UI
- Dry-run mode: validates creation path without writing subtasks
- Create-subtasks mode: writes linked subtasks to Jira issue

## Common issues
- Preference appears lost across browsers: `localStorage` is browser-specific.
- Users expect dry-run to create issues: dry-run does not write to Jira.
- Diagnostics visible in development only: expected behaviour.

## Related pages
- [Overview](overview.md)
- [Workflow](workflow.md)
- [Security and data](security-data.md)
