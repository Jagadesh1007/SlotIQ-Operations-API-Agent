FR#IRM-2 - View Interview Reschedule Requests

Title: View and track interview reschedule requests

Description:
As a TA Team Admin, I want to view and track reschedule requests for interviews within my assigned practices, so that I can monitor the status and outcomes of all rescheduling activities.

Business Scope:
- View list of reschedule requests with filtering options
- Track status and history of requests
- Filter by date, status, and interview
- Access details of each request
- Monitor approval and completion

Acceptance Criteria:
- Given a TA Team Admin
  When viewing reschedule requests
  Then only requests from assigned practices are displayed

- Given a Master Admin
  When viewing reschedule requests
  Then requests from all practices are displayed

- Given any authorized user
  When applying filters (date, status, interview)
  Then only matching requests are displayed

- Given any user
  When providing invalid filter criteria
  Then appropriate error message is displayed

Business Rules & Constraints:
- Requests must be filterable by date, status, and interview
- Only active requests are shown by default
- Practice-specific access controls must be enforced
- Status and history must be visible

Out of Scope:
- UI design for request tracking
- Notification system
- Approval workflow implementation
- Export functionality

Traceability:
- Source FR: FR#IRM-2 (FR#IRM-2 – Retrieve Interview Reschedule Requests.md)