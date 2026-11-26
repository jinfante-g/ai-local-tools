# Phase 01: Foundations and project

**State:** Planned; implementation not started.

**Purpose:** Establish an approved foundation for AI Local Tools and a small, demonstrable first product slice.

## Outcomes

- A reviewed project charter and README explain the idea, users, and boundaries.
- Repository and development tooling follow confirmed corporate requirements.
- An approved Bug Briefs first slice has measurable acceptance criteria.
- A thin first screen or vertical slice is implemented only after the gates below.
- Any AI behavior in the slice passes the model/runtime/license gate; otherwise its deferral is recorded and approved.
- Work has reviewable test results, evidence, and an independent audit.

This package prepares documentation; it does not perform these implementation tasks.

## In scope after approval

- Create or prepare the GitHub repository and root README.
- Confirm applicable corporate constraints and repository controls.
- Select and verify the current stable Angular version, npm tooling, Tailwind CSS, Angular CDK, storage, and test setup.
- Agree the first screen/vertical slice for Bug Briefs and its acceptance criteria.
- Implement the approved slice, possibly using synthetic/sample data until persistence and AI decisions are approved.
- Evaluate one bounded local AI task only if the owner approves it and its specific model/runtime passes the gate.
- Record implementation, tests, decisions, screenshots, and limitations.

## Out of scope

- Implementing all 16 selected Bug Briefs capabilities.
- Building a general-purpose AI framework before a real use case needs it.
- Hosted inference, a backend, or unapproved integrations.
- Assuming a model is compatible or licensed because its library is open source.
- Treating this documentation ZIP as a completed project phase.

## Gates

### Gate 0 — Organizational and repository readiness

**Review:** applicable security/privacy/accessibility standards; package and repository restrictions; GitHub/branch/PR expectations; approved development environment.

**Pass when:** the owner confirms applicable requirements or records which remain out of scope for the first slice. Resolve blocking policy conflicts before affected implementation.

### Gate 1 — Phase plan approval

**Review:** proposed repository/app setup, selected first slice, scope, acceptance criteria, dependencies, test approach, risks, and estimated steps.

**Pass when:** the owner explicitly approves the phase plan. An agent must not start implementation before this approval.

### Gate 2 — Technical and AI feasibility

**Review:** current stable Angular/package compatibility; browser/device test; exact model/runtime identifiers; model and artifact licenses; download/cache/network behavior; measured size, memory, latency, and quality using synthetic data.

**Pass when:** technologies used in the slice are approved and required checks are recorded. If AI remains unverified, either defer it through an owner-approved decision or keep that feature blocked.

### Gate 3 — Phase acceptance

**Review:** change summary, acceptance checklist, test results, screenshots, known limitations, and independent audit.

**Pass when:** criteria are met, material findings are resolved or explicitly accepted by the owner, documentation is updated, and the owner records phase acceptance.

## Deliverables

- Reviewed repository README and initial project documentation.
- Approved source baseline and one approved first product slice, if implementation is authorized.
- Decision records for unresolved or material technical choices.
- Phase evidence and audit record.
- Updated [status](../../STATUS.md).

Use [TASKS.md](TASKS.md) and [ACCEPTANCE.md](ACCEPTANCE.md). Phase 02 begins only after phase 01 acceptance; that does not automatically authorize phase 02 implementation.
