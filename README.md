Engineer can review the generated DDR before submission.
Approver selection is mandatory before DDR submission.
Only approvers belonging to the same Product Group are displayed.
The submitter cannot select themselves as an approver.
Successful submission transitions the DDR to the approval stage.
DDR approval notification emails are sent within 2 minutes of submission.
DDR rejection requires a mandatory non-blank comment.
Rejection comments are used as input for DDR regeneration.
Regenerated DDR reflects the rejection guidance provided.
All submission, approval, and rejection events are recorded in audit logs.


Functional
Engineer can reject the generated DDR before admin submission.
Rejection requires a mandatory non-blank comment.
Rejection comments are used as input for DDR regeneration.
A new version of the DDR is generated after rejection.
Regenerated DDR reflects the revision guidance provided.
Rejection reason is recorded in the State Database.
Appropriate error messages are displayed if regeneration fails.
Non-Functional
Rejection and state transition are processed atomically.
DDR regeneration activities are auditable and linked to the workflow ID.
Rejection events are logged with correlation IDs.
Version history of regenerated DDR documents is maintained.

Functional
Only assigned admin reviewers can approve the DDR.
Admin can approve the submitted DDR with an optional comment.
State DB is updated to DDR Approved upon successful approval.
Workflow progresses to the RELEASE_GENERATING stage after approval conditions are met.
Approval notification email is sent to the submitter within 1 minute.
UI reflects the approved status immediately after approval.
Approval actions are recorded in audit logs.
Non-Functional
Approval is enforced through server-side RBAC validation.
State update and notification are processed atomically.
Approval actions are idempotent and prevent duplicate processing.
All approval events are logged with correlation IDs for traceability.


Functional
Only assigned admin reviewers can reject the DDR.
Rejection requires a mandatory non-blank comment.
DDR status is updated to DDR_GENERATING after rejection.
Rejection comments are used as input for DDR regeneration.
The submitter receives an email containing the rejection reason and next steps.
The UI reflects the rejected status immediately.
Rejection actions are recorded in audit logs.
Non-Functional
Rejection is enforced through server-side RBAC validation.
State updates and notification events are processed atomically.
Rejection actions are idempotent and prevent duplicate processing.
All rejection events are logged with correlation IDs for traceability.
