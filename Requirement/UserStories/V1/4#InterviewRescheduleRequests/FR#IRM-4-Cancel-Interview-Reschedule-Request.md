FR#IRM-4 - Cancel Interview Reschedule Request

Title: Cancel a pending interview reschedule request

Description:
As a TA Team Admin, I want to cancel pending reschedule requests within my assigned practices, so that unnecessary or incorrect requests do not affect the interview process.

Business Scope:
- Cancel reschedule requests before they are processed
- Record reason for cancellation
- Maintain audit trail of cancellations
- Ensure original interview schedule remains unchanged

Acceptance Criteria:
- Given a TA Team Admin
  When cancelling a pending request in their practice
  Then the request is marked as cancelled with reason recorded

- Given a Master Admin
  When cancelling any pending request
  Then the request is marked as cancelled with reason recorded

- Given a TA Team Admin
  When attempting to cancel a request outside their practice
  Then the request is rejected with appropriate error

- Given any authorized user
  When cancelling a processed request
  Then the request is rejected

- Given any user
  When cancelling without providing a reason
  Then the request is rejected with validation message

Business Rules & Constraints:
- Only pending requests can be cancelled
- Cancellation reason is mandatory
- Audit fields must be updated
- Original interview schedule must remain unchanged

Out of Scope:
- UI design for cancellation
- Notification system
- Approval workflow implementation
- Data purge functionality

Traceability:
- Source FR: FR#IRM-4 (FR#IRM-4 – Cancel Interview Reschedule Request.md)