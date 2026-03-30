# Comms-Stack System Specification

Status: Draft v1.0  
Owner: Communications Systems Design  
Audience: Communications, Policy, Internal Tools, Leadership  
Last updated: 2026-03-30

## 1. Overview

`Comms-Stack` is an AI-native communications operating system designed for Stripe Ireland. It enables a single high-judgment communications lead to operate with the leverage, memory, and preparation quality of a compact specialist team without delegating final editorial judgment to automation.

The system is not a generic writing assistant. It is a structured operating layer for:

- daily landscape awareness
- campaign design and execution support
- stakeholder preparation
- cross-geo coordination
- crisis response
- institutional memory compounding

The core design insight is simple:

**The agents are the interface. The knowledge layer is the moat.**

## 2. Problem Statement

Communications work in Ireland is high-context, relationship-dense, and timing-sensitive.

The current operating failure modes for a single comms lead are:

- too much context lives in heads, inboxes, and chat threads
- journalist, founder, and policy context is expensive to recall on demand
- global and local comms calendars collide without enough warning
- reactive issues require fast synthesis under uncertainty
- narrative quality depends on repeated manual reconstruction of arguments and proof points
- editorial voice is hard to preserve when AI drafts too much

The system must therefore increase preparation quality, reduce retrieval latency, and preserve trust.

## 3. Goals

### 3.1 Primary goals

1. Make the daily briefing indispensable.
2. Make every high-stakes interaction better prepared.
3. Turn campaign creation into a repeatable system, not heroic effort.
4. Produce faster and more reliable crisis handling.
5. Externalize institutional knowledge so a successor can ramp quickly.
6. Preserve human editorial and reputational judgment.

### 3.2 Success metrics

- Morning briefing adoption is near-daily on business days.
- Inbound press inquiries grow relative to outbound pitch volume.
- Time to first holding statement drops below 30 minutes in exercised scenarios.
- Edit distance on AI-assisted drafts declines over time via voice memory.
- Knowledge coverage expands across reporters, founders, campaigns, and risks.
- SF-Dublin comms conflicts trend toward zero.

## 4. Non-Goals

- Fully autonomous outbound media relations
- Autonomous publishing to public channels
- Replacing legal, policy, or government affairs review
- General-purpose social media scheduling
- Replacing CRM, calendar, or internal comms systems of record

## 5. Design Principles

1. **AI prepares; humans decide.**
2. **Preparation is higher leverage than generation.**
3. **Every output must improve memory.**
4. **Local context outranks generic best practice.**
5. **Small-market relationship intelligence is strategic infrastructure.**
6. **The system must be legible, inspectable, and Markdown-first.**

## 6. Operating Model

The system runs at two speeds.

### 6.1 Daily heartbeat

This is the every-day operating rhythm.

- `/landscape` in the morning
- `/brief` before meetings, media interactions, and events
- `/rolodex` after meaningful contacts
- `/sync` and `/policy` whenever background context changes

Questions answered:

- What changed?
- What matters today?
- Who do I need to understand before I engage?
- What timing or political conflicts are emerging?

### 6.2 Campaign surges

This is the episodic, multi-week rhythm around launches, reports, thematic pushes, and partner stories.

Canonical flow:

1. `/narrative`
2. `/angles`
3. `/campaign`
4. `/draft`
5. `/brief`
6. `/linkedin`, `/founder-voice`, and/or `/data`
7. `/monitor`
8. `/retro`

### 6.3 Emergency mode

When a high-risk signal appears, the system pivots into a war room flow:

1. `/landscape` flags anomaly
2. `/warroom` opens a structured incident file
3. `/brief` prepares stakeholder packets
4. `/draft` produces holding lines and support copy
5. `/sync` blocks cross-geo conflicts
6. `/internal` prepares employee messaging
7. `/monitor` tracks corrections and framing drift
8. `/retro` updates playbooks

## 7. Architecture

### 7.1 Logical layers

```text
Signals -> Analysis -> Preparation -> Human Judgment -> External Action -> Learning

Signals:
  media, LinkedIn, founders, competitors, policy, partner milestones, internal calendars

Analysis:
  landscape, policy, narrative, angles, warroom

Preparation:
  brief, draft, campaign, founder-voice, linkedin, internal, sync

Human Judgment:
  comms lead, leadership, policy/legal partners, cross-geo comms counterparts

External Action:
  calls, emails, interviews, internal posts, media launches, LinkedIn posts, reports

Learning:
  retro, rolodex, voice memory, campaign archive, playbooks
```

### 7.2 Active agent roster

#### Daily heartbeat

| Command | Role | Primary output |
|---|---|---|
| `/landscape` | Ecosystem scout | Morning brief, alerts, framing watch, competitor context |
| `/brief` | Stakeholder briefer | One-page prep packs, talking points, risk notes |
| `/rolodex` | Relationship manager | Relationship updates, interaction memory, graph notes |

#### Campaign surge

| Command | Role | Primary output |
|---|---|---|
| `/narrative` | Chief narrative architect | Argument stack and messaging hierarchy |
| `/angles` | Story angle generator | Audience and outlet angle matrix |
| `/draft` | Content engine | Draft materials aligned to voice memory |
| `/campaign` | Campaign architect | Sequencing, ownership, channel and dependency plan |
| `/data` | Franchise engine | Data-report packages and approved insight summaries |
| `/founder-voice` | Partner storytelling engine | Founder story assessments and prep packs |
| `/linkedin` | Professional network amplifier | LinkedIn drafts and amplification copy |
| `/monitor` | Post-deploy tracker | Coverage analysis, correction queue, resonance report |
| `/retro` | Learning engine | Retrospectives, changes to memory, system recommendations |

#### Coordination

| Command | Role | Primary output |
|---|---|---|
| `/sync` | SF-Dublin bridge | Calendar, translation, and escalation briefs |
| `/policy` | Government affairs advisor | Policy landscape brief and impact assessment |
| `/internal` | Employee comms bridge | Internal versions of external moments and crisis notes |

#### Emergency

| Command | Role | Primary output |
|---|---|---|
| `/warroom` | Crisis commander | Situation report, holding lines, stakeholder map |

### 7.3 Retired or transformed commands

- `/sentiment` -> absorbed into `/landscape`
- `/listen` -> absorbed into `/landscape` and `/founder-voice`
- `/event` -> absorbed into `/campaign`
- `/pitch` -> transformed into `pitch-pack` mode under `/brief` and campaign planning

## 8. Knowledge Layer

The knowledge layer is the system of record. It must remain durable, inspectable, and directly editable.

### 8.1 Top-level structure

```text
knowledge/
  stripe-narrative.md
  ireland-media-graph.md
  partner-tracker.md
  crisis-playbooks.md
  style-guide.md
  voice-memory.md
  policy-landscape.md
  competitor-intelligence.md
  founder-pipeline.md
  internal-comms-log.md
  weekly-retros/
  campaign-archive/
  source-ledger/
  sync-calendar/
```

### 8.2 Memory classes

1. **Narrative memory**  
What Stripe Ireland wants to stand for.

2. **Relationship memory**  
Who matters, what they care about, and how they connect.

3. **Editorial memory**  
How the comms lead edits, structures, and rejects language.

4. **Operational memory**  
What happened, what was done, and what should change next time.

### 8.3 Knowledge file contracts

#### `knowledge/stripe-narrative.md`

Required sections:

- current master framing
- supporting claims
- approved proof points
- known weak claims
- taboo phrases
- Ireland-specific localizers
- active campaign overlays

#### `knowledge/ireland-media-graph.md`

Required sections:

- reporter and outlet index
- beat mapping
- relationship quality
- recent contact history
- angle preferences
- avoidance notes
- cross-relationships of significance

#### `knowledge/voice-memory.md`

Required sections:

- author profile
- positive patterns
- negative patterns
- structural preferences
- vocabulary constraints
- edit-diff examples
- freshness timestamp

#### `knowledge/crisis-playbooks.md`

Required sections:

- scenario type
- initial stakeholder map
- first-hour questions
- holding posture variants
- escalation triggers
- internal comms delta
- post-event retro hooks

## 9. Data Schemas

The system is Markdown-first, with optional YAML or JSON sidecars where machine-readability improves orchestration or graph queries.

### 9.1 Reporter record schema

```yaml
id: rpt_irish_times_fintech_001
name: Jane Example
outlet: The Irish Times
beat:
  - fintech
  - Irish business
  - regulation
relationship_status: warm
last_contact_at: 2026-03-14
last_contact_summary: Discussed Q2 data report framing and timing.
preferences:
  likes:
    - founder-led stories
    - original data
    - local economic context
  avoids:
    - generic corporate framing
    - over-scripted quotes
angle_fit:
  payments_infrastructure: high
  SME_growth: high
  AI_policy: medium
risk_flags:
  - skeptical_of_headcount_claims
  - sensitive_to_large-tech-regulatory-spin
linked_entities:
  - ida_board_contact_004
  - angel_network_017
notes:
  - Asked if prior pitch was AI-written; prefer direct, human outreach.
source_refs:
  - knowledge/source-ledger/reporter-notes-2026-03.md
```

### 9.2 Founder story candidate schema

```yaml
id: fndr_story_023
company: Galway Goods
founder: Aisling Example
stripe_relationship: existing_customer
story_stage: candidate
story_strength: strong
media_readiness: medium
stripe_angle: international expansion enabled by payments infrastructure
proof_points:
  - revenue_growth_qoq
  - export_mix_increase
  - team_growth
timing:
  ideal_window_start: 2026-04-15
  ideal_window_end: 2026-05-10
outlet_fit:
  - Business Post
  - The Currency
  - regional_press
risks:
  - founder_has_never_done_broadcast
  - numbers_need_finance_confirmation
owner: ireland_comms
status_notes: Waiting on permission to cite growth numbers.
```

### 9.3 Crisis incident schema

```yaml
id: incident_2026_05_processor_breach
opened_at: 2026-05-12T07:18:00Z
status: active
severity: high
classification: third_party_security_event
known_facts:
  - Stripe systems unaffected
  - third-party processor incident confirmed
unknowns:
  - affected merchant count
  - exact data categories exposed
stakeholders:
  tier_1:
    - dpc
    - affected_merchants
    - ireland_gm
  tier_2:
    - ida
    - enterprise_ireland
    - sf_comms
holding_variants:
  - minimal
  - moderate
  - assertive
chosen_variant: moderate
decision_owner: ireland_comms_lead
sync_conflicts:
  - sf_security_blog_post_2026_05_12
postmortem_ref: knowledge/weekly-retros/week-20.md
```

### 9.4 Voice memory schema

```yaml
author_id: ireland_comms_lead
updated_at: 2026-03-30
patterns_to_prefer:
  - lead_with_human_impact
  - keep_paragraphs_short
  - use_one_crisp_number_per_section
patterns_to_avoid:
  - leverage
  - transformational
  - ecosystem_in_generic_form
structure_preferences:
  op_ed: vignette_vignette_argument_close
  briefing: context_implication_action
  internal_note: facts_first_then_reassurance
edit_examples:
  - before: "Stripe leverages..."
    after: "Stripe helps..."
```

### 9.5 Campaign record schema

```yaml
id: campaign_state_of_irish_commerce_q3_2026
type: franchise
objective: Establish Stripe as the most credible source on Ireland's digital economy.
owner: ireland_comms
status: live
start_date: 2026-08-20
target_audiences:
  - business_press
  - policymakers
  - founders
  - enterprise_prospects
primary_assets:
  - report
  - charts
  - executive_linkedin_post
  - journalist_briefs
approval_gates:
  - data_privacy_review
  - editorial_review
  - policy_review_if_needed
success_metrics:
  - tier_1_placements
  - inbound_inquiries
  - source_citation_rate
retro_ref: knowledge/campaign-archive/state-of-commerce-q3.md
```

## 10. Command Contracts

Each command has a stable contract: inputs, required reads, outputs, and memory updates.

### 10.1 `/landscape`

**Purpose**  
Produce the daily operating picture.

**Required reads**

- `knowledge/stripe-narrative.md`
- `knowledge/ireland-media-graph.md`
- `knowledge/policy-landscape.md`
- `knowledge/competitor-intelligence.md`

**Primary inputs**

- latest market signals
- monitoring feeds
- known upcoming events

**Primary outputs**

- morning brief
- top five developments
- framing watch
- competitive context
- reporter movement
- amber/red alerts

**Memory updates**

- append meaningful new entities to media graph or competitor intelligence

### 10.2 `/brief`

**Purpose**  
Prepare the human for an interaction.

**Modes**

- reporter
- founder
- executive
- policy
- partner
- pitch-pack

**Primary outputs**

- contact summary
- context and stakes
- recommended talking points
- likely objections
- do-not-say list
- timing and relationship note

**Memory updates**

- none during pre-brief
- post-interaction notes go through `/rolodex`

### 10.3 `/rolodex`

**Purpose**  
Update the relationship memory after each significant contact.

**Primary outputs**

- new contact note
- changed relationship score
- next suggested follow-up
- related-entity link suggestions

### 10.4 `/narrative`

**Purpose**  
Create or refine the argument stack behind a topic or campaign.

**Primary outputs**

- thesis
- three to five supporting arguments
- proof points
- likely attacks
- local Ireland angle

### 10.5 `/angles`

**Purpose**  
Turn a thesis into audience- and outlet-specific hooks.

**Primary outputs**

- outlet matrix
- protagonist choice
- timing rationale
- contrarian backup angle

### 10.6 `/draft`

**Purpose**  
Generate internal drafts aligned to voice memory.

**Required reads**

- `knowledge/style-guide.md`
- `knowledge/voice-memory.md`
- relevant campaign or brief file

**Primary outputs**

- draft content
- rationale notes
- claims requiring confirmation

**Hard rule**

- mark every unsupported claim explicitly

### 10.7 `/campaign`

**Purpose**  
Package a campaign so it can be executed and measured.

**Primary outputs**

- objective
- audience hierarchy
- asset list
- owner map
- timing sequence
- dependencies
- risk register

### 10.8 `/data`

**Purpose**  
Generate data-driven communications packages from pre-approved aggregate views.

**Primary outputs**

- data report brief
- chart list
- summary insights
- outlet excerpts
- privacy review checklist

**Hard rule**

- no access to raw transaction-level data

### 10.9 `/founder-voice`

**Purpose**  
Develop a founder-led storytelling pipeline.

**Primary outputs**

- candidate scoring
- story assessment
- founder prep
- journalist prep

### 10.10 `/linkedin`

**Purpose**  
Create LinkedIn-ready amplification tied to leadership voice.

**Primary outputs**

- post draft
- opening hook variants
- CTA options
- comment strategy

### 10.11 `/monitor`

**Purpose**  
Evaluate what happened after launch or response.

**Primary outputs**

- coverage summary
- message pull-through score
- misframing list
- correction opportunities
- follow-up recommendations

### 10.12 `/retro`

**Purpose**  
Update the operating system after real use.

**Primary outputs**

- weekly review
- what worked
- what failed
- structural change recommendation
- knowledge updates

### 10.13 `/sync`

**Purpose**  
Prevent local-global collision and produce local variants.

**Modes**

- calendar
- translation
- escalation

**Primary outputs**

- 30-day conflict map
- Ireland-localized message variant
- coordination brief with options and trade-offs

### 10.14 `/policy`

**Purpose**  
Track policy and regulatory context that can affect the narrative.

**Primary outputs**

- policy landscape brief
- relevance assessment
- talking points
- coordination recommendations for policy/legal teams

### 10.15 `/internal`

**Purpose**  
Bridge external comms events into employee communication.

**Primary outputs**

- internal post
- employee FAQ
- Slack update
- manager note

### 10.16 `/warroom`

**Purpose**  
Structure crisis response under uncertainty.

**Primary outputs**

- known/unknown matrix
- stakeholder tiering
- holding statements
- immediate next actions
- escalation triggers

## 11. Workflow Specifications

### 11.1 Daily morning briefing workflow

```text
1. Collect market signals.
2. Run /landscape.
3. Produce morning brief.
4. Route urgent alerts to the comms lead.
5. Update relationship or competitor records only if a true delta exists.
```

Expected SLA:

- Standard morning brief by 08:00 local time
- Crisis pre-scan by 06:00 local time during elevated-risk periods

### 11.2 Pre-interaction workflow

```text
1. Human requests /brief with target and context.
2. System reads relevant relationship, narrative, and recent-coverage files.
3. System outputs prep pack.
4. Human conducts interaction.
5. Human or assistant runs /rolodex with post-contact notes.
```

### 11.3 Campaign creation workflow

```text
1. Run /narrative on the objective.
2. Run /angles on the selected thesis.
3. Run /campaign to produce the plan and dependencies.
4. Run /draft for required materials.
5. Run /brief for stakeholder and reporter preparation.
6. Run supporting agents: /linkedin, /founder-voice, /data as needed.
7. Human approves and executes.
8. Run /monitor after launch.
9. Run /retro at campaign close.
```

### 11.4 Crisis workflow

```text
1. /landscape flags a high-risk signal.
2. Open incident with /warroom.
3. Confirm facts vs unknowns.
4. Draft holding variants.
5. Run /sync escalation if global conflict risk exists.
6. Run /internal for employee message.
7. Deliver stakeholder-specific briefs via /brief.
8. Track coverage via /monitor.
9. Capture lessons via /retro.
```

### 11.5 Voice-memory workflow

```text
1. /draft produces a first draft.
2. Human edits materially.
3. Edit diff is reviewed.
4. Repeated patterns are added to voice memory.
5. Future /draft and /linkedin runs read the updated voice memory.
```

### 11.6 Data-franchise workflow

```text
1. Define report thesis via /narrative.
2. Query approved aggregate views via /data.
3. Review privacy and aggregation gates.
4. Draft executive summary and outlet excerpts.
5. Build launch plan in /campaign.
6. Prepare journalist and executive briefs.
7. Monitor coverage and citations.
8. Store reusable methodology and lessons in archive.
```

## 12. Prompt Contracts

Prompts must be stable enough to produce consistent specialist behavior and explicit enough to constrain sloppy generation.

### 12.1 Global system prompt

```text
You are a specialist agent inside Comms-Stack for Stripe Ireland.

Your job is to improve preparation quality, narrative clarity, and institutional memory.
You are not authorized to publish, send, or imply final approval on any external communication.
Use the knowledge layer as source of truth. If the knowledge layer is silent, say so explicitly.
Prefer concise, decision-useful outputs over generic prose.
When a claim is unverified, mark it as UNVERIFIED.
When legal, policy, or reputational risk is present, surface it plainly.
```

### 12.2 `/landscape` prompt contract

```text
Produce a daily Ireland comms briefing.

Priorities:
1. Detect meaningful signal changes, not noise.
2. Flag timing-sensitive developments.
3. Highlight any shift in how Stripe, competitors, or Irish digital commerce are being framed.
4. Note reporter behavior that suggests a story is forming.

Output sections:
- Top developments
- Why this matters
- Competitive context
- Reporter watch
- Policy watch
- Recommended actions today

Do not invent monitoring evidence. If a signal is weak, say "weak signal."
```

### 12.3 `/brief` prompt contract

```text
Prepare a one-page interaction brief for a human operator.

The brief must include:
- who this person is
- why this interaction matters now
- what they care about
- three talking points
- two likely objections or questions
- one thing to avoid
- relationship context
- recommended posture

Do not draft the final outreach email unless explicitly asked for a pitch-pack.
Even in pitch-pack mode, provide strategy and notes, not final-send copy.
```

### 12.4 `/narrative` prompt contract

```text
Build the argument stack behind a communications objective.

Return:
- one-sentence thesis
- supporting arguments
- proof points needed
- likely critiques
- Ireland-specific resonance
- what would make the thesis stronger

Reject vague framing. Force specificity.
```

### 12.5 `/draft` prompt contract

```text
Draft material in the author's working voice using style-guide.md and voice-memory.md.

Rules:
- do not use banned terms from voice memory
- favor the author's preferred structure
- mark every unsupported fact as UNVERIFIED
- include a short note listing the edits most likely still needed
```

### 12.6 `/warroom` prompt contract

```text
Open and manage a communications incident.

Produce:
- situation summary
- confirmed facts
- unknowns
- stakeholder map by tier
- holding statement variants
- next actions in the next 15, 60, and 180 minutes

Stay disciplined:
- do not speculate beyond the evidence
- separate perception risk from factual risk
- identify if cross-geo coordination is required
```

### 12.7 `/retro` prompt contract

```text
Review the last week or campaign and improve the system.

Return:
- what worked
- what failed
- what surprised us
- what to merge, split, add, or retire
- what knowledge files must change

Do not produce generic retros. Tie every recommendation to observed behavior or outcomes.
```

## 13. Operating Rules

### 13.1 Editorial rules

1. External words remain human-owned.
2. AI may draft, summarize, compare, and package, but cannot imply approval.
3. The system must optimize for clarity and credibility over flourish.
4. Every major draft must declare what is assumed vs confirmed.

### 13.2 Source and evidence rules

1. Every non-obvious claim must have a source or be marked `UNVERIFIED`.
2. Reporter preferences must be tied to observed interactions when possible.
3. Data-franchise outputs must cite approved aggregate views and privacy review status.
4. Crisis outputs must maintain an explicit known/unknown split.

### 13.3 Memory rules

1. Every significant interaction should produce a `rolodex` update.
2. Every material human edit to drafted copy should be considered for voice memory.
3. Every campaign or incident should end with a retro artifact.
4. Memory should prefer durable patterns over ephemeral trivia.

### 13.4 Approval rules

Human approval is required for:

- any reporter outreach
- any public post
- any quote
- any crisis posture decision
- any policy-sensitive message
- any use of internal or sensitive data

### 13.5 Coordination rules

1. Global and local calendars must be checked before launch-sensitive moments.
2. Timing conflicts that create reputational ambiguity escalate via `/sync`.
3. Employee communications should not lag major external events without a reason.

## 14. Guardrails and Risk Controls

### 14.1 Hard safety boundaries

- No raw transaction data access from comms-facing agents
- No autonomous send or publish
- No hidden use of AI-generated outreach as if it were purely human-authored
- No unsupported claims in crisis, policy, or data outputs

### 14.2 Failure modes

| Failure mode | Impact | Mitigation |
|---|---|---|
| Overconfident but weak briefing | Poor judgment | Require explicit confidence and evidence tags |
| AI-written outreach feels uncanny | Relationship damage | Use pitch-pack mode, not final-send drafts |
| Global-local timing collision | Narrative confusion | Calendar and escalation modes in `/sync` |
| Drafts sound generic | Reduced trust and more edits | Continuous `voice-memory.md` updates |
| Data report overreaches | Reputational and privacy risk | Aggregate-only data paths and review gates |
| Crisis speculation outruns facts | Credibility damage | Strict known/unknown matrix in `/warroom` |

## 15. Observability and Metrics

### 15.1 Daily rhythm metrics

- morning brief completion rate
- pre-meeting brief usage
- relationship update latency

### 15.2 Narrative metrics

- inbound press inquiries
- citation frequency as a source of truth
- message pull-through rate

### 15.3 Campaign metrics

- placement quality
- founder-story conversion
- LinkedIn amplification engagement
- repeat use of campaign assets

### 15.4 Crisis metrics

- time to first alert
- time to first holding statement
- time to first internal employee note
- correction rate on misframed stories

### 15.5 Memory metrics

- relationship graph coverage
- voice-memory convergence
- playbook completeness
- archive reuse rate

## 16. Implementation Notes

This document describes the target operating system, not the codebase structure for an implementation. A later implementation can choose:

- pure Markdown + scripts
- Markdown + YAML sidecars + local CLI
- a thin orchestration layer backed by a graph store

Recommended implementation path:

1. Start Markdown-first.
2. Add structured sidecars only for graph and workflow needs.
3. Keep the knowledge layer human-readable from day one.

## 17. Rollout Plan

### Phase 1: foundation

Ship:

- `/landscape`
- `/brief`
- `/rolodex`
- `/narrative`
- `/draft`
- `/warroom`
- `/retro`

Goal:

- establish daily utility, crisis readiness, and memory capture

### Phase 2: campaign system

Ship:

- `/angles`
- `/campaign`
- `/monitor`
- `/sync`
- `/linkedin`
- `/founder-voice`

Goal:

- make campaigns repeatable and coordinated

### Phase 3: franchise and policy

Ship:

- `/data`
- `/policy`
- `/internal`

Goal:

- establish Stripe as a recurring source of truth and reduce coordination gaps

### Phase 4: v2 intelligence

Ship:

- `/foresight`
- `/visual`
- `/go`

Goal:

- add proactive planning, visual support, and command composition

## 18. Future Extensions

### 18.1 `/foresight`

Phase 1:

- calendar of inevitabilities
- prebuilt narrative stacks for known events

Phase 2:

- predictive narrative modeling from landscape and policy history

### 18.2 `/visual`

- branded visual specs for charts and social assets
- Figma-ready output or equivalent design handoff

### 18.3 `/go`

- orchestration command that selects and sequences the right agents for a given objective

## 19. Open Questions

1. When should the relationship layer migrate from Markdown to a graph-backed store?
2. Which sources are approved for policy and media monitoring in production?
3. How should privacy and data-review status be represented in reusable machine-readable form?
4. Which internal systems should be write targets versus read-only context providers?
5. How should per-author voice memory be segmented when multiple leaders need distinct drafting support?

## 20. Final Design Summary

`Comms-Stack` v1 is a **16-agent, knowledge-centric, two-speed communications operating system**.

It is designed around three convictions:

1. The highest leverage is in preparation, not autonomous publishing.
2. The most valuable asset is a compounding knowledge layer.
3. The right system should make human judgment sharper, faster, and more consistent over time.
