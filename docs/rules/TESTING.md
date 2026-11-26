# Testing rules

- Add unit tests from the start for non-trivial behavior and important edge cases.
- Add E2E tests progressively for the main user journeys.
- Test storage boundaries, migrations, failures, and recovery before relying on persistent data.
- Keep model tests reproducible with pinned model/runtime identifiers or deterministic fixtures; do not rely only on subjective output inspection.
- Use synthetic data for AI tests and screenshots.
- Cover unsupported browser/runtime, model-loading, cancellation, and inference-error states for enabled AI features.
- Record exactly which checks ran and their result. Never report an unrun check as passed.
- Keep test commands aligned with approved project tooling.
