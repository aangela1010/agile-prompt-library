# Retro Synthesis Prompt

## What this does

Takes raw retrospective input (sticky notes, FigJam/whiteboard exports, or
bullet notes) and produces two outputs in one pass:

1. A structured summary formatted for a Confluence page
2. A short Slack message to share with the team after the session

Use this after any sprint retrospective where notes were captured in a
whiteboard tool or live doc and need to be cleaned up and distributed.

## The Prompt

You are an experienced Scrum Master synthesizing notes from a sprint
retrospective. Your job is to turn raw input into two clean outputs.

**Input:**
- Team name or context: [TEAM NAME / CONTEXT]
- Sprint number or date: [SPRINT # OR DATE RANGE]
- Raw retrospective notes: [PASTE NOTES HERE — sticky text, bullets, freeform]
- Retrospective format used: [e.g. Start Stop Continue, 4Ls, Mad Sad Glad]

**Output 1: Confluence Page Summary**

Produce a structured retrospective summary with the following sections:

- **Sprint:** [sprint number or date]
- **Format:** [retro format used]
- **What went well:** A synthesized summary of positive themes, not a raw list.
  Group similar items. Write in complete sentences.
- **What could improve:** A synthesized summary of friction or challenge themes.
  Group similar items. Write in complete sentences.
- **Action items:** A numbered list of specific, ownable actions that came out
  of the session. Each item should include what the action is and who owns it
  if that information is available.
- **Facilitator notes:** [Optional] Any patterns worth flagging for the next
  retro or for the team's attention over the coming sprint.

**Output 2: Slack Summary**

Write a brief, conversational Slack message (4 to 6 sentences) to send to the
team channel after the retro. It should:

- Acknowledge the session warmly without being performative
- Call out one or two key themes that came up
- List the action items clearly
- End with a forward-looking sentence about the next sprint

Tone should be direct and human, not corporate. Write it as if the Scrum
Master is speaking, not as a formal announcement.

## Refinement Notes

- If the raw notes are very sparse, add this line to the prompt: "Where input
  is thin, note that in the output rather than inventing themes."
- If the team uses a specific retro format consistently, hardcode it into your
  saved version of this prompt so you do not have to fill it in each time.
- The Slack message tone can be adjusted by adding: "The team communication
  style is [formal / casual / dry humor]" to the input block.
