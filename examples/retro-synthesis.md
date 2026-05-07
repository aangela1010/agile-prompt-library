# Retro Synthesis Example

## Raw Notes

Start:
- Doing mid-sprint check-ins on blockers instead of waiting for standup
- Tagging QA earlier when tickets are close to done
- Using the shared Slack channel for cross-team questions instead of DMs

Stop:
- Pulling in new work mid-sprint without team discussion
- Letting review cycles sit for more than a day without a nudge
- Scheduling meetings during the last two days of sprint

Continue:
- The Friday async update format, team likes it
- Pairing on complex tickets
- Keeping retro to 45 minutes

Action items:
- Team agrees on a no-new-work-mid-sprint norm, owned by the SM
- QA to be tagged when ticket hits code review, owned by devs
- Nudge protocol for stale reviews, owned by the SM

```## Prompt

You are an experienced Scrum Master synthesizing notes from a sprint
retrospective. Your job is to turn raw input into two clean outputs.

Team name or context: Team Orion, Notifications Service
Sprint number or date: Sprint 24
Retro format used: Start Stop Continue

Raw notes: [as above]

Note: This prompt produces two outputs. Do not skip the Slack summary.
```

## Output

### Confluence Summary

**Sprint:** 24
**Format:** Start Stop Continue

**What went well:**
The team identified several process improvements worth adopting. Mid-sprint
blocker check-ins were flagged as a higher-value touchpoint than waiting for
standup, and earlier QA involvement as tickets near completion was seen as
a way to reduce late-cycle rework. The team also recognized the value of
centralizing cross-team communication in shared Slack channels rather than
fragmented DMs.

**What could improve:**
Mid-sprint scope additions without team discussion were identified as a
recurring source of friction. Stale review cycles and meetings scheduled
in the final two days of sprint were also called out as drag on focus and
throughput.

**What to protect:**
The Friday async update format has team buy-in and should be preserved.
Pairing on complex tickets and maintaining a 45-minute retro cadence were
both flagged as worth protecting.

**Action Items:**

| # | Action | Owner | Tag |
|---|--------|-------|-----|
| 1 | Establish a no-new-work-mid-sprint norm | SM | Norm |
| 2 | Tag QA when ticket hits code review | Devs | Process |
| 3 | Build a nudge protocol for stale reviews | SM | Protocol |

### Slack Summary

🌟 Sprint 24 retro is a wrap — thanks everyone for a good conversation.

Things we are adding:
- Mid-sprint blocker check-ins
- Earlier QA tagging as tickets near done
- Shared Slack channel for cross-team questions

Things we are dropping:
- Mid-sprint scope additions without discussion
- Letting reviews go stale
- Meetings in the last two days of sprint

Keeping what is working:
- Friday async updates
- Pairing on complex tickets
- 45-minute retros

Action items:
- No-new-work-mid-sprint norm (SM to own)
- QA tagged at code review (devs to own)
- Nudge protocol for stale reviews (SM to own)

Shout if anything looks off.

## Notes

Prompt required explicit follow-up instruction to produce the Slack summary.
A reminder line has been added to the prompt: "This prompt produces two outputs.
Do not skip the Slack summary."

Output added a formatted action item table unprompted, which improved on the
numbered list specified in the prompt. No editing required on either output.
