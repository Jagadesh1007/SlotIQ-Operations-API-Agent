FR#CPM-1 - Create Candidate Profile

Title: Create new candidate profiles for interview process

Description:
As a TA Team Admin, I want to create candidate profiles within my assigned practices, so that I can manage candidate information throughout the interview process.

Business Scope:
- Record candidate personal and professional information
- Link candidates to hiring opportunities
- Assign appropriate designations
- Store resume references
- Track candidate sources
- Enable interview scheduling

Acceptance Criteria:
- Given a TA Team Admin
  When creating a profile with valid details
  Then the profile is created with a unique ID

- Given a Master Admin
  When creating a profile for any practice
  Then the profile is created successfully

- Given any user
  When creating a profile with invalid email format
  Then the request is rejected with validation message

- Given any user
  When creating a profile with duplicate email
  Then the request is rejected for duplication

- Given any authorized user
  When creating a profile with invalid designation
  Then the request is rejected with appropriate error

- Given any authorized user
  When creating a profile with invalid hiring opportunity
  Then the request is rejected with appropriate error

Business Rules & Constraints:
- First and last names are mandatory (1-50 characters)
- Email must be unique and valid format (max 250 characters)
- Years of experience must be positive number
- Resume document reference is mandatory
- Designation must be valid (applied and presented)
- Must be linked to valid hiring opportunity
- Candidate source must be specified

Out of Scope:
- UI design for profile creation
- Resume upload mechanism
- Email verification process
- Duplicate detection algorithms
- Integration with external systems

Traceability:
- Source FR: FR#CPM-1 (FR#CPM-1 – Create Candidate Profile.md)