# Definition of Done

The Definition of Done ensures that each increment delivered by the team meets the agreed-upon quality benchmarks and
can be considered potentially shippable. The DoD reduces technical debt, enhances maintainability, and ensures
consistency across the microservices and frontend codebases. Meeting the DoD guarantees that completed items add
measurable value and are ready to be demonstrated or released.

## Draft Definition of Done (DoD)

### User Story

1. **Code Quality & Review:**
    * Code is committed, pushed to GitHub, and associated with the correct branch (following naming conventions).
    * Code passes automated CI checks (build, unit tests, linting).
    * Code has been peer-reviewed and approved via pull requests, adhering to the team’s coding standards and
      guidelines (e.g., .NET conventions, React best practices).

2. **Testing & Verification:**
    * All acceptance criteria are met and verified against the requirements in Azure Boards.
    * All unit tests and integration tests related to the change pass successfully.
    * API contracts are validated, and integration between microservices is tested where applicable.
    * Any new UI components are validated both functionally and for accessibility where practical.
    * Tests adequately covers the changed areas, or meets the team’s agreed-upon coverage threshold (e.g., 80%).

3. **Documentation & Artifacts:**
    * Relevant documentation is updated (e.g., README, architecture diagrams, API contracts, microservice READMEs) to
      reflect the changes.
    * User-facing documentation or release notes are updated if the new feature or fix affects end-users or support
      staff.
    * Infrastructure-as-Code templates (e.g., Bicep, Terraform) or Kubernetes manifests are updated if the change
      requires environment configuration adjustments.

4. **Deployment & Environment Validation:**
    * The feature is successfully deployed to the development or test environment using the GitOps pipeline (e.g.,
      GitHub Actions + Argo CD) and verified to run correctly on Kubernetes.
    * Smoke tests or basic end-to-end tests pass in the test environment.
    * The feature can be demonstrated in the demo environment if required.

5. **Business & Stakeholder Review:**
    * The Product Owner (or delegated business stakeholder) confirms that the acceptance criteria are fulfilled.
    * The increment is ready for the Sprint Review or can be potentially released to Production.

6. **No Known Regressions or Critical Issues:**
    * No unresolved high-severity bugs or regressions have been introduced by the change.
    * Known issues (if any) are documented and tracked as separate backlog items if they are not blocking release.

### Rationale for Included Criteria

* **Code Review & CI Checks (DoD):** Ensures quality and consistency across code contributions.
* **Automated Testing (DoD):** Guarantees reliability and reduces regressions in a microservices environment.
* **Documentation Updates (DoD):** Maintains long-term maintainability, enabling easier onboarding and troubleshooting.
* **Verified Deployment (DoD):** Ensures the feature is actually running as expected in the environment, aligned with
  GitOps principles.
