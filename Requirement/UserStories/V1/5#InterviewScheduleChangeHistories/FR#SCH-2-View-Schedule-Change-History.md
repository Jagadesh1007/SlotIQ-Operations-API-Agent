FR#SCH-2 - View Interview Schedule Change History

Title: View and search history of interview schedule changes

Description:
As a TA Team Admin, I want to view and search the history of interview schedule changes within my assigned practices, so that I can monitor all modifications and ensure compliance.

Business Scope:
- View list of schedule change history records
- Filter history by interview, date, and type
- Access details of each change
- Track status and reason for changes
- Support audit and reporting needs

Acceptance Criteria:
- Given a TA Team Admin
  When viewing schedule change history
  Then only records from assigned practices are displayed

- Given a Master Admin
  When viewing schedule change history
  Then all records are displayed

- Given any authorized user
  When applying filters (interview, date, type)
  Then only matching records are displayed

- Given any user
  When providing invalid filter criteria
  Then appropriate error message is displayed

Business Rules & Constraints:
- History must be filterable by interview, date, and type
- Only authorized users can view history
- Audit fields must be maintained
- Practice-specific access controls

Out of Scope:
- UI design for history search
- Data export functionality
- Notification system
- Manual history record creation

Traceability:
- Source FR: FR#SCH-2 (FR#SCH-2 – Retrieve Schedule Change History.md)