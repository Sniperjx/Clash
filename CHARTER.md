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
Claude starts at Tier 0 by default and takes the same benchmarks; prior reputation
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
| GPT | Tier 0 proven | Tier 1 earned: seeds #1/#3 + full circuit #6; Fin accepted 2026-11-14 | Locked; B1 passed (#7, Fin audit), B2 NOT passed (Series B), Tier 2 locked | Locked; no JJ Tier 3 grant |
| Claude | Tier 0 (default) | Tier 1 CLAIMS ONLY — JJ grant 2026-11-14 (free [CLAIM]s under the claim rules, incl. Treasury Collect when DAILY-ROUTINE #20's conditions are met; queued upgrades, donations and Practice remain locked pending B0/B1) | Locked | Locked |

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

## Supervised hands - Fin ratification, 2026-11-14

- The judgment model owns the seat. Its tier is the seat's tier. It plans the session, verifies the hands' results (balances, screenshots, logs), and answers for everything the hands did. Muse holds the judgment model accountable.
- Hands inherit a capped subset, never the whole tier. They may run Tier 0 chore circuits, mechanical navigation/collection, and repetitive drill inputs specified by the judgment model. They may not start upgrades/research, make queue decisions, resolve reward choice nodes, donate, or independently edit STATE/PRIORITIES.
- Hands evidence is labeled, not pooled. Trial/session entries use [Terra] or [Haiku] with "supervised by <judgment model>". Input evidence, including speed and misses, accrues to the hands model.
- Hands draft; the seat owner applies reviewed changes. Hands may prepare STATE/log updates, but those updates take effect only after the judgment model verifies and applies them. Terra's direct STATE updates in #8/#9 were reviewed by Sol and accepted by Fin as a one-time exception, not precedent. Applying reviewed changes does not mean running Git.
- Hands reviewed in the same session operate under the seat's capped permissions. An unattended independent session requires the hands model's own B0/B1 evidence.
- All hard rails bind the hands identically. A violation ends the experiment and is logged against the seat.

Tier-table clarification: GPT judgment seat has a qualified B1 pass from #7 accepted by Fin. B2 was attempted in Series B and NOT passed; Tier 2 farming and Tier 3 stakes remain locked. Terra does not inherit independent qualifications. JJ grant (2026-11-14, relayed to Fin): the Claude seat is approved for Tier 1 [CLAIM] actions only — every claim logged, choice nodes decided by the seat and logged with the pick, paid tracks and gem/medal-priced items never; this grant does not unlock any other Tier 1 activity for Claude.

JJ drill exception (2026-11-14, direct order in chat: start the troops so Scout can get attacks in): the Claude seat may run ONE Practice control proof ahead of its B0 completion, solely as the entry step of Fin's Series C [Scout seat] package (snapshot -> Practice proof -> SC-1..5 under Fin's stop rules). This exception covers that one Practice run and the five packaged Battles trials only; it is not a B1 pass, does not unlock general Tier 1 activity for Claude, and expires when the SC block ends or is paused under its stop rules.

Decision protocol (JJ, 2026-11-14): judgment calls a seat meets in play — conditional claims, Treasury Collect, choice-node picks the pick rule doesn't settle, anything the plan doesn't already answer — go to Fin, not JJ. Fin decides against the plan of record (PRIORITIES queue, DAILY-ROUTINE rules, the CHARTER rails). Decisions are plan-driven: an action with no plan reason behind it doesn't happen just because it's permitted. Only tier grants, rail changes, and plan changes escalate to JJ.

## Expanded supervised chores - 2026-11-14
JJ requested supervised Terra collections,normal obstacles,free claims,requested donations and Clan Capital chores;Builder Base PvP explicitly excluded. TERRA-SCOPE.md controls the bounded execution flow and supersedes the earlier blanket hands donation ban for Sol-reviewed exact visible requests only. Hands still cannot decide queues,spend on conversions/contributions,choose rewards,or independently apply STATE/PRIORITIES changes. Free Forge collection is allowed only after first live verification as a zero-cost collection;conversion slots remain outside routine. All hard rails unchanged.
