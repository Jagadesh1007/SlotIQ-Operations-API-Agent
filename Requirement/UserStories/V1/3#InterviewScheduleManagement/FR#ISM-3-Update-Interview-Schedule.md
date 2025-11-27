FR#ISM-3 - Update Interview Schedule

Title: Modify existing interview schedule details

Description:
As a TA Team Admin, I want to update interview schedule details within my assigned practices, so that I can maintain accurate and current interview information.

Business Scope:
- Update interview time slots
- Change panel members
- Modify interview notes
- Update interview type
- Maintain schedule accuracy
- Track schedule modifications

Acceptance Criteria:
- Given a TA Team Admin
  When updating a schedule within their practice
  Then the changes are saved and notifications sent

- Given a Master Admin
  When updating any interview schedule
  Then the changes are saved successfully

- Given a TA Team Admin
  When attempting to update a schedule outside their practice
  Then the request is rejected with appropriate error

- Given any authorized user
  When updating to an unavailable time slot
  Then the request is rejected with conflict message

- Given any authorized user
  When updating a completed interview
  Then the request is rejected with appropriate message

- Given any authorized user
  When updating with invalid panel member
  Then the request is rejected with validation message

Business Rules & Constraints:
- Cannot modify completed interviews
- New time slot must be available
- Panel member must be available
- Calendar invites must be updated
- All participants must be notified
- Modified date and user must be updated
- Status transitions must be valid

Out of Scope:
- UI design for edit interface
- Calendar integration details
- Email template design
- Notification system implementation
- Approval workflow

Traceability:
- Source FR: FR#ISM-3 (FR#ISM-3 – Update Interview Schedule.md)