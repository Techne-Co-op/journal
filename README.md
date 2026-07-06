# journal

The journal of [Techne](https://techne.coop) — book of original entry for [RegenHub, LCA](https://techne.coop/legal/), a Colorado Limited Cooperative Association in Boulder.

Live at **[journal.techne.coop](https://journal.techne.coop)**

---

## What this is

In accounting, a journal is the book of original entry: where events are first written down before they post to the ledger. This is that layer for the cooperative. Members record contributions, reflections, exchanges, and clearings here. Work moves through a shared board. And the encyclopedia holds what the cooperative has made.

The journal is the cooperative's workshop — door open, work in progress visible on the benches. What you see is real and wearing its stage.

---

## Three surfaces

### Common Work — the shared board

Work moves through six stages: captured → offered → held → standing → socialized → resolved. Each stage is a plain word with a plain meaning. Nothing resolves without a named member performing that act.

Path: `/common-work/`

### The Daybook — each member's record

Where members write. Four kinds of entry: reflection, contribution, exchange, clearing. Private by default. The member chooses what lands — what becomes part of the shared record. The cooperative sees only rhythm (that you wrote, when, how often) until you share something deliberately.

The bloom visualization renders the day's activity as a clock face. Petals at the hour they were made public, in the color of that hour on the sunset spectrum.

Path: `/daybook/`

### The Encyclopedia — the artifact register

The cooperative's named things: policies, practices, roles, agreements, works — organized into nine shelves by kind. Each entry carries its status, tier of visibility, and who tends it.

Where Daybook and Common Work are flow, the Encyclopedia is stock. A live view of what the cooperative has made and what it governs. Data fetched from the Parachute vault at page load. D3 force graph + hierarchy navigation. Three visibility tiers (public / participant / member) simulated client-side.

Path: `/encyclopedia/`  
Live vault: `https://our.parachute.computer/vault/techne/`  
Tags: `encyclopedia-entry` (18 entries), `encyclopedia-shelf` (9 shelves)

---

## The one rule

**Machines prepare; people land.** Nothing enters the official record — no stage advances, no decision settles, no page publishes — without a named member choosing it. The system is built to refuse otherwise. This is structure, not etiquette.

---

## How work becomes patronage

Each Daybook entry links to a work item. Each work item belongs to a program. Each program accumulates a patronage record. Surplus and standing follow that record, by rules set before the work began.

The stack: your entry → work item → program → patronage record → allocation.

---

## Two addresses

| Address | What it is |
|---|---|
| `journal.techne.coop` | The workshop. Work in the open, wearing its stage. |
| `techne.coop` | The cooperative's voice. Finished, ratified, signed by a named member. |

A page crosses from the journal to the cooperative's voice through the same landing rule — a named member's act, not an automatic promotion.

---

## Repository contents

| Path | Contents |
|---|---|
| `/` | Landing page — introduction to all three surfaces |
| `/common-work/` | Common Work interface — six-stage coordination board |
| `/daybook/` | Daybook interface, bloom visualization, full module spec |
| `/daybook/onboarding/` | Six-step guided introduction for new members |
| `/daybook/two-layers/` | Settled and ripening — the two-layer bloom |
| `/encyclopedia/` | Encyclopedia of Artifacts — live vault view |
| `/architecture/` | Pre-implementation spec: schema, state machines, logic, invariants |
| `/design-system/` | Design System v4 — tokens, components, site application protocol |

---

## Technology

- Static HTML/CSS/JS — no build step, served as GitHub Pages
- D3.js for bloom visualization (daybook) and force graph (encyclopedia)
- Parachute vault REST API for encyclopedia data (`our.parachute.computer/vault/techne/api/`)
- Magic link auth (planned for contribution and clearing entry kinds)
- Techne Design System v4: Libre Baskerville + IBM Plex Mono, sunrise color spectrum

---

## Status

Open-draft for founding members. Launch August 14. Not yet ratified policy.

The cooperative's practice is the elder — where our actual work diverges from what these pages say, we amend the pages to follow.

---

Built by [Techne Studio](https://techne.coop) · RegenHub, LCA · Boulder, Colorado
