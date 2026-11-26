# Development workflow

Use this workflow for each phase and material change. Human approval gates are intentional: agents prepare and execute approved work but do not approve their own scope.

~~~mermaid
flowchart TD
    A[Read AGENTS, status, project context] --> B[Review phase plan and acceptance criteria]
    B --> C[Check open policy, compatibility, and license items]
    C --> D[Prepare a bounded implementation plan]
    D --> E{Human approves phase or material change?}
    E -->|No| F[Revise plan or stop affected work]
    F --> D
    E -->|Yes| G[Implement on feature branch]
    G --> H[Run approved checks and capture evidence]
    H --> I[Independent audit]
    I --> J{Critical findings or unmet criteria?}
    J -->|Yes| K[Fix findings and update evidence]
    K --> H
    J -->|No| L[Update docs, status, and decision records]
    L --> M[Open pull request to main]
    M --> N{Owner accepts phase?}
    N -->|No| O[Address review feedback]
    O --> H
    N -->|Yes| P[Record acceptance and close phase]
    P --> Q[Request approval for next phase]
~~~

## Gate behavior

- The plan names scope, affected files/areas, risks, validation, and evidence.
- Explicit approval is required before phase implementation and material scope/architecture changes.
- If a check blocks one optional feature, isolate it and record the decision rather than silently changing policy.
- Audit findings are not self-approved. The owner decides whether a non-critical limitation can be accepted.
- Merge remains subject to repository branch protection and review policy.
