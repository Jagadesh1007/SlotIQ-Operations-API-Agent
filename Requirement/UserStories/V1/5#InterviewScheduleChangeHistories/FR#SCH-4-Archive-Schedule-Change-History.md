FR#SCH-4 - Archive Interview Schedule Change History

Title: Archive old interview schedule change history records

Description:
As a TA Team Admin, I want the system to archive old schedule change history records within my assigned practices, so that only relevant and recent history is retained for compliance and reporting.

Business Scope:
- Automatically archive history records older than retention period
- Maintain audit trail of archival actions
- Ensure only authorized users can view archived records
- Support compliance and data retention policies

Acceptance Criteria:
- Given a history record exceeds retention period
  When the system processes archival
  Then the record is archived and marked accordingly

- Given a TA Team Admin
  When viewing archived history
  Then only records from assigned practices are accessible

- Given a Master Admin
  When viewing archived history
  Then all records are accessible

- Given any authorized user
  When searching for archived history by interview or date
  Then matching records are displayed

Business Rules & Constraints:
- Archival must be based on retention period
- Only authorized users can view archived records
- Audit fields must be maintained
- Practice-specific access controls

Out of Scope:
- UI design for archival display
- Data export functionality
- Notification system
- Manual archival actions

Traceability:
- Source FR: FR#SCH-4 (FR#SCH-4 – Archive Schedule Change History.md)