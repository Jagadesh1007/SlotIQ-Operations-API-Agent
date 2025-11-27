FR#ISM-1 - Schedule New Interview

Title: Schedule technical interviews for candidates

Description:
As a TA Team Admin, I want to schedule technical interviews for candidates within my assigned practices, so that I can coordinate interview sessions between candidates and panel members.

Business Scope:
- Create new interview schedules
- Assign technical panel members
- Set interview date and time slots
- Link to candidate profiles
- Specify interview types
- Generate calendar invites
- Track interview status

Acceptance Criteria:
- Given a TA Team Admin
  When scheduling an interview with valid details
  Then the interview is scheduled and calendar invites are sent

- Given a Master Admin
  When scheduling an interview for any practice
  Then the interview is scheduled successfully

- Given any authorized user
  When scheduling with an unavailable panel member
  Then the request is rejected with appropriate message

- Given any authorized user
  When scheduling outside business hours
  Then the request is rejected with appropriate message

- Given any authorized user
  When scheduling with invalid time slots
  Then the request is rejected with validation message

- Given any authorized user
  When scheduling for an invalid candidate
  Then the request is rejected with appropriate error

Business Rules & Constraints:
- Interview title and notes are mandatory
- Panel member must be available for selected slot
- Time slot must be within business hours
- No overlapping interviews for same panel member
- Valid interview type must be selected
- Must be linked to active candidate profile
- Calendar invites must be generated

Out of Scope:
- UI design for scheduling interface
- Calendar integration details
- Email template design
- Room booking system
- Video conference setup

Traceability:
- Source FR: FR#ISM-1 (FR#ISM-1 – Schedule New Interview.md)