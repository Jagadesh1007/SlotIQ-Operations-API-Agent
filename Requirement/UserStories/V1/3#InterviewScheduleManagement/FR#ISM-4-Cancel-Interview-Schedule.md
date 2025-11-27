FR#ISM-4 - Cancel Interview Schedule

Title: Cancel scheduled interviews when needed

Description:
As a TA Team Admin, I want to cancel interview schedules within my assigned practices, so that I can manage scheduling conflicts and candidate withdrawals effectively.

Business Scope:
- Cancel upcoming interviews
- Record cancellation reasons
- Notify all participants
- Remove calendar invites
- Track cancellation history
- Free up panel member time slots

Acceptance Criteria:
- Given a TA Team Admin
  When canceling an interview in their practice
  Then the schedule is cancelled and all participants notified

- Given a Master Admin
  When canceling any interview schedule
  Then the schedule is cancelled successfully

- Given a TA Team Admin
  When attempting to cancel an interview outside their practice
  Then the request is rejected with appropriate error

- Given any authorized user
  When canceling without providing a reason
  Then the request is rejected with validation message

- Given any authorized user
  When canceling a completed interview
  Then the request is rejected with appropriate message

- Given any authorized user
  When canceling a past interview
  Then the request is rejected with appropriate message

Business Rules & Constraints:
- Cancellation reason is mandatory
- Cannot cancel completed interviews
- Cannot cancel past interviews
- All participants must be notified
- Calendar invites must be removed
- Time slots must be freed
- Cancellation history must be maintained

Out of Scope:
- UI design for cancellation
- Calendar system integration
- Email template design
- Notification mechanism
- Rescheduling process

Traceability:
- Source FR: FR#ISM-4 (FR#ISM-4 – Cancel Interview Schedule.md)