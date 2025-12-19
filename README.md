# agentic-story-illustrator
A multi-agent creative production pipeline used to generate illustrations for books.

## Project Goal

This project explores how multi-agent systems can be used to add supplemental
illustrations to classic novels. The focus is on learning, transparency, and
reproducibility — not building a production system.

Agents are treated as specialized transformations that produce structured
artifacts (JSON) rather than free-form text.

## Repository layout

- `agents/` — agent prompts/roles and agent-specific docs.
- `schemas/` — JSON Schemas that define the structured inputs/outputs used by agents.
- `stories/` — story artifacts (inputs, outputs, drafts).
- `notes/` — working notes and learnings.

