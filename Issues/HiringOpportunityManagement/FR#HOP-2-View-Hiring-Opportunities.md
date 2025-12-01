# Issue Template: View Hiring Opportunities (FR#HOP-2)

### User Story
See: `Requirement/UserStories/V1/1#HiringOpportunityManagement/FR#HOP-2-View-Hiring-Opportunities.md`

### Functional Requirement
See: `Requirement/Functional/1#HiringOpportunityManagement/FR#HOP-2 – Retrieve Hiring Opportunities.md`

### Technical References
- OpenAPI Contract: `Requirement/Technical/OperationsAggregate/OperationsAggregateContracts.openapi.yml`
- Entity Definition: `Requirement/Technical/OperationsAggregate/OperationsAggregateEntities.openapi.yml`

### Implementation Scope
- [ ] API Endpoints (Minimal API)
- [ ] Logic Layer (CQRS handlers, DTOs)
- [ ] Data Layer (Entities, Repositories, SQL)
- [ ] Unit Tests

### Acceptance Criteria
- [ ] Endpoint: GET /hiringOpportunities
- [ ] Handler: GetHiringOpportunitiesQueryHandler
- [ ] Repository: GetAllHiringOpportunitiesAsync
- [ ] Entity: HiringOpportunity
- [ ] SQL: GetAllHiringOpportunities.sql

### Coding Standards & References
- Follow all instructions in the relevant AGENT.md files for each layer:
    - [API Layer](../../SlotIQ.Operations.API/AGENT.md)
    - [Logic Layer](../../SlotIQ.Operations.Logic/AGENT.md)
    - [Data Layer](../../SlotIQ.Operations.Data/AGENT.md)
    - [UnitTests Layer](../../SlotIQ.Operations.UnitTests/AGENT.md)
    - [Common Layer](../../SlotIQ.Operations.Common/AGENT.md)
- Reference these files in all related code, PRs, and reviews.

---
