# Comms-Stack

`Comms-Stack` is an AI-native communications operating system scaffold for Stripe Ireland.

This repository is designed for one high-judgment communications lead operating with the leverage of a specialist team. The system is Markdown-first, memory-centric, and explicitly built around the rule that AI prepares and humans decide.

## What is in this repo

- `SYSTEM_SPEC.md` - canonical system design
- `CLAUDE.md` - agent operating instructions for working inside the repo
- `knowledge/` - persistent narrative, relationship, editorial, policy, and operational memory
- `templates/` - reusable output shapes for briefs, campaigns, incidents, retros, and data work
- `.cursor/skills/` - project-local agent skills for the 16 active commands
- `docs/` - operator-facing guidance for running the system well

## Active command set

### Daily heartbeat
- `/landscape`
- `/brief`
- `/rolodex`

### Campaign surge
- `/narrative`
- `/angles`
- `/draft`
- `/campaign`
- `/data`
- `/founder-voice`
- `/linkedin`
- `/monitor`
- `/retro`

### Coordination
- `/sync`
- `/policy`
- `/internal`

### Emergency
- `/warroom`

## Operating doctrine

1. The knowledge layer is the system of record.
2. Outbound words remain human-owned.
3. Every meaningful interaction should improve memory.
4. Skills must produce decision-useful outputs, not generic prose.
5. If evidence is weak, say so plainly.

## Getting started

1. Read `SYSTEM_SPEC.md` for the full architecture.
2. Read `docs/OPERATING_MODEL.md` for the two-speed operating model.
3. Read `CLAUDE.md` so agents use the repo correctly.
4. Use the seeded files in `knowledge/` as the system of record.
5. Use the templates in `templates/` instead of inventing ad hoc output shapes.
