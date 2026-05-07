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

### Prompts

- `prompts/retro-synthesis.md` — Synthesize raw retrospective input into a
  structured Confluence summary and Slack follow-up
- `prompts/stakeholder-update.md` — Draft a concise, VP-ready sprint status
  update from raw sprint data
- `prompts/blocker-triage.md` — Analyze a blocker and generate a structured
  options and escalation recommendation
- `prompts/ticket-quality-review.md` — Review a user story for acceptance
  criteria gaps and definition of ready alignment
- `prompts/dependency-risk.md` — Identify and articulate cross-team dependency
  risks for planning conversations

### Examples

The `examples` folder contains end-to-end examples for each prompt showing
realistic input and the AI output it produced, along with notes on what worked
and what needed adjustment. Use these to understand what good output looks like
before running a prompt against your own data.

## How to use it

Each prompt file contains a template with placeholders in brackets. Copy the
prompt, replace the placeholders with your actual content, and paste it into
your AI tool of choice. Output will typically need light editing for tone or
context but should be usable as a strong first draft.

An `example-template.md` file is included in the examples folder if you want
to contribute a new example or document your own results.

These prompts were developed and tested using Claude (Anthropic).

## Notes

This is a living document. Prompts are updated as they are tested against real
delivery scenarios and refined for output quality. Commit history reflects
changes and the reasoning behind them.
