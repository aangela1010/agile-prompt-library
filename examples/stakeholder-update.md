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
A few quick questions before I finalize anything:

Do you want this formatted as a written narrative (good for Confluence or a Slack post), a structured doc, or something else?
Is there a stakeholder audience I should calibrate for (e.g., leadership only, cross-team, just the team itself)?

In the meantime, here's a solid draft you can react to:

Team Orion | Notifications Service | Sprint 25 Review
Sprint 25 is wrapped, and the headline is: the sprint goal shipped.
Email retry logic is live in production, completing a dependency that the payments team had been waiting on. That one mattered beyond Orion, and the team delivered it on day 8 of the sprint. The push notification duplicate bug, which surfaced mid-sprint and was not planned work, got fixed and deployed by day 10 without derailing the goal. That kind of absorption capacity is worth noting.
On the template migration front, 8 of 11 legacy notification templates are now running on the new service. The remaining 3 were intentionally deprioritized when the bug work came in and will carry into Sprint 26. They are on track to wrap in the first half of the sprint. The team has been heads down on migration work for two sprints now, and the finish line is close.
Shipped to production
Email retry logic (day 8), push notification bug fix (day 10), API documentation update for the notifications endpoint.
Carrying into Sprint 26
3 remaining legacy notification templates, expected to complete early in the sprint.

Let me know if the tone is right, if you want the SM observations woven in more explicitly, or if there's a specific section you want expanded.

## Notes

Claude asked clarifying questions. Edit the initial prompt with more specifics stated.
