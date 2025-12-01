# Issue Template: View Candidate Profiles (FR#CPM-2)

### User Story
See: `Requirement/UserStories/V1/2#CandidateProfileManagement/FR#CPM-2-View-Candidate-Profiles.md`

### Functional Requirement
See: `Requirement/Functional/2#CandidateProfileManagement/FR#CPM-2 – Retrieve Candidate Profiles.md`

### Technical References
- OpenAPI Contract: `Requirement/Technical/OperationsAggregate/OperationsAggregateContracts.openapi.yml`
- Entity Definition: `Requirement/Technical/OperationsAggregate/OperationsAggregateEntities.openapi.yml`

### Implementation Scope
- [ ] API Endpoints (Minimal API)
- [ ] Logic Layer (CQRS handlers, DTOs)
- [ ] Data Layer (Entities, Repositories, SQL)
- [ ] Unit Tests

### Acceptance Criteria
- [ ] Endpoint: GET /candidateProfiles
- [ ] Handler: GetCandidateProfilesQueryHandler
- [ ] Repository: GetAllCandidateProfilesAsync
- [ ] Entity: CandidateProfile
- [ ] SQL: GetAllCandidateProfiles.sql

### Coding Standards & References
- Follow all instructions in the relevant AGENT.md files for each layer:
    - [API Layer](../../SlotIQ.Operations.API/AGENT.md)
    - [Logic Layer](../../SlotIQ.Operations.Logic/AGENT.md)
    - [Data Layer](../../SlotIQ.Operations.Data/AGENT.md)
    - [UnitTests Layer](../../SlotIQ.Operations.UnitTests/AGENT.md)
    - [Common Layer](../../SlotIQ.Operations.Common/AGENT.md)
- Reference these files in all related code, PRs, and reviews.

---
