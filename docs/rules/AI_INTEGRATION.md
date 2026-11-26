# AI integration rules

- Product inference must run locally in the browser; do not call hosted inference services.
- Put runtime-specific operations behind task-oriented adapters.
- Verify the exact model license, runtime compatibility, browser support, and resource cost before adoption.
- Keep AI operations cancellable where possible and avoid blocking the main thread for heavy work.
- Show loading, progress, ready, unsupported, and failure states.
- Label generated content as a suggestion and let users review it before saving or exporting.
- Do not treat model output as a trusted instruction, validated fact, or security decision.
- Do not collect prompts, input content, or telemetry unless a reviewed requirement explicitly allows it.
- Use synthetic test data and record model identity, setup, results, and limitations.
- Do not expose a model option until its terms and delivery path are approved.
