# StakeHolder Update Example
---
## Raw Notes

Team: Team Orion, Notifications Service
Sprint: Sprint 25, just wrapped
Sprint goal: Ship the email retry logic and complete the migration of legacy notification templates to the new service
Completed work:

- Email retry logic shipped to production
- 8 of 11 legacy notification templates migrated
- Bug fix for duplicate push notifications affecting mobile users
- Updated internal API documentation for the notifications endpoint

Incomplete work:

- 3 remaining legacy templates, deprioritized mid-sprint when the duplicate push notification bug came in and required unplanned attention

Deployments:

- Email retry logic to production on day 8 of sprint
- Push notification bug fix to production on day 10

Carry-over:

- 3 remaining templates rolling into Sprint 26, on track to complete in first half of sprint

SM notes:

- Team handled the unplanned bug work well without derailing the sprint goal
- The email retry logic was a dependency for the payments team, glad it shipped
- Template migration is tedious work, team has been heads down on it for two sprints
---

## Prompt
Use the pasted notes to identify key themes, decisions, and action items. Produce a structured summary suitable for Confluence, email or Slack. 
Audience: Scrum Masters, support, and engineering leadership. 
[Raw Notes pasted at this point in the prompt]


## Output
Team Orion | Notifications Service | Sprint 25 Retrospective Summary

Sprint Goal
Ship the email retry logic and complete the migration of legacy notification templates to the new service.
Outcome: Partially Met
The sprint goal was split across two distinct workstreams. The email retry logic shipped successfully. Template migration reached 8 of 11, with 3 remaining templates carrying into Sprint 26 due to an unplanned bug that required mid-sprint attention.

What Shipped
The email retry logic went to production on day 8, completing a dependency that the payments team was waiting on. A duplicate push notification bug affecting mobile users was identified and resolved, with a fix deployed on day 10. Internal API documentation for the notifications endpoint was also updated. Eight of the eleven legacy notification templates were successfully migrated to the new service.

What Carried Over
Three legacy templates did not make it into the sprint. When the push notification bug came in, the team made a deliberate call to deprioritize the remaining templates in order to address user-facing impact. Those three templates are rolling into Sprint 26 and are expected to complete in the first half of the sprint.

Deployments
ReleaseDateEmail retry logicSprint Day 8Push notification bug fixSprint Day 10

SM Notes
The team absorbed a meaningful unplanned interruption without losing the primary sprint goal. The email retry delivery was time-sensitive given the payments team dependency, and the team delivered it on schedule. The template migration work has been steady and heads-down across two sprints now. Worth acknowledging that this is unglamorous, detail-heavy work and the team has stayed consistent through it.

Looking Ahead: Sprint 26
Carry-in: 3 legacy notification templates (target: complete in first half of sprint)

## Notes

Claude asked clarifying questions. Edit the initial prompt with more specifics stated.
