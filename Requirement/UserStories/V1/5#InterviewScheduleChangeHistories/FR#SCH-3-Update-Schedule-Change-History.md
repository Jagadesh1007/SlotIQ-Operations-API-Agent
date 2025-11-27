FR#SCH-3 - Update Interview Schedule Change History

Title: Update details of interview schedule change history records

Description:
As a TA Team Admin, I want to update details of schedule change history records within my assigned practices, so that corrections and clarifications can be made for audit purposes.

Business Scope:
- Update reason or status for history records
- Maintain audit trail of changes
- Ensure only authorized users can update history
- Support compliance and reporting needs

Acceptance Criteria:
- Given a TA Team Admin
  When updating a history record in their practice
  Then the changes are saved successfully

- Given a Master Admin
  When updating any history record
  Then the changes are saved successfully

- Given a TA Team Admin
  When attempting to update a history record outside their practice
  Then the request is rejected with appropriate error

- Given any user
  When updating with invalid data
  Then the request is rejected with validation messages

Business Rules & Constraints:
- Only authorized users can update history
- Reason and status must remain valid
- Audit fields must be updated
- Practice-specific access controls

Out of Scope:
- UI design for update form
- Notification system
- Data export functionality
- Manual history record creation

Traceability:
- Source FR: FR#SCH-3 (FR#SCH-3 – Update Schedule Change History.md)