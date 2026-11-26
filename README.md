# AI Local Tools

A local-first, browser-based toolkit for developers and QA. Bug Briefs is the first planned tool in a modular Angular application.

**Package status:** Project documentation and planning; the existing Angular CLI scaffold is still a placeholder, with no product features. See [project status](docs/STATUS.md).

## Start here

1. Read [project context](docs/PROJECT.md) and the [documentation index](docs/INDEX.md).
2. Read [AGENTS.md](AGENTS.md) before using an AI agent in this repository.
3. Review the [roadmap](docs/ROADMAP.md) and [development workflow](docs/workflows/DEVELOPMENT.md).
4. Resolve the open checks in [project status](docs/STATUS.md) and obtain phase approval before implementation.

## Product direction

AI Local Tools is intended to host multiple productivity tools behind shared navigation and shared capabilities. Bug Briefs is the first planned tool for capturing and preparing software issue reports.

The app is planned as frontend-only. Product inference must run locally in the browser; sending user content to hosted inference services is out of scope.

## Confirmed technical direction

- Angular, targeting the latest stable release available when implementation begins
- npm; GitHub; feature branches and pull requests to main
- Tailwind CSS and Angular CDK; light and dark themes
- Desktop Chrome and Edge as initial browser targets
- LocalStorage for preferences; IndexedDB through Dexie.js for application data
- runonweb.ai as the initial local-inference candidate, behind adapters
- Unit tests from the start; E2E coverage added progressively
- English for code and project documentation; Spanish for Slack progress updates

These decisions are not proof that dependencies or models have been validated. Corporate requirements, runtime compatibility, and model licenses remain open. See [status](docs/STATUS.md).

## Planned feature area

The selected Bug Briefs feature set is listed in [its requirements](docs/features/bug-briefs/REQUIREMENTS.md). Selection does not mean implementation or a confirmed delivery order.

## Scope of this package

This archive prepares project context, rules, the eight-phase roadmap, detailed plans and gates for phases 01 and 02, workflow diagrams, and reusable evidence, audit, Slack, and agent prompt templates. It does not create the repository, initialize Angular, or implement product features.
