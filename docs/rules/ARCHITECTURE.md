# Architecture rules

- Keep the application in one Angular repository with feature boundaries.
- Keep feature-specific behavior inside its feature.
- Put code in shared layers only when more than one feature needs it.
- Keep shared code independent from feature internals.
- Use lazy routes when they improve loading and ownership boundaries.
- Keep browser storage and AI runtime access behind clear services/adapters.
- Do not add a backend, microfrontend, or architecture framework without an approved requirement.
- Record material architecture decisions in an ADR.
- Treat the structure in [the proposal](../architecture/PROJECT_STRUCTURE.md) as a starting point, not a built tree.
