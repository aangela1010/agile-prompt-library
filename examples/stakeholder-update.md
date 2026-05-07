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

``` ## Prompt
Use the pasted notes to identify key themes, decisions, and action items. Produce a structured summary suitable for Confluence, email or Slack. 
Audience: Scrum Masters, support, and engineering leadership. 
[Raw Notes pasted at this point in the prompt]


## Output
# Team Orion | Sprint 25 Retrospective Summary
**Service:** Notifications Service
**Sprint Goal:** Ship email retry logic and complete migration of legacy notification templates to the new service

---

## Sprint Outcome: Goal Partially Met

The sprint goal was partially achieved. The email retry logic shipped to production, satisfying the primary deliverable and unblocking a downstream dependency for the payments team. Template migration fell short of completion due to unplanned bug work, with 3 of 11 templates carrying over to Sprint 26.

---

## Completed Work

- Email retry logic deployed to production (Day 8)
- 8 of 11 legacy notification templates migrated to the new service
- Bug fix for duplicate push notifications affecting mobile users deployed to production (Day 10)
- Internal API documentation updated for the notifications endpoint

---

## Incomplete Work

| Item | Reason | Status |
|---|---|---|
| 3 remaining legacy notification templates | Deprioritized mid-sprint to address unplanned push notification bug | Carrying into Sprint 26 |

---

## Deployments

| Deployment | Environment | Day |
|---|---|---|
| Email retry logic | Production | Day 8 |
| Push notification bug fix | Production | Day 10 |

---

## Carry-Over: Sprint 26

The 3 remaining templates are scoped for the first half of Sprint 26 and are on track to complete within that window. No architectural changes are expected; this is continuation work.

---

## SM Notes

The team absorbed unplanned bug work cleanly without losing the sprint goal. The duplicate push notification issue required immediate attention given its impact on mobile users, and the team reprioritized well.

The email retry logic was a cross-team dependency for payments; getting that out on Day 8 was the right call and kept downstream work unblocked.

Worth flagging for Sprint 26 planning: the template migration has now stretched across two sprints. The work itself is not at risk, but it is tedious and the team has been heads down on it for a while. Consider whether there is room to vary the workload or acknowledge the effort in the sprint review.

---

*Summary prepared post-Sprint 25 | Team Orion | Notifications Service*
```

## Notes

Claude asked clarifying questions. Edit the initial prompt with more specifics stated.
Formatting issues from direct paste of output: explicity asked for a .md compatible format (for example file) 
