# SynapseWorks Documentation

This repository contains GitBook-ready Markdown documentation for SynapseWorks Atlassian Marketplace apps.
Synapse runs fully on Atlassian Forge with no external backend or external storage.

## Documentation
- [GitBook documentation site](https://synapseworks.gitbook.io/synapseworks-docs/)
- [Documentation index](docs/index.md)
- [Synapse Forge overview](docs/synapse/overview.md)
- [Decision Register overview](docs/decision-register/overview.md)
- [Trust & Security Overview](docs/common/trust-security.md)

## Publish with GitBook

## Purpose
Provide a simple process to publish this repository to GitBook.

## Who it is for
- Documentation owners
- Product and support teams

## Prerequisites
- Access to a GitBook workspace
- Access to this Git repository

## Steps
1. Connect the repository to GitBook using Git Sync.
2. Set `docs/` as the documentation root in your GitBook configuration.
3. Use `docs/index.md` as the entry point for navigation.
4. Validate internal links after each update.
5. Publish changes from GitBook once review is complete.

## Common issues
- Wrong content root can hide pages; ensure `docs/` is selected.
- Broken relative links are usually caused by file moves without link updates.
