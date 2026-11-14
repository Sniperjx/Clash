# ORCHESTRATION — The Clash RSI System (v1, 2026-11-14, JJ's design brief)

One folder, one set of rules, several ways to staff it. The CHARTER (tiers,
rails, gates) never changes with staffing — only who sits where does. Every
session, however staffed, reads this folder first and leaves its results here.

## Roles

- **Director** — plans the session and audits the results, working from TEXT
  (this folder), never from the game screen. May be JJ, Fin, or Claude (Sonnet).
  A director touches no game input; directing requires no benchmark gates.
- **Seat** — the judgment model that owns a live session and answers for it
  (today: GPT Sol). Owns tier decisions, attack calls, and verification.
- **Hands** — a supervised executor inside the seat's session (today: Terra),
  bounded by TERRA-SCOPE and the CHARTER supervised-hands rules.
- **Auditor** — Fin, asynchronously: verifies logs against STATE, rules on
  amendments, keeps this pack honest. Not in the live loop.

## Seat configurations

- **Config A — GPT solo (LIVE today):** Sol seats, Terra hands, Fin audits.
- **Config B — Claude directs GPT:** Sonnet (director) writes the session plan
  into this folder; the GPT seat executes it; Sonnet reviews the folder results
  and writes the next plan. Spends Claude usage on judgment and GPT usage on
  execution — each where it is cheapest.
- **Config C — Scheduled launch:** on JJ's schedule, Claude opens the GPT app
  on the PC, hands GPT a session brief from this folder, and GPT runs it
  unattended-in-tier; results land in the folder for director/Fin audit. The
  PC-side machinery (scheduling, app launching) is built and owned by PC-side
  Claude — his exclusive lane. This document is the protocol it implements.
- **Config D — JJ present:** any configuration with JJ watching; JJ's word and
  JJ's Escape key outrank every plan, always.
- Claude as a *player* (hands on the game itself) is a different thing from
  directing: if JJ ever seats Claude at the controls, Claude starts at Tier 0
  and passes B0/B1 like anyone. Directing never implies playing clearance.

## The attack pipeline — frame economy (the usage problem, solved by shape)

Screenshots are the context sink; judgment is not. The pipeline rations the
seat's frames and gives the high-frame work to the hands:

1. **SEARCH — Terra.** Clicks Next and classifies every offered base against
   the written rubric (class call, TH position, sweeper coverage, loot). NO-GO
   classes are discarded by Terra alone. On an ELIGIBLE base, Terra captures
   one scout view and calls the seat. Searching never consumes seat frames.
2. **DECIDE — Seat, <= 15 seconds.** The scout window (~30s before the battle
   clock starts) is the hard wall, so the seat's job is a checklist, not an
   essay: confirm the class call, pick the entry segment, name the Freeze
   targets. This is only possible because the attack plan is PRE-WRITTEN per
   base class (the standing script + class cards) — the seat selects and
   fills blanks; it does not improvise a plan per base. **Timeout or no
   answer = Next.** A skipped good base costs 1,600 gold; a rushed bad plan
   costs the attack.
3. **EXECUTE — Seat (default).** Deployment accuracy is the seat's proven
   skill (Series B: ~14.7s mean windows, 1 recovered miss in 5). Terra
   executing battles is NOT granted by this document — it is its own benchmark
   track (Terra-B: Practice input accuracy first, then supervised live
   execution with the seat calling batches), granted only on evidence.
4. **MONITOR — triggers, not spectating.** Nobody watches the battle
   frame-by-frame. The script runs in batches; the seat sees only
   batch-boundary frames (~3-4 per battle). Terra may watch for trigger
   events (hero health crossing the ability threshold, pack reaching the
   core, a cluster qualifying for the reserve Rage) and pull the seat in only
   on a trigger. Spectating was the context bonfire; this ends it.
5. **REVIEW — text.** Settled results come from the Attack Log (one read).
   Hands draft the log entries; the seat verifies and commits (standing rule).

## Context and usage doctrine

- The seat's frames per battle are budgeted: scout confirm 1-2, batch
  boundaries 3-4, settled log 1. Anything beyond that needs a named reason.
- State travels as TEXT in this folder, read once — never re-screenshotted
  into existence every session.
- The director's context is spent on plans and audits (text), the seat's on
  decisions (few frames), the hands' on volume (many cheap frames).
- Every session logs its rough usage shape (frames taken by role, battles,
  chores done) so allocation is tuned on evidence at reviews — that tuning
  loop is part of the RSI, not an afterthought.

## GPT account rotation (JJ's two accounts)

- Rotation is BY SESSION, never mid-session and never mid-battle.
- SESSION-LOG records which account ran each session.
- Default: alternate accounts session by session. A director may assign a
  specific account when JJ reports one has usage to burn — that assignment is
  written into the session plan.
- The switching mechanics inside the PC apps are the implementers' problem
  (Claude/GPT on the PC); the system's requirements are only: log the account,
  never switch mid-session, and a switch never changes tiers or gates.

## Scheduled sessions (Config C protocol)

A scheduled run requires, in this folder BEFORE it fires: a session brief
(workstream, the exact trials or chore list, stop conditions, account
assignment). The seat executes within its earned tiers — a schedule grants no
tier, no spend, and no exception. Anything unexpected follows the standing
rule: stop, screenshot, log, leave it for the director. JJ can cancel any
schedule at any time; a missed or failed launch is logged, never retried in a
loop.

## The RSI loop

Sessions produce logs; logs produce reviews (TRIAL-LOG, series reviews);
reviews produce amendments to this pack (ATTACK-PLAN, TERRA-SCOPE, this file);
amendments are versioned and ruled by Fin with JJ as the final gate on
anything touching tiers, rails, or money-adjacent rules. The system improves
the system — with receipts.
