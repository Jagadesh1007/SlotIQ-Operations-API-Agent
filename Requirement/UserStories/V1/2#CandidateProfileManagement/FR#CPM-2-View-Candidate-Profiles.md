FR#CPM-2 - View Candidate Profiles

Title: Search and view candidate profiles with filtering options

Description:
As a TA Team Admin, I want to search and view candidate profiles within my assigned practices, so that I can manage and track candidates effectively throughout the interview process.

Business Scope:
- View list of candidate profiles with pagination
- Search candidates by various criteria
- Filter by hiring opportunity, designation, experience
- Access detailed candidate information
- Track candidate status in interview process

Acceptance Criteria:
- Given a TA Team Admin
  When viewing candidate profiles
  Then only profiles from assigned practices are displayed

- Given a Master Admin
  When viewing candidate profiles
  Then profiles from all practices are displayed

- Given any authorized user
  When applying search filters
  Then matching candidates are displayed

- Given any authorized user
  When specifying page size and number
  Then correct subset of results is returned

- Given any authorized user
  When searching by experience range
  Then candidates within that range are displayed

- Given any user
  When providing invalid search criteria
  Then appropriate error message is displayed

Business Rules & Constraints:
- Default page size is 10 profiles
- Maximum page size is 50 profiles
- Search by name, email, or designation
- Filter by experience range
- Filter by hiring opportunity
- Practice-specific access controls
- Personal information must be appropriately masked

Out of Scope:
- UI design for search interface
- Advanced search algorithms
- Export functionality
- Profile comparison features
- Real-time updates

Traceability:
- Source FR: FR#CPM-2 (FR#CPM-2 – Retrieve Candidate Profiles.md)