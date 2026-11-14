# SCHEDULE — Scheduled-Run Design (Clash RSI) — DESIGN, NOT YET LIVE

Status: design for CLO1's PC launcher build (ORCHESTRATION Config C) + JJ's
window choices. Nothing here fires unattended until (a) the launcher exists,
(b) the seat's first run of each shape is attended, (c) JJ approves the
windows. Tier rails apply unchanged: unattended runs are Tier 0 / claims /
earned-Tier-1 shapes only; no Tier 2+ unattended until earned and ruled.

## Run shapes
1. **Chore circuit** (Tier 0 + claims): collectors, normal obstacles (NEVER
   event obstacles), free claims per CHALLENGE-INVENTORY, BB collections,
   Clock Tower when its free boost is off cooldown. ~Daily.
2. **Upgrade-trigger check**: read builder/lab/pet timers; when a slot is
   free AND PRIORITIES v2's next item for that slot is affordable, start it
   (directed-queue starts only; verify cost in-game before confirming; log).
   Runs a few times daily — timers, not the clock, drive value.
3. **Attack block** (only for seats/tiers that have earned it): a packaged
   trial/farming block with predeclared stop rules, logged per trial.
4. **Claim sweep**: Daily Tasks / event free tracks / Clan Games free claims
   as they appear; choice nodes seat-decided and logged per the claims grant.

## Proposed windows (JJ to confirm/adjust; PC is often left on)
- Late morning PT: chore circuit + upgrade check (catches overnight timers).
- Afternoon PT: attack block window (aligns with GPT 5h resets when usable).
- Evening PT: chore circuit + upgrade check + claim sweep.
- Overnight: only long-timer verification (e.g. pet completion ~03:33 PT
  events) — no new unattended shapes overnight until the day shapes are
  proven boring.

## Hard constraints (measured, not assumed)
- GPT account rotation CANNOT be automated (browser account chooser needs
  JJ's click; agents never type credentials). Schedules use the signed-in
  account; rotation happens when JJ is present.
- Claude scheduled launches need the PC launcher (CLO1 builds; Claude-as-
  director needs no game gates, Claude-as-player earns them in-game).
- Any unexpected dialog, spend prompt, or rail-adjacent screen stops the
  run and logs — unattended never improvises.

## JJ's task lists
JJ may hand Fin a list for a window ("do X, Y, Z tonight"); Fin slots items
into the shapes above, rules on anything the list doesn't cover against the
plan of record, and reports back per item: done / blocked / needs JJ.
