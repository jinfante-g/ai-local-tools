# Proposed project structure

The following is a starting point for planning. Adjust it to the Angular version and repository conventions selected at the phase 01 gate.

~~~text
ai-local-tools/
├── README.md
├── AGENTS.md
├── docs/
│   ├── architecture/
│   ├── decisions/
│   ├── evidence/
│   ├── features/
│   ├── phases/
│   ├── prompts/
│   ├── rules/
│   ├── templates/
│   └── workflows/
└── src/
    └── app/
        ├── core/
        │   ├── ai/
        │   ├── configuration/
        │   └── storage/
        ├── layout/
        ├── shared/
        ├── features/
        │   └── bug-briefs/
        ├── app.config.ts
        └── app.routes.ts
~~~

## Boundary rules

- core owns app-wide services with a clear cross-feature responsibility.
- layout owns the shell and navigation.
- shared contains reusable UI or utilities with no feature-specific business rules.
- features/bug-briefs owns Bug Briefs routes, screens, and domain behavior.
- A feature may use approved shared capabilities; shared code must not import feature internals.
- Introduce an AI adapter only for an approved task and runtime. Avoid a generic framework until a second concrete provider/use case justifies it.

The source tree does not exist in this documentation package. This proposal is not implemented structure.
