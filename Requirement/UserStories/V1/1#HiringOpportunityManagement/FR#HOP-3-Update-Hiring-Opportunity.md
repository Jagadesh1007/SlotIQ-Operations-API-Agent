FR#HOP-3 - Update Hiring Opportunity

Title: Modify existing hiring opportunity details

Description:
As a TA Team Admin, I want to update hiring opportunity details within my assigned practices, so that I can keep the recruitment requirements current and accurate.

Business Scope:
- Modify opportunity details like title, description, and planned count
- Update status of opportunities
- Track changes through audit fields
- Maintain accuracy of recruitment needs

Acceptance Criteria:
- Given a TA Team Admin
  When updating an opportunity within their practice
  Then the changes are saved successfully

- Given a Master Admin
  When updating any hiring opportunity
  Then the changes are saved successfully

- Given a TA Team Admin
  When attempting to update an opportunity outside their practice
  Then the request is rejected with appropriate error

- Given any user
  When updating with invalid data
  Then the request is rejected with validation messages

- Given any authorized user
  When updating a non-existent opportunity
  Then appropriate error message is displayed

- Given any authorized user
  When updating status
  Then only valid status transitions are allowed

Business Rules & Constraints:
- Cannot change practice assignment
- Title must remain 5-50 characters
- Planned candidates count must stay within 0-50
- All mandatory fields must remain populated
- Modified date and user must be updated
- Status transitions must follow defined workflow
- Cannot update deactivated opportunities

Out of Scope:
- UI design for edit form
- Email notifications for changes
- Version history display
- Approval workflow

Traceability:
- Source FR: FR#HOP-3 (FR#HOP-3 – Update Hiring Opportunity.md)