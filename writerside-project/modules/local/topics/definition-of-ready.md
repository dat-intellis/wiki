# Definition of Ready

The Definition of Ready ensures that a work item (e.g., user story or task) is fully understood, refined, and ready to
be developed. It prevents the team from starting work on unclear or incomplete items, reducing rework and ensuring the
team can deliver value efficiently. By meeting the DoR, we confirm that the work item can be confidently pulled into the
sprint backlog.

## Draft Definition of Ready (DoR)

### User Story

1. **Clarity & Alignment:**
    - The user story is clearly stated in Azure Boards with a well-defined title and short summary.
    - The business value and purpose of the story are described, aligning with product goals.
    - Acceptance criteria are explicit, testable, and reflect both functional and non-functional requirements (e.g.,
      performance, security, UI/UX considerations).

2. **Dependencies & Constraints:**
    - All external dependencies (e.g., APIs from another microservice, third-party integrations, Azure services,
      credentials) are identified and documented.
    - Constraints (e.g., regulatory compliance, budget limitations) are noted.

3. **Technical Details & Feasibility:**
    - The story includes relevant architectural notes, or a reference to architectural diagrams/design docs if needed.
    - The data model and interface contracts (API specs, schema changes) are clearly defined and accessible.
    - The story can be executed locally using the defined developer setup (e.g., local Kubernetes cluster, Docker
      Compose) to ensure local parity and feasibility.

4. **Size & Estimation:**
    - The team has estimated the story (e.g., using story points) and the estimation is agreed upon by the development
      team.
    - The work is appropriately sized and can be completed within one sprint.

5. **Acceptance & Prioritization:**
    - The Product Owner (PO) has reviewed and approved the acceptance criteria.
    - The item is prioritized and ordered in the product backlog, ready to be pulled into the sprint backlog.

6. **Appropriate Documentation:**
    - Any relevant references (links to wireframes, design documents, previous tickets) are attached to the work item.
    - The story has no major unresolved questions or open-ended discussions.

### Rationale for Included Criteria

- **Clarity & Acceptance Criteria (DoR):** Ensures the team understands what to build and can confirm completion.
- **Dependencies Identified (DoR):** Minimizes blockers and surprises during implementation.
- **Estimation & Approval (DoR):** Ensures work items fit within a sprint and have been agreed upon by the team.