FR#HOP-1 - Create Hiring Opportunity

Title: Create new hiring opportunities for interview requirements

Description:
As a TA Team Admin, I want to create hiring opportunities for my assigned practice, so that I can initiate the interview process for required positions.

Business Scope:
- Create new hiring opportunities with required details like title, job description, and planned candidate count
- Assign opportunities to specific practices
- Specify opportunity category (Forecast or Client Requirements)
- Track status of hiring needs
- Enable efficient candidate recruitment process

Acceptance Criteria:
- Given a TA Team Admin with valid practice assignment
  When creating a hiring opportunity with all required information
  Then the opportunity is created and a unique ID is returned

- Given a TA Team Admin
  When creating an opportunity with invalid practice assignment
  Then the request is rejected with appropriate error message

- Given a Master Admin
  When creating a hiring opportunity for any practice
  Then the opportunity is created successfully

- Given any user
  When creating an opportunity with missing required fields
  Then the request is rejected with clear validation messages

- Given any user
  When creating an opportunity with invalid category
  Then the request is rejected with appropriate error message

- Given any user
  When creating an opportunity with planned candidates count > 50
  Then the request is rejected for exceeding maximum limit

Business Rules & Constraints:
- Title must be 5-50 characters
- Job description is mandatory
- Planned candidates count must be 0-50
- Practice must be valid and active
- Opportunity category must be valid (Forecast/ClientRequirements)
- Status is automatically set to "Open" for new opportunities
- All audit fields (created date, modified date, source) are mandatory

Out of Scope:
- UI design for opportunity creation form
- Email notifications
- Document attachments
- Integration with external systems

Traceability:
- Source FR: FR#HOP-1 (FR#HOP-1 – Create Hiring Opportunity.md)