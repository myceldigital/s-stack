## Changes

- Initialized the `Comms-Stack/` project root for a Stripe-style communications operating system specification.
- Added project-level overview and workflow state so the project is self-describing from its own root.
- Authored `SYSTEM_SPEC.md` as the canonical design artifact covering architecture, schemas, workflows, prompts, and operating rules.
- Recorded the system's key design choice that AI handles preparation and analysis while humans retain final editorial and outbound control.
- Added a full repo scaffold with `README.md`, `docs/OPERATING_MODEL.md`, a seeded `knowledge/` tree, and reusable `templates/`.
- Added 16 project-local skills under `.cursor/skills/`, one for each active agent in the system, with explicit workflow, output, escalation, and memory-update contracts.
- Added `CLAUDE.md` and `.gitignore` so the repo has explicit agent operating rules and clean git hygiene before publishing.
- Initialized git in the project root, preserved the remote `LICENSE`, pushed the folder contents to `myceldigital/s-stack`, and updated the GitHub repo description.
