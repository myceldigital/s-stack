# Comms-Stack

**An AI-native communications operating system for Stripe Ireland.**

`Comms-Stack` is a serious operating scaffold for a high-judgment communications lead who needs the leverage of a compact team without outsourcing editorial judgment to automation.

This repo is built around one principle:

**AI prepares. Humans decide.**

It is not a chatbot. It is not a press-release generator. It is a structured system for:

- daily market and media sensing
- stakeholder preparation
- campaign design and execution support
- founder-story packaging
- data-franchise development
- local-global coordination
- crisis readiness
- institutional memory compounding

## Why this exists

Communications work in Ireland is dense with context, timing, relationships, and political nuance. Too much of that usually lives in inboxes, ad hoc notes, and people's heads.

`Comms-Stack` externalizes that operating intelligence into a repo-native system made of:

- a persistent `knowledge/` layer
- reusable `templates/`
- specialist project-local skills in `.cursor/skills/`
- explicit operating rules in `CLAUDE.md`
- a full design spec in `SYSTEM_SPEC.md`

The repo is designed so a strong operator can move faster, stay sharper, and leave behind a system that compounds rather than disappearing with them.

## Core ideas

1. **The agents are the interface. The knowledge layer is the moat.**
2. **Preparation is more valuable than pseudo-autonomous output.**
3. **The best comms system improves judgment instead of replacing it.**
4. **Small-market relationship intelligence is strategic infrastructure.**

## Active command set

### Daily heartbeat
- `/landscape` — daily market, media, competitor, and policy briefing
- `/brief` — one-page stakeholder preparation pack
- `/rolodex` — relationship memory update after meaningful interactions

### Campaign surge
- `/narrative` — argument stack and thesis design
- `/angles` — audience- and outlet-specific hooks
- `/draft` — working drafts aligned to voice memory
- `/campaign` — sequencing, assets, approvals, and dependencies
- `/data` — aggregate-data franchise and evidence packaging
- `/founder-voice` — founder-story pipeline and prep
- `/linkedin` — executive and amplification posts in the right voice
- `/monitor` — post-launch pull-through and correction tracking
- `/retro` — system-improving retrospectives

### Coordination
- `/sync` — SF-Dublin timing, translation, and escalation support
- `/policy` — comms-relevant Irish and EU policy interpretation
- `/internal` — employee-facing translation of external moments and incidents

### Emergency
- `/warroom` — crisis structure, holding posture options, and stakeholder maps

## Repo structure

```text
.
├── .cursor/skills/        # project-local skills for all active agents
├── knowledge/             # narrative, relationship, policy, crisis, and editorial memory
├── templates/             # reusable output templates and YAML record shells
├── docs/                  # shared operating guidance
├── CLAUDE.md              # repo-local agent operating rules
├── SYSTEM_SPEC.md         # canonical design specification
├── PROJECT_TECHNICAL_OVERVIEW.md
├── CHANGES.md
└── workflow_state.md
```

## How to use it

### 1. Learn the architecture
Read:
- `SYSTEM_SPEC.md`
- `docs/OPERATING_MODEL.md`
- `CLAUDE.md`

### 2. Use the knowledge layer as the system of record
Start from:
- `knowledge/stripe-narrative.md`
- `knowledge/ireland-media-graph.md`
- `knowledge/policy-landscape.md`
- `knowledge/voice-memory.md`
- `knowledge/crisis-playbooks.md`

### 3. Run the system at two speeds
Daily heartbeat:
1. `/landscape`
2. `/brief`
3. `/rolodex`

Campaign surge:
1. `/narrative`
2. `/angles`
3. `/campaign`
4. `/draft`
5. `/brief`
6. `/linkedin`, `/founder-voice`, and/or `/data`
7. `/monitor`
8. `/retro`

### 4. Use the templates instead of improvising structure
Key templates:
- `templates/brief-template.md`
- `templates/campaign-template.md`
- `templates/incident-template.md`
- `templates/retro-template.md`
- `templates/data-report-template.md`

## Skill design

Each skill directory contains:
- `SKILL.md` — concise activation and workflow instructions
- `reference.md` — deeper strategic guidance, decision lenses, and failure modes

This keeps the main skill discoverable and tight while preserving enough depth to operate well under pressure.

## Current maturity

This is a high-quality scaffold, not a finished product. It already includes:
- a complete system spec
- a seeded knowledge tree
- reusable templates
- 16 advanced project-local skills
- explicit operator rules for safe usage

What it does **not** include yet:
- live monitoring integrations
- automated data pipelines
- graph-backed relationship storage
- production orchestration

## Operating boundary

This repo is intentionally strict about one thing:

**No outbound autonomy.**

AI can analyze, prepare, compare, package, and draft. Human operators retain the final call on outreach, publication, quotes, crisis posture, and sensitive messaging.
