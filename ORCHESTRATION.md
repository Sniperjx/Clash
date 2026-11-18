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

## Roadmap (JJ's directive, 2026-11-14 — read with #interpret latitude)

The point of the whole system: **JJ's spare model usage — Claude's, GPT's, or
a mix — converts into account progression while JJ is AFK**, on schedules,
inside the charter. Staffing follows usage: whichever house has usage to burn
staffs the seats; the folder and the rules are constant.

**North star (JJ, 2026-11-14): competence at LOW usage.** The system must
learn to play well without burning usage on constant screenshots, so the same
budget covers more work. Efficiency is therefore a first-class metric,
reviewed like battle stats: usage per chore circuit, per battle, per
challenge, logged per session. The levers: hands-first volume (cheap models
see the many frames; judgment sees summaries and decisive frames only),
state carried as text instead of re-screenshotted, sessions batched (one
circuit does all chores; attacks run in series), settled-source reads over
live spectating — and above all RELIABILITY, because retries, recoveries,
and verification loops are the hidden usage sink. Fundamentals get reliable
first; clan management, wars, and CWL (Phase 3) are earned on top of a cheap,
dependable base, not bolted onto an expensive one. JJ is out of the loop for
operations; the seats and Muse run it and bring him results.

- **Phase 1 — the Claude seat (NEXT).** Sonnet designs how a Claude seat runs
  efficiently: Sonnet as the seat's judgment, Haiku as its hands (the
  Sol/Terra shape, Claude-flavored) — what Haiku can scout, search, collect,
  and verify; Sonnet's frame budget; how the seat learns (its own LESSONS and
  review entries, same RSI discipline). Design first (director work, no game
  gates needed); playing clearance is earned through B0/B1 like every seat.
  Sonnet's brief: KICKOFF-CLAUDE.md.
- **Phase 2 — AFK progression.** Scheduled sessions (Config C) doing the
  earned-tier work unattended: chores, the daily routine, farming inside the
  seat's tier, Series C trials when a cleared seat is scheduled — plus
  **challenge and reward completion**: season/event challenge tracks, Clan
  Games-style tasks, and free-track claims, each mapped to a tier BEFORE it
  is automated (free claims and no-choice tasks are low-tier; anything with
  choice nodes, spends, or clan-visible effects keeps its existing gate).
  Nothing in this phase expands a tier by implication.
- **Phase 3 — bigger things (JJ-GATED, future).** Wars, CWL, and the rest of
  Tier 3 stay exactly as gated as they are today until JJ explicitly opens
  this phase. "Eventually" is a roadmap word, not an authorization: when JJ
  opens it, the system designs war participation as its own benchmarked
  program (declarations, participation scope, attack standards) before a
  single war action is taken.

## The RSI loop

Sessions produce logs; logs produce reviews (TRIAL-LOG, series reviews);
reviews produce amendments to this pack (ATTACK-PLAN, TERRA-SCOPE, this file);
amendments are versioned and ruled by Fin with JJ as the final gate on
anything touching tiers, rails, or money-adjacent rules. The system improves
the system — with receipts.

---

# AFK Operating Protocol (JJ directive, 2026-11-14 — Fin's interpretation, recorded)

JJ is often AFK and leaves the show to the seats. The loop:

1. **Scout (Claude seat) plays and thinks**: attacks, inspections, in-game
   execution, higher-level in-session judgment. Fin researches, designs,
   rules, audits — Fin does not play.
2. **GPT as Scout's overflow**: when Claude usage runs out OR GPT is simply
   the available hands, Scout tasks GPT through the PC apps (Codex / Chrome)
   as Config B sessions, logged as such. GPT's own seat qualifications and
   the two-model rules (Sol judges, Terra hands) are unchanged.
3. **Account-switch loop**: GPT usage exhausted and a switch needed ->
   Scout reports HERE to Fin -> Fin notifies JJ in this chat -> JJ goes to
   the PC, switches the account himself, and says so here -> work resumes.
   Agents never type credentials, never work around sign-in. If JJ does not
   respond, GPT-dependent work PARKS (no nagging, no repeated pings) and all
   Claude-side / Fin-side work continues; the parked item is re-raised once
   when JJ next appears. A same-account usage-window reset (e.g. a 5h window
   rolling over) needs no switch and no JJ action — the seat just resumes
   and logs it.
4. **Focus**: MAIN village and WAR base only. Builder Base is out of the
   active routine (JJ, 2026-11-14) — no BB chores, no BB circuits, until he
   reopens it. (BB collections already inside a Home circuit stop too.)
5. **Item use**: magic items and potions are system-managed per the ITEMS
   policy (research-backed; potions fire on policy conditions; Books,
   Hammers, and Runes need Fin's per-use approval in chat). Gem-priced or
   money-priced anything stays banned outright. Normal loot and trophies
   are expendable in the name of science; financial/gem mistakes are not.
