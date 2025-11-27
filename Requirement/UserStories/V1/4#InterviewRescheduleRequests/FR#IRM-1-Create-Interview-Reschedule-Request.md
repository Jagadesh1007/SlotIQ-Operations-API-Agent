FR#IRM-1 - Create Interview Reschedule Request

Title: Request to reschedule a candidate interview

Description:
As a TA Team Admin, I want to request a reschedule for candidate interviews within my assigned practices, so that interviews can be moved to a more suitable time when needed.

Business Scope:
- Submit reschedule requests for scheduled interviews
- Provide reason for rescheduling
- Ensure new time slot is available
- Track status of reschedule requests
- Notify relevant parties of changes

Acceptance Criteria:
- Given a TA Team Admin
  When submitting a valid reschedule request
  Then the request is created and tracked with a unique ID

- Given a Master Admin
  When submitting a reschedule request for any interview
  Then the request is created successfully

- Given any user
  When submitting a request with missing or invalid details
  Then the request is rejected with clear validation messages

- Given any authorized user
  When submitting a request for a non-existent interview
  Then the request is rejected with appropriate error

Business Rules & Constraints:
- Reason for rescheduling is mandatory
- New interview slot must be available and not conflict
- Only active interviews can be rescheduled
- Request status must be tracked
- Audit fields must be maintained

Out of Scope:
- UI design for request submission
- Notification templates
- Approval workflow implementation
- Calendar integration

Traceability:
- Source FR: FR#IRM-1 (FR#IRM-1 – Create Interview Reschedule Request.md)