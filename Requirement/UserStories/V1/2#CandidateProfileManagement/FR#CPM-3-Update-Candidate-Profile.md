FR#CPM-3 - Update Candidate Profile

Title: Modify existing candidate profile information

Description:
As a TA Team Admin, I want to update candidate profiles within my assigned practices, so that I can maintain accurate and current candidate information.

Business Scope:
- Update candidate personal information
- Modify professional details
- Update resume references
- Change designations
- Maintain data accuracy
- Track profile modifications

Acceptance Criteria:
- Given a TA Team Admin
  When updating a profile within their practice
  Then the changes are saved successfully

- Given a Master Admin
  When updating any candidate profile
  Then the changes are saved successfully

- Given a TA Team Admin
  When attempting to update a profile outside their practice
  Then the request is rejected with appropriate error

- Given any user
  When updating with invalid email format
  Then the request is rejected with validation message

- Given any authorized user
  When updating designation
  Then only valid designations are accepted

- Given any authorized user
  When updating a non-existent profile
  Then appropriate error message is displayed

Business Rules & Constraints:
- Email must remain unique if changed
- Names must be 1-50 characters
- Experience must be positive number
- New resume reference must be valid
- Cannot change linked hiring opportunity
- Modified date and user must be updated
- Cannot update deactivated profiles

Out of Scope:
- UI design for edit form
- Resume update mechanism
- Email verification process
- Version history display
- Notification system

Traceability:
- Source FR: FR#CPM-3 (FR#CPM-3 – Update Candidate Profile.md)