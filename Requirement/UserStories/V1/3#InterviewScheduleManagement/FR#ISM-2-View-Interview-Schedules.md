FR#ISM-2 - View Interview Schedules

Title: View and track interview schedules with filtering options

Description:
As a TA Team Admin, I want to view and search interview schedules within my assigned practices, so that I can monitor and manage the interview process effectively.

Business Scope:
- View list of interview schedules with pagination
- Filter by date range and status
- Search by candidate or panel member
- Track interview status
- Monitor schedule conflicts
- View schedule details

Acceptance Criteria:
- Given a TA Team Admin
  When viewing interview schedules
  Then only schedules from assigned practices are displayed

- Given a Master Admin
  When viewing interview schedules
  Then schedules from all practices are displayed

- Given any authorized user
  When filtering by date range
  Then only schedules within that range are shown

- Given any authorized user
  When searching by panel member
  Then only their scheduled interviews are shown

- Given any authorized user
  When filtering by interview status
  Then only matching schedules are displayed

- Given any user
  When providing invalid search criteria
  Then appropriate error message is displayed

Business Rules & Constraints:
- Default to current week's schedule
- Maximum date range of 3 months
- Default page size is 10 schedules
- Maximum page size is 50 schedules
- Sort by date/time by default
- Practice-specific access controls
- Show only active schedules by default

Out of Scope:
- UI design for schedule view
- Calendar view implementation
- Export functionality
- Real-time updates
- Analytics features

Traceability:
- Source FR: FR#ISM-2 (FR#ISM-2 – Retrieve Interview Schedules.md)