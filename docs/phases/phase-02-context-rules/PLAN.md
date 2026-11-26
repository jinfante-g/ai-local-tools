# Phase 02: Context and rules

**State:** Planned; implementation not started.

**Purpose:** Give AI agents compact, persistent project context and verify they follow it before broader spec-led work begins.

## Outcomes

- Root agent instructions point to concise, authoritative project context.
- Architecture, Angular, code style, AI, security, testing, and documentation rules are short and actionable.
- Open decisions remain visibly pending instead of being treated as facts.
- A controlled agent exercise checks compliance with the rules.
- Findings and revisions are documented and approved.

## In scope after approval

- Review phase 01 learnings and applicable corporate requirements.
- Refine AGENTS.md, project status, architecture overview, and rule files.
- Define which files agents must read for each task and when they must request gate approval.
- Run a bounded evaluation with synthetic context and a representative plan/change proposal.
- Check English documentation, local-only inference, privacy handling, scope discipline, testing claims, and approval behavior.
- Record deviations, rule changes, and evidence.

## Out of scope

- Building specialized agent configurations or reusable skills (phases 04 and 05).
- Automating approvals or granting agents merge/publish authority.
- Implementing a product feature solely to test rule compliance.
- Claiming an agent is reliable based on one successful prompt.

## Gates

### Gate 0 — Context and authority review

**Review:** current phase 01 decisions, corporate policies, project context, and existing instructions.

**Pass when:** the owner confirms authoritative sources and resolves conflicts that affect the rules.

### Gate 1 — Rule set approval

**Review:** concise rule changes, affected files, expected behavior, evaluation cases, and risks.

**Pass when:** the owner explicitly approves the rules and evaluation plan before the exercise.

### Gate 2 — Agent compliance evaluation

**Review:** exact prompt/context, agent output, checklist results, deviations, and remediation.

**Pass when:** mandatory behaviors pass the agreed evaluation or remaining failures are addressed and the owner approves an explicit limitation. One trial is evidence of a trial, not proof of general reliability.

### Gate 3 — Phase acceptance

**Review:** final rule files, evaluation record, audit findings, and updated status.

**Pass when:** instructions are consistent and concise, critical checks pass, findings are resolved or accepted, and the owner records acceptance.

## Deliverables

- Approved persistent context and concise rule set.
- Agent execution and audit prompts fit for reuse.
- Dated evaluation record with evidence and limitations.
- Updated [status](../../STATUS.md).

Use [TASKS.md](TASKS.md) and [ACCEPTANCE.md](ACCEPTANCE.md). Phase 03 requires separate approval.
