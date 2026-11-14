# CHARTER — Mission, Tiers, Rails

## Mission

Progress JJ's Clash of Clans account productively and get better at playing it over time:
resources collected, obstacles cleared, builders and Lab never idle, upgrades following
the agreed queue, and attacking skill that climbs from "poor" to "reliable" through
measured practice. JJ (account: level 226, TH17, clan Boysenberry, co-leader) lets you
play because this system makes you accountable: everything is logged, graded, and earned.

## Permission tiers

You hold a tier **per activity**, not overall. Both agents (Claude, GPT) start where the
evidence puts them — GPT's 2026-11-14 tests are the seed evidence (BENCHMARKS.md).
Claude starts at Tier 0/1 by default and takes the same benchmarks; prior reputation
earns nothing here, only logged results do.

| Tier | Activities | How it's earned |
|---|---|---|
| **0 — Chores** | Collect from mines/collectors/drills, Loot Cart, Builder Base collectors; clear **normal** obstacles (trees, bushes, stumps, mushrooms, Gem Boxes); inspect anything; read profiles/lists | Default. GPT already proven reliable here (2026-11-14). |
| **1 — Housekeeping** | Train/change saved armies; donate troops (when a request is visible and the requested troop is known); Practice attacks; Friendly Challenges; single-player (goblin) maps; start upgrades **on the PRIORITIES queue** when a builder is free and resources suffice; Lab research on the queue | Navigation reliability: 3 consecutive chore sessions with zero wrong-screen errors logged, + read PLAYBOOK/LESSONS. |
| **2 — Farming attacks** | Multiplayer **Battles** (non-ranked) attacks for loot with the approved army; may surrender a lost attack to save time/heroes | Benchmark gate B2 (BENCHMARKS.md): practice standard met across 5 logged attempts. |
| **3 — Stakes (JJ-gated)** | War/CWL attacks, Ranked/Legends attacks, Clan Capital raid attacks, spending Magic Items, starting **off-queue** upgrades, Builder Base versus battles for trophies | **Never self-granted.** JJ says yes per era/season. Log his yes in this file with the date. |

Current tier status (update this table as evidence lands):

| Agent | Chores | Housekeeping | Farming | Stakes |
|---|---|---|---|---|
| GPT | ✅ Tier 0 (proven 2026-11-14) | Not yet (donation unproven; upgrades untested) | ❌ (practice best: 31%, 0★) | ❌ |
| Claude | Tier 0 (default) | Not yet | ❌ | ❌ |

## Supervised hands — the two-model seat (JJ's architecture, 2026-11-14)

A seat can be TWO models: a judgment model (GPT Sol; later, for Claude's trial,
Sonnet) directs a faster hands model (Terra; later Haiku). The pattern is JJ's, and
it mirrors how his whole stack works — the strong model plans and verifies, the fast
model executes volume. Rules:

- **The judgment model owns the seat.** Its tier is the seat's tier. It plans the
  session, verifies the hands' results (balances, screenshots, logs), and answers
  for everything the hands did. Muse holds the judgment model accountable, not
  the hands.
- **Hands inherit a capped subset, never the whole tier.** Hands may run: Tier 0
  chore circuits, mechanical navigation/collection, and repetitive drill inputs
  the judgment model specified. **Expanded scope (JJ, 2026-11-14):** name-verified
  normal obstacles, zero-choice free claims, the bounded Sol-reviewed donation
  flow, Clan Capital free-Forge claims, and Builder Base chores — all itemized
  with stop conditions in TERRA-SCOPE.md, which is the controlling document for
  hands scope. Hands may NOT: start upgrades or research, make queue decisions,
  resolve reward CHOICE/overflow nodes, spend Capital Gold or convert resources,
  play Builder Base versus battles, or edit STATE/PRIORITIES.
- **Hands' evidence is labeled, not pooled.** Trial and session entries carry
  [Terra] / [Haiku] tags with "supervised by <judgment model>." Input-skill
  evidence (deployment speed, misses) accrues to the hands model — that is
  exactly what it is being auditioned on.
- **State edits: hands draft, the seat owner commits.** A hands model may prepare
  STATE/log updates, but they take effect only after the judgment model verifies
  and commits them. (Clarified 2026-11-14 after Terra's first supervised session
  updated STATE before this ruling reached Sol; Sol reviewed those changes after
  the fact and they stand — one-time exception, not a precedent.)
- **Unsupervised hands = their own gauntlet.** While supervised and verified in
  the same session, hands work under the seat's tier. The moment hands would play
  a session the judgment model is not reviewing, they need their own B0/B1 passes
  like any new agent.
- Rails bind hands identically. A rail violation by hands ends the experiment
  and is logged against the seat.

## Hard rails — never, at any tier

- **Never spend gems.** Not one, not for anything. (Balance at system start: 2,803.)
- **Never spend real money** or open purchase flows beyond cancelling out of them.
- **NEVER CLEAR EVENT OBSTACLES. ONLY NORMAL obstacles may be cleared** (JJ's emphasized
  rule, 2026-11-14). "Event" covers anniversary cakes, holiday/seasonal obstacles, and
  anything decorated or unique. Cleared list is ONLY: normal trees, bushes, stumps,
  mushrooms, and Gem Boxes. When in doubt, it is an event obstacle — leave it, log it.
- **Never act as JJ socially:** no clan chat messages, no clan mail, no kicking/promoting/
  demoting anyone, no leaving the clan, no changing clan settings, no friend requests.
  Donating a requested troop is the only clan interaction allowed (Tier 1+).
- **Never change account settings,** name, Supercell ID, or linked devices.
- **Never attack in War/CWL/Ranked/Legends** without Tier 3 (JJ's logged yes).
- **Never start an upgrade that isn't on the PRIORITIES queue** without Tier 3.
- If the game shows something you don't understand — a new dialog, a confirmation you
  didn't expect, a purchase screen — **stop, screenshot/note it in the log, and back out.**
  Confusion is a stop signal, not a click-through signal.

## Spending resources (allowed, within the tiers)

- Starting **queued** upgrades/research with gold/elixir/dark elixir: Tier 1+.
- Clearing normal obstacles (costs elixir/gold, often yields gems): Tier 0.
- Training armies: Tier 1+. Donations: Tier 1+.
- Walls with overflow resources, using a FREE builder (walls are instant but still need
  one — v1.1 correction): Tier 1+, per PRIORITIES Tier E.

## The improvement rule (RSI)

This system's whole point is recursive improvement. Procedure improvements (better
technique, better order inside a tier) you may adopt yourself — log them in LESSONS.md.
Tier promotions follow the benchmark gates. **Rail changes are never self-granted:**
anything in the "Hard rails" list can only be changed by JJ, recorded here with his date.
If you believe a rail should change, write the proposal at the bottom of LESSONS.md
under "Proposals for JJ" and keep obeying the rail until he rules.
