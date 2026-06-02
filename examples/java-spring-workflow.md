# Java/Spring Agent Workflow

This document illustrates how the agents collaborate to deliver a feature.

## 🔄 The Lifecycle of a Feature

### Phase 1: Orchestration (Maestro)
- **Action**: Receives the prompt.
- **Process**: Identifies that it's a "Spring Boot feature creation".
- **Dispatch**: Sends the request to the **Architect**.

### Phase 2: Strategic Planning (Architect)
- **Action**: Defines the API endpoints, database schema, and package structure.
- **Output**: A `PLAN.md` with "Before/After" states.
- **Review**: The **Reviewer** (Adversarial Mode) checks if the plan violates `java-clean-api.md`.

### Phase 3: Implementation (Coder)
- **Action**: Receives the approved plan.
- **Output**: Generates `@Entity`, `@Repository`, `@Service`, and `@RestController`.
- **Constraint**: Follows `code-quality.md` (naming, SOLID, etc.).

### Phase 4: Infrastructure (DevOps)
- **Action**: Scans the implementation.
- **Output**: Generates a multi-stage `Dockerfile` and `docker-compose.yml`.

### Phase 5: Verification (Reviewer)
- **Action**: Runs a `code-sec-review.md` on the generated code.
- **Action**: Performs a final coherence check.

### Phase 6: Delivery (Maestro)
- **Action**: Presents the final files, summary of changes, and a request for `git commit` authorization.
