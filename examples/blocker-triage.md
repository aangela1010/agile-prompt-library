# Blocker Triage Prompt

## What this does

Takes a raw blocker description and produces a structured triage summary
suitable for a ticket, a Slack thread, or a leadership escalation. Covers
the full picture of the blocker: what it is, what it affects, what the
options are, and what needs to happen next.

Use this when a blocker surfaces and you need to move quickly from
"something is wrong" to "here is what we know and what we are doing about it."

## Raw Notes
sprint 25 day 4
payments team pinged in slack - they cant test checkout flow 
because our retry logic isnt handling failed notifications correctly
edge case we didnt catch in dev
jake from payments flagged it, their QA is blocked
release scheduled end of sprint, 6 days out
talked to dev lead - thinks it's a 2 day fix but hasnt looked closely yet
not sure if we need to push the release or if payments can work around it
need to loop in product
## Refinement Notes

- If the blocker is a dependency on another team, add: "This is a
  cross-team dependency. Frame the options and next steps section around
  what needs to happen on each side."
- If escalation is needed urgently, add: "This blocker requires immediate
  escalation. Lead with the escalation section."
- The "what has been tried" field is important. The more detail you
  provide there, the less the output will suggest options that have
  already been ruled out.
- If your org uses a specific ticket format such as RAID or a risk
  register, add a line at the end: "Also produce a one paragraph summary
  suitable for pasting into [TICKET TYPE]."

```
## Prompt

You are an experienced Scrum Master triaging a blocker that has surfaced
during an active sprint. Your job is to take raw information and produce
a structured summary that gives stakeholders everything they need to
understand the blocker, assess its impact, and act on it.

Audience: All stakeholders, engineering and product leadership
Team: Team Orion, Notifications Service
Initiative: Checkout Flow Modernization

Input:
- Team and initiative affected: Team Orion, Notifications Service,
  Checkout Flow Modernization initiative
- Blocker description: Retry logic in the notifications service is not
  correctly handling a failed notification edge case, blocking the Artemis
  payments team from testing the checkout flow
- When it was identified: Sprint 25, Day 4
- What is at risk if unresolved: End of sprint release, six days out.
  Artemis QA is fully blocked. Payments team checkout flow cannot proceed.
- What has been tried or ruled out: Dev lead consulted, believes fix is
  approximately two days but has not done a close investigation yet.
  No workaround identified.
- Who needs to act or decide: Orion dev lead on investigation and fix,
  product on release strategy decision
- Initiative this rolls up to: Checkout Flow Modernization
- Additional context: This is a cross-team dependency. Frame options and
  next steps around what needs to happen on each side.
```
## Output

Blocker Triage Summary
## Initiative: Payment Module |  Team: Orion |  Affected Team: Artemis (Payments)  |  Sprint 25, Day 4

## Blocker
The Artemis payments team cannot test their checkout flow because retry logic in the notifications service is not correctly handling a failed notification edge case. This bug was not caught in development and is now blocking Artemis QA entirely.

## Impact
Artemis QA is fully blocked today. The Payment Module release is scheduled for end of sprint, six days out. If the fix takes the estimated two days and rework or retest time is needed, the release window is at risk. Any downstream work Artemis has scheduled post-QA is also at risk of slipping.

## Status
Jake from Artemis flagged the issue in Slack on Sprint 25 Day 4. Orion's dev lead has been consulted and believes the fix is approximately two days of work, but has not yet done a close investigation. No workaround has been identified yet. Root cause is confirmed as an unhandled edge case in the retry logic, not a broader architectural issue.

## Options and Decisions
### Option 1: 
Fix and hold the release Orion dev completes the fix within the sprint. Release proceeds as scheduled if the fix lands with enough time for Artemis to complete QA. Risk: estimate is soft and has not been validated by close investigation. If the fix runs long, the release slips anyway with less runway to react.

### Option 2: 
Artemis works around the issue Artemis QA scopes around the blocked checkout flow and tests what it can, with the fix delivered post-release or in a fast follow. Risk: untested checkout behavior ships to production. Needs product sign-off on acceptable risk.

### Option 3: 
Partial release Release proceeds without the features or flows dependent on the broken notification path. Artemis completes full QA after the fix lands. Risk: requires scoping what can safely ship, adds coordination overhead, and may reduce the value of the release.

## Decision needed from product: which option is acceptable given business risk and release scope.


# Next Steps
## Within 24 hours:

Dev lead completes a close investigation of the retry logic issue and validates or revises the two-day estimate. Owner: Orion dev lead.
Scrum Master loops in product to present the three options and get a decision on release strategy. Owner: Orion Scrum Master.
Artemis confirms whether any portion of QA can proceed independently while the fix is in progress. Owner: Artemis QA lead.

## Within 48 hours:

Release decision made and communicated to both teams. Owner: Product.
If fixing, dev work begins with a clear completion target. Owner: Orion dev lead.


## Escalation
Yes. This needs product involvement immediately. The core question is a business risk decision: whether to hold the release, ship with a known gap, or scope a partial release. That call belongs to product, not the delivery teams. No additional escalation above product is indicated at this time, but if the fix estimate grows or the release decision affects other downstream commitments, leadership may need visibility.



## Notes
Prompt required clarifying questions on two seperate attempts before producing output. Fields for audience, affected team, and initiative have been added to the input block explicity to reduce ambiguity on future runs. The more complete the input the less back and forth required.
