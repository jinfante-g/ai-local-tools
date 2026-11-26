# Bug Briefs: selected requirements

The owner selected these capabilities for the product direction. Selection records interest; it does not confirm priority, MVP inclusion, delivery phase, feasibility, or acceptance criteria. Confirm those through a reviewed feature spec.

## Selected capabilities

1. Incident dashboard.
2. Bug report editor.
3. Screenshot and evidence attachments.
4. OCR to extract error messages.
5. Report generation using templates.
6. Export and copy as Markdown or JSON.
7. Local history and persistence.
8. Basic model management.
9. Semantic search and duplicate detection.
10. Dictation with Whisper.
11. Automatic bug classification.
12. Translate reports into English.
13. Report generation with a local LLM.
14. Sensitive-information anonymization.
15. Test-case generation.
16. Offline support and PWA behavior.

## Constraints that apply

- The MVP is frontend-only and targets desktop Chrome and Edge.
- Product inference must remain local.
- Preferences use LocalStorage; structured product data uses IndexedDB via Dexie.js.
- Model/runtime compatibility, browser coverage, licensing, network behavior, and performance require validation.
- AI output must be reviewable and editable.
- Corporate requirements remain pending.

## Planning fields required per feature

For each capability, create a spec that states the user problem, priority, dependencies, data handled, local model/runtime if any, acceptance criteria, error states, accessibility needs, tests, evidence, and known limitations.
