# Project status

- **As of:** 2026-11-25
- **Documentation package:** Prepared
- **Angular implementation:** Not started
- **Active phase:** Phase 01 planning; implementation requires approval

## State by area

| Area | State | Notes |
|---|---|---|
| Project name and first tool | Confirmed | AI Local Tools; Bug Briefs |
| Primary users | Confirmed | Developers and QA |
| Frontend direction | Confirmed at high level | Angular, npm, Tailwind CSS, Angular CDK |
| Storage direction | Confirmed | LocalStorage for preferences; Dexie.js over IndexedDB for product data |
| Inference policy | Confirmed | Browser-local inference only; no hosted inference |
| Initial runtime candidate | Selected for evaluation | runonweb.ai; compatibility and license checks are not complete |
| Browser targets | Confirmed target | Desktop Chrome and Edge; actual model/runtime support is unverified |
| Corporate requirements | Pending | Obtain applicable security, privacy, accessibility, package, and deployment standards |
| Angular version and package compatibility | Pending validation | Select the then-current stable version and verify approved dependencies before setup |
| Model and artifact licenses | Pending | Review each model and artifact, not only the runtime library |
| Runtime/hardware compatibility | Pending | Verify browser, WebGPU/WASM path, memory, performance, and fallback for the chosen task |
| Feature order and MVP boundary | Pending | All listed Bug Briefs capabilities are selected; priority and phase assignment are not confirmed |
| Visual design | Pending | Light/dark themes are chosen; visual system is not |
| Phase 01 and 02 execution | Not started | Plans and gates are prepared in this package |

## Blocking checks before relevant implementation

1. Confirm applicable corporate policies and repository controls.
2. Check the current stable Angular release and compatibility of npm, Tailwind CSS, Angular CDK, storage, and test tooling.
3. For each proposed model, verify model-specific license and redistribution/use terms for the corporate context.
4. Test the selected runtime/model combination in desktop Chrome and Edge on representative hardware using synthetic inputs.
5. Confirm whether model files may be downloaded, where they may be hosted or cached, and expected offline behavior.
6. Agree the first vertical slice, feature order, and measurable acceptance criteria.

A pending check blocks only the affected decision or implementation. Record the outcome in a decision record and update this page. Do not report a check complete without evidence.

## Current deliverable

The package contains the root README and agent instructions, project and architecture context, concise rules, roadmap, phase 01 and 02 plans with gates, Mermaid workflow, and reusable evidence/audit/Slack/prompt templates. The Angular CLI scaffold remains a placeholder; no product features or runtime validation are included.
