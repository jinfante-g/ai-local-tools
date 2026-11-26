# Architecture overview

## Proposed shape

A single Angular application hosts a shared workspace shell and separate feature areas. Bug Briefs is the first feature. Shared navigation and genuinely reusable capabilities can support later tools; feature-specific screens and business rules remain inside their feature.

~~~text
Browser application
├── Shared shell and navigation
├── Shared platform capabilities
│   ├── Local AI adapters and model lifecycle
│   ├── Local storage
│   └── Shared UI primitives
└── Feature areas
    └── Bug Briefs
~~~

This is a proposed organization based on confirmed product direction. It is not implemented or validated against a repository.

## Runtime boundary

- Frontend-only application; no application backend is planned for the MVP.
- Inference runs on the device in the browser.
- Model downloads or static asset delivery may still use a network. Review separately from inference and confirm approved hosting, caching, and offline behavior.
- Initial browser targets are desktop Chrome and Edge.
- User data stays in browser storage unless the owner approves a specific export or integration flow.

## Modularity

Use feature boundaries and lazy routes where useful. Shared code is for capabilities used by multiple features, not speculative abstractions. AI libraries should be isolated behind task-oriented adapters so feature code does not depend on vendor APIs.

## Important constraints

- Verify corporate standards before selecting versions, dependencies, hosting, or model assets.
- Verify browser/runtime/model compatibility and resource use before committing to an AI feature.
- Review every model's license individually.
- Make AI output visible, editable, and explicitly a suggestion where users rely on it.
- Keep [architecture rules](../rules/ARCHITECTURE.md) and [AI rules](../rules/AI_INTEGRATION.md) current as decisions are validated.
