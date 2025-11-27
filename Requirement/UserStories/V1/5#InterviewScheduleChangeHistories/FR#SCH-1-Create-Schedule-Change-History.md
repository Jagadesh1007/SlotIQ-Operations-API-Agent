FR#SCH-1 - Create Interview Schedule Change History

Title: Record history of interview schedule changes

Description:
As a TA Team Admin, I want the system to record all changes to interview schedules within my assigned practices, so that I can track modifications and maintain an audit trail.

Business Scope:
- Automatically record every change to interview schedules
- Link history records to original interviews and reschedule requests
- Track reason and status for each change
- Maintain complete audit trail
- Support compliance and reporting needs

Acceptance Criteria:
- Given a schedule change occurs
  When the change is processed
  Then a history record is created with all relevant details

- Given a TA Team Admin
  When viewing change history
  Then only records from assigned practices are accessible

- Given a Master Admin
  When viewing change history
  Then all records are accessible

- Given any authorized user
  When searching for history by interview or date
  Then matching records are displayed

Business Rules & Constraints:
- History must be linked to original interview and reschedule request
- Reason and status must be recorded
- Audit fields must be maintained
- Only authorized users can view history

Out of Scope:
- UI design for history display
- Notification system
- Data export functionality
- Manual history record creation

Traceability:
- Source FR: FR#SCH-1 (FR#SCH-1 – Create Interview Schedule Change History.md)