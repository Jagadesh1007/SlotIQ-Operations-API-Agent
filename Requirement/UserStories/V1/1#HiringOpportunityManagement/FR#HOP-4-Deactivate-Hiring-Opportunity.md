FR#HOP-4 - Deactivate Hiring Opportunity

Title: Deactivate hiring opportunities that are no longer needed

Description:
As a TA Team Admin, I want to deactivate hiring opportunities within my assigned practices, so that closed or cancelled recruitment needs are properly archived.

Business Scope:
- Mark opportunities as inactive
- Provide reason for deactivation
- Prevent modifications to deactivated opportunities
- Maintain historical record
- Clean up active opportunities list

Acceptance Criteria:
- Given a TA Team Admin
  When deactivating an opportunity in their practice
  Then the opportunity is marked as inactive with reason recorded

- Given a Master Admin
  When deactivating any opportunity
  Then the opportunity is marked as inactive with reason recorded

- Given a TA Team Admin
  When attempting to deactivate an opportunity outside their practice
  Then the request is rejected with appropriate error

- Given any authorized user
  When deactivating an opportunity with active interviews
  Then the request is rejected with appropriate message

- Given any authorized user
  When deactivating without providing a reason
  Then the request is rejected with validation message

- Given any user
  When attempting to modify a deactivated opportunity
  Then the request is rejected

Business Rules & Constraints:
- Deactivation reason is mandatory
- Cannot deactivate opportunities with active interviews
- Status must be updated to closed/cancelled
- Deactivated opportunities cannot be reactivated
- All related records must be properly archived
- Audit trail must be maintained

Out of Scope:
- UI design for deactivation
- Email notifications
- Archival process implementation
- Data purge functionality

Traceability:
- Source FR: FR#HOP-4 (FR#HOP-4 – Deactivate Hiring Opportunity.md)