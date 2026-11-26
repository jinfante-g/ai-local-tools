# Project charter

## Purpose

AI Local Tools is an internal productivity project intended to demonstrate both AI-assisted software development and useful AI capabilities inside a browser application. The product should help developers and QA while keeping application data and inference on the user's device.

## First tool: Bug Briefs

Bug Briefs will help users capture, organize, and prepare software issue reports. It is the first tool in a larger single-repository platform. A shared navigation shell can host future tools while each tool keeps its own routes and feature logic.

This is a complement to existing issue-tracking workflows, not a replacement for Jira or another system.

## Users and working model

- Initial users: developers and QA.
- Initial developer: one project owner working with a combination of AI agents.
- Repository: GitHub; feature branches and pull requests to main.
- Target local directory: /Documents/globant/ai-local-tools.
- Code and project documents: English.
- Progress reports intended for Slack: Spanish.

## Confirmed direction

| Area | Decision |
|---|---|
| Framework | Angular; target latest stable release available when implementation starts |
| Package manager | npm |
| UI | Tailwind CSS and Angular CDK |
| Themes | Light and dark |
| MVP deployment shape | Frontend-only; no backend |
| Preferences | LocalStorage |
| Product data | IndexedDB through Dexie.js |
| Local inference | runonweb.ai is the initial candidate, with adapters for other providers |
| Hosted inference | Not allowed; inference must be local |
| Initial browsers | Desktop Chrome and Edge |
| Shared AI model management | Include progressively; model download, cache, states, and metrics are in the product direction |
| Tests | Unit tests from the start; E2E progressively |
| Agent approvals | Before each phase and material changes |
| Evidence | Markdown records and screenshots |

## Scope boundaries

This package is documentation only. It does not create the GitHub repository, initialize Angular, or implement a screen.

The selected Bug Briefs capabilities are a product backlog, not a promise that all ship in the MVP. Their order, acceptance criteria, and phase assignment require planning and approval. See [requirements](features/bug-briefs/REQUIREMENTS.md).

No backend, hosted inference, or external service integration is approved by this charter. Static hosting and model artifact delivery need separate review because they may involve network access.

## Success measures to define during planning

Before implementation, agree how to measure the first useful vertical slice. Candidate measures include:

- A user can create, review, save, reopen, and export a draft issue report locally.
- Any enabled AI action runs in the browser and shows its state, limitations, and editable output.
- Core flows work in supported desktop Chrome and Edge configurations.
- A new agent can follow the repository context, obtain approval at gates, and produce reviewable evidence.

These are proposed measures; phase 01 must turn selected measures into approved acceptance criteria.

## Open questions

See [STATUS.md](STATUS.md) for unresolved corporate, compatibility, licensing, and product decisions.
