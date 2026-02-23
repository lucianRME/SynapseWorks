# Synapse Workflow

## Purpose
Describe the operating workflow for generating, refining, validating, and creating execution artefacts.

## Who it is for
- Delivery teams standardising breakdown quality
- Process owners building repeatable issue handling patterns

## Prerequisites
- Synapse panel access on a Jira issue
- Issue context available (summary, description, comments, labels, issue type, project data)

## Steps
1. Generate preview from current issue context.
2. Review grouped output and executable BDD-style scenarios.
3. Refine content using `Refine with Synapse`:
   - Edit titles and BDD steps
   - Toggle grouping and BDD style
   - Reset individual items when needed
4. Validate path using dry-run mode.
5. Create subtasks from approved output.
6. Review creation status, including created keys and any per-item errors.

## Operational notes
- If refine is opened before preview generation, guidance is shown to direct the user to generate first.
- Friendly status mapping helps users interpret creation outcomes.
- Dev-only diagnostics are available for controlled troubleshooting in development contexts.

## Rovo positioning
Where Rovo assists with AI suggestions, Synapse adds operational control by applying consistent structure and validation before execution in Jira.

## Common issues
- Users skip dry-run and hit avoidable errors in create mode.
- Incomplete issue context can reduce preview quality.
- Mixed editing styles can reduce consistency across teams; align on BDD style toggles.

## Related pages
- [Overview](overview.md)
- [Quickstart](quickstart.md)
- [Configuration](configuration.md)
