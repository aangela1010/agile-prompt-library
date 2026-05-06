# Agile Prompt Library

A curated collection of AI prompts for Scrum Masters and Agile delivery leads,
built to reduce the manual overhead of recurring facilitation and communication tasks.

## Why this exists

Agile ceremonies and delivery workflows generate a lot of repetitive writing and
synthesis work: retrospective summaries, stakeholder updates, blocker write-ups,
ticket quality checks. Most of that work follows predictable patterns, which makes
it a good candidate for AI-assisted automation.

This library is the result of identifying those patterns in real delivery contexts
and building prompts that produce reliable, high-quality output with minimal
editing. The goal is not to replace judgment but to get to a strong first draft
faster, so the time spent on delivery work goes toward thinking, not formatting.

## What is in here

- `prompts/retro-synthesis.md` — Synthesize raw retrospective input into a
  structured summary with themes and action items
- `prompts/stakeholder-update.md` — Draft a concise, VP-ready sprint status
  update from raw sprint data
- `prompts/blocker-triage.md` — Analyze a blocker and generate a structured
  options and escalation recommendation
- `prompts/ticket-quality-review.md` — Review a user story for acceptance
  criteria gaps and definition of ready alignment
- `prompts/dependency-risk.md` — Identify and articulate cross-team dependency
  risks for planning conversations

## How to use it

Each file contains a prompt template with placeholders in brackets. Copy the
prompt, replace the placeholders with your actual content, and paste it into
your AI tool of choice. Output will typically need light editing for tone or
context but should be usable as a strong first draft.

These prompts were developed and tested using Claude (Anthropic).

## Notes

This is a living document. Prompts are updated as they are tested against real
delivery scenarios and refined for output quality.
