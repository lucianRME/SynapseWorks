# SynapseWorks Documentation

This repository contains GitBook-ready Markdown documentation for the SynapseWorks product portfolio.

SynapseWorks builds privacy-first workflow tools for Jira teams, safer everyday web use, and local Android document handling. Synapse and Decision Register are Jira/Atlassian products, Submit Guard is a Chrome extension, and RME: Private PDF Scanner is a privacy-first Android document scanner with a private on-device library, multilingual OCR, document tools, and user-controlled export. RME is publicly available on [Google Play](https://play.google.com/store/apps/details?id=org.synapseworks.pageharbor).

## Documentation
- [GitBook documentation site](https://synapseworks.gitbook.io/synapseworks-docs/)
- [Documentation index](docs/index.md)
- [Synapse Forge overview](docs/synapse/overview.md)
- [Decision Register overview](docs/decision-register/overview.md)
- [Submit Guard overview](docs/submit-guard/overview.md)
- [RME: Private PDF Scanner overview](docs/rme-pdf-scanner/overview.md)
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
2. Preserve the published space's existing `./docs` Git Sync mapping. Its configuration is `docs/.gitbook.yaml`, with `root: ./` and `index.md` as the entry point. The repository-root `.gitbook.yaml` supports the existing root-level sync with `root: ./docs/`.
3. GitBook derives the sidebar from the documentation folders and page titles; `docs/index.md` also provides the product navigation.
4. Validate internal links after each update.
5. Publish changes from GitBook once review is complete.

## Common issues
- Wrong content root can hide pages; ensure `docs/` is selected.
- Broken relative links are usually caused by file moves without link updates.
- Both `.gitbook.yaml` files map the former `pageharbor` landing route and its four child routes directly to their RME PDF Scanner destinations using [GitBook-supported redirects](https://gitbook.com/docs/docs-as-code/git-sync/content-configuration). Keep their redirect maps identical and preserve these compatibility rules when moving pages again.
- After pushing to the connected branch, confirm Git Sync has imported the commit. If the published site has not updated, open the SynapseWorks Docs space in GitBook, review the synced content, and publish it to the existing site. Check both the canonical RME PDF Scanner routes and the legacy redirects.
- This Markdown-only repository has no configured build, test runner, or link checker. Validate relative Markdown links, GitBook redirect targets, and `git diff --check` before publishing.
