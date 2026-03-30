## Comms-Stack Operating Instructions

This repo is a Markdown-first communications operating system scaffold.

### Core rule

AI prepares. Humans decide.

Never imply final approval, send outbound messages automatically, or present speculative claims as confirmed fact.

### Source of truth

Before running a comms workflow, read the relevant files in `knowledge/`.

At minimum:

- `/landscape`: read `knowledge/stripe-narrative.md`, `knowledge/ireland-media-graph.md`, `knowledge/policy-landscape.md`, `knowledge/competitor-intelligence.md`
- `/brief`: read the relevant relationship records plus the active narrative or campaign context
- `/draft`: read `knowledge/style-guide.md` and `knowledge/voice-memory.md`
- `/warroom`: read `knowledge/crisis-playbooks.md` and any active sync or policy context

### Skill usage

Use the project-local skills in `.cursor/skills/` for the active command set:

- Daily heartbeat: `/landscape`, `/brief`, `/rolodex`
- Campaign surge: `/narrative`, `/angles`, `/draft`, `/campaign`, `/data`, `/founder-voice`, `/linkedin`, `/monitor`, `/retro`
- Coordination: `/sync`, `/policy`, `/internal`
- Emergency: `/warroom`

### Memory discipline

- Every significant interaction should result in a memory update through `/rolodex`, `/retro`, or the relevant archive file.
- If a human materially edits a draft, update `knowledge/voice-memory.md` with durable editorial patterns.
- If a campaign or incident finishes, archive the result and capture reusable lessons.

### Output discipline

- Prefer decision-useful outputs over generic prose.
- Mark unsupported claims as `UNVERIFIED`.
- Use files under `templates/` when producing structured outputs.
- Preserve the founder as protagonist in founder stories and keep Stripe as enabling infrastructure unless the task explicitly requires a Stripe-led message.
