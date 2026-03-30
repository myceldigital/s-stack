## Project Technical Overview

`Comms-Stack` is an AI-native communications operating system scaffold tailored to Stripe Ireland's communications function.

### Purpose

The project now combines a full system design with an implementation-oriented repository scaffold for specialist-agent workflows, durable knowledge, reusable templates, and project-local skills.

### Primary Deliverable

- `SYSTEM_SPEC.md` — full internal-design-doc-style specification covering goals, architecture, agent roster, knowledge layer, schemas, workflows, prompts, operating rules, risk controls, and rollout strategy.

### Scaffold Contents

- `README.md` — top-level operating overview and command map
- `CLAUDE.md` — repo-local agent instructions for using the system safely and consistently
- `docs/OPERATING_MODEL.md` — two-speed operating model and workflow doctrine
- `knowledge/` — seeded memory files for narrative, relationships, policy, editorial voice, crisis playbooks, and archives
- `templates/` — reusable templates for briefs, campaigns, incidents, retros, data work, and structured sidecars
- `.cursor/skills/` — 16 project-local skill definitions matching the active agent roster

### Core System Shape

- 16 active agents grouped into daily heartbeat, campaign surge, coordination, and emergency layers.
- A two-speed operating model:
  - daily heartbeat for landscape awareness, stakeholder preparation, and relationship memory
  - campaign surges for launches, data franchises, partner storytelling, and amplification
- A compounding knowledge layer that stores narrative, relationship, editorial, policy, and operational memory.
- Markdown-first storage with optional YAML sidecars for structured records.

### Key Architectural Decisions

- AI prepares; humans decide and publish.
- Knowledge files are the system of record.
- `voice-memory.md` is a first-class editorial asset.
- `rolodex` evolves toward a relationship graph, not a flat contact list.
- `pitch` is not a standalone agent; it becomes a preparation mode inside briefing and campaign flows.

### Intended Audience

- Communications leaders
- Chief of staff / strategic ops leaders
- AI systems designers
- Internal tooling teams who may later implement the system

### Build And Runtime Notes

- This project currently contains a scaffolded operating repository, not a runnable application service.
- The repo is designed to be directly usable inside Cursor through project-local skills in `.cursor/skills/`.
- Sensitive outbound actions remain human gated by design.

### Verification Notes

- A valid scaffold includes coherent seed knowledge, reusable templates, and skill definitions aligned to the canonical system specification.
- Representative files should be read back after major updates and checked with editor diagnostics.
