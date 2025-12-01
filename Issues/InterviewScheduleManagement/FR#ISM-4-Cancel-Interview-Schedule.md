# Issue Template: Cancel Interview Schedule (FR#ISM-4)

### User Story
See: `Requirement/UserStories/V1/3#InterviewScheduleManagement/FR#ISM-4-Cancel-Interview-Schedule.md`

### Functional Requirement
See: `Requirement/Functional/3#InterviewScheduleManagement/FR#ISM-4 – Cancel Interview Schedule.md`

### Technical References
- OpenAPI Contract: `Requirement/Technical/OperationsAggregate/OperationsAggregateContracts.openapi.yml`
- Entity Definition: `Requirement/Technical/OperationsAggregate/OperationsAggregateEntities.openapi.yml`

### Implementation Scope
- [ ] API Endpoints (Minimal API)
- [ ] Logic Layer (CQRS handlers, DTOs)
- [ ] Data Layer (Entities, Repositories, SQL)
- [ ] Unit Tests

### Acceptance Criteria
- [ ] Endpoint: DELETE /interviewSchedules/{interviewScheduleID}
- [ ] Handler: CancelInterviewScheduleCommandHandler
- [ ] Repository: CancelInterviewScheduleAsync
- [ ] Entity: InterviewSchedule
- [ ] SQL: CancelInterviewSchedule.sql

### Coding Standards & References
- Follow all instructions in the relevant AGENT.md files for each layer:
    - [API Layer](../../SlotIQ.Operations.API/AGENT.md)
    - [Logic Layer](../../SlotIQ.Operations.Logic/AGENT.md)
    - [Data Layer](../../SlotIQ.Operations.Data/AGENT.md)
    - [UnitTests Layer](../../SlotIQ.Operations.UnitTests/AGENT.md)
    - [Common Layer](../../SlotIQ.Operations.Common/AGENT.md)
- Reference these files in all related code, PRs, and reviews.

---
