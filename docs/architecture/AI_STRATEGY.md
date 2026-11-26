# AI strategy

## Goal and boundary

The product is intended to demonstrate AI-assisted development and selected AI capabilities inside the product. Product inference must run locally in the browser. No hosted inference API may receive user content.

## Initial direction

- Evaluate runonweb.ai as the first runtime/library candidate.
- Keep feature logic behind task-oriented provider adapters so a later approved local runtime can be substituted.
- Add a shared AI Model Manager progressively for model download, cache, lifecycle states, capability checks, and metrics.
- Use the smallest suitable local model or deterministic method for each task. A generative LLM is not required for every feature.
- Run heavy work off the UI thread when the runtime supports it and measurement shows the need.

## Candidate task families

The selected backlog includes OCR, speech-to-text, embeddings/search, classification, translation, text generation, and anonymization. These may need different models and runtimes; no single model is assumed to cover them all.

## Validation before adoption

For each candidate model/runtime pair, record:

1. Task and why a deterministic or smaller model is insufficient.
2. Runtime and exact model identifier/version.
3. License and use/redistribution conditions, reviewed for the corporate context.
4. Browser and hardware support, including WebGPU/WASM requirements and fallback.
5. Download size, memory, latency, and representative quality using synthetic test data.
6. Whether assets are fetched, cached, or available offline, and the approved delivery location.
7. Error, cancellation, progress, and unsupported-device behavior.
8. Evidence and explicit owner decision.

**Pending:** runonweb.ai compatibility with the chosen Angular/runtime setup, exact model compatibility, model licenses, browser coverage, and performance are not checked in this package.

## User experience and trust

- Show model state and progress before an action depends on a model.
- Explain unavailable, loading, failed, and ready states.
- Let users review and edit generated results before export or save.
- Do not imply model output is authoritative.
- Do not persist raw prompts or sensitive inputs for metrics by default.
- Keep runtime metrics local and minimal; define retention before collecting them.

See [AI integration rules](../rules/AI_INTEGRATION.md) and [security rules](../rules/SECURITY.md).
