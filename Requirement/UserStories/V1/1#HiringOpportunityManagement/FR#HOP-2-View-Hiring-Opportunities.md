FR#HOP-2 - View Hiring Opportunities

Title: View and search hiring opportunities with filtering options

Description:
As a TA Team Admin, I want to view and search hiring opportunities within my assigned practices, so that I can track and manage recruitment needs effectively.

Business Scope:
- View list of hiring opportunities with pagination
- Filter opportunities by practice, category, and status
- Sort opportunities by different criteria
- Access detailed information about each opportunity
- Monitor recruitment progress

Acceptance Criteria:
- Given a TA Team Admin
  When viewing hiring opportunities
  Then only opportunities from assigned practices are displayed

- Given a Master Admin
  When viewing hiring opportunities
  Then opportunities from all practices are displayed

- Given any authorized user
  When applying filters (practice, category, status)
  Then only matching opportunities are displayed

- Given any authorized user
  When requesting a specific page size and number
  Then the correct page of results is returned

- Given any authorized user
  When sorting by any valid field
  Then results are ordered accordingly

- Given any user
  When providing invalid filter criteria
  Then appropriate error message is displayed

Business Rules & Constraints:
- Default page size is 10 items
- Maximum page size is 50 items
- Results must be filterable by practice, category, and status
- Sorting available by creation date, modified date, title
- Only active opportunities are displayed by default
- Practice-specific access controls must be enforced

Out of Scope:
- UI design for search interface
- Export functionality
- Advanced search capabilities
- Real-time updates

Traceability:
- Source FR: FR#HOP-2 (FR#HOP-2 – Retrieve Hiring Opportunities.md)