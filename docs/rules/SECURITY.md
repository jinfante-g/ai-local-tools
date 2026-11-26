# Security and privacy rules

- Assume issue text, screenshots, logs, OCR, transcripts, and model output may contain sensitive data.
- Use synthetic or explicitly approved data in development, demos, prompts, tests, and evidence.
- Never commit secrets, credentials, customer data, or unredacted internal screenshots.
- Keep inference local. Do not transmit issue content to an external model or service.
- Treat model downloads, browser caches, package downloads, and static hosting as separate network/data flows that need review.
- Validate imported files, size/type limits, persisted records, and exported content.
- Avoid unnecessary persistence; explain what is stored and provide a reviewed deletion path.
- Do not claim anonymization is complete or guaranteed. Require human review of redacted output.
- Follow corporate security, privacy, retention, and accessibility standards once obtained.
- Record a security-relevant deviation and stop affected work until the owner resolves it.
