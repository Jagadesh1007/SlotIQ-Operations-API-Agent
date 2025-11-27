FR#IRM-3 - Update Interview Reschedule Request

Title: Modify details of an interview reschedule request

Description:
As a TA Team Admin, I want to update details of reschedule requests within my assigned practices, so that I can correct or change information before the request is processed.

Business Scope:
- Update reason or new interview slot for a reschedule request
- Track changes and maintain audit trail
- Ensure only pending requests can be updated
- Maintain accuracy of reschedule information

Acceptance Criteria:
- Given a TA Team Admin
  When updating a pending reschedule request in their practice
  Then the changes are saved successfully

- Given a Master Admin
  When updating any reschedule request
  Then the changes are saved successfully

- Given a TA Team Admin
  When attempting to update a request outside their practice
  Then the request is rejected with appropriate error

- Given any user
  When updating with invalid data
  Then the request is rejected with validation messages

- Given any authorized user
  When updating a processed request
  Then the request is rejected

Business Rules & Constraints:
- Only pending requests can be updated
- Reason and new slot must remain valid
- Audit fields must be updated
- Cannot update requests after approval/rejection

Out of Scope:
- UI design for update form
- Notification system
- Approval workflow implementation
- Version history display

Traceability:
- Source FR: FR#IRM-3 (FR#IRM-3 – Update Interview Reschedule Request.md)