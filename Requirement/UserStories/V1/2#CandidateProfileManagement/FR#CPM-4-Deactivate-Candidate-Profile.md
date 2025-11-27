FR#CPM-4 - Deactivate Candidate Profile

Title: Deactivate candidate profiles no longer under consideration

Description:
As a TA Team Admin, I want to deactivate candidate profiles within my assigned practices, so that I can maintain a clean and relevant candidate pool.

Business Scope:
- Mark profiles as inactive
- Record deactivation reason
- Prevent profile modifications
- Archive candidate information
- Maintain historical records
- Clean up active candidates list

Acceptance Criteria:
- Given a TA Team Admin
  When deactivating a profile in their practice
  Then the profile is marked as inactive with reason recorded

- Given a Master Admin
  When deactivating any profile
  Then the profile is marked as inactive with reason recorded

- Given a TA Team Admin
  When attempting to deactivate a profile outside their practice
  Then the request is rejected with appropriate error

- Given any authorized user
  When deactivating a profile with pending interviews
  Then the request is rejected with appropriate message

- Given any authorized user
  When deactivating without providing a reason
  Then the request is rejected with validation message

- Given any user
  When attempting to modify a deactivated profile
  Then the request is rejected

Business Rules & Constraints:
- Deactivation reason is mandatory
- Cannot deactivate profiles with pending interviews
- Deactivated profiles cannot be reactivated
- Related documents must be archived
- Audit trail must be maintained
- Profile history must be preserved

Out of Scope:
- UI design for deactivation
- Document archival process
- Notification system
- Data purge functionality
- Recovery process

Traceability:
- Source FR: FR#CPM-4 (FR#CPM-4 – Deactivate Candidate Profile.md)