# AUTOMATION — The Standing Runbook (JJ mandate, 2026-11-16)

JJ's directive: the system runs the account end-to-end — collecting,
attacking, building — without him present. He touches only: GPT account
switches, Tier 3 calls, and one-off owner decisions (base picks, clan
bonus medals). Everything else is the seats' work, pulled from TASK-QUEUE.md.

## Operators (JJ simplification, 2026-11-18 — supersedes the 2026-11-16 cascade)
**Sol (GPT) and Sonnet (Claude) only.** The two seats are interchangeable
single operators: identical protocol, identical grants, same queue, same
rails, both reporting to Fin in the Muse chat. JJ opens whichever seat he
has usage for; that seat works the queue solo. Terra is retired as hands;
no other model operates the account. Config B (one seat directing the
other) is retired. Trial evidence is still logged per operator — records
stay honest even though permissions are shared; B2 remains per-operator
until one passes. Account switching stays JJ-present (measured constraint);
reading which account is signed in is a look-only read any seat may do
itself. When one pool is dry, JJ opens the other seat; when both are dry,
the queue parks and Fin's oversight notes it once.

## Commands
JJ runs the account with one-line orders defined in COMMANDS.md
(chores / attacks / upgrades / status / full run). Passes, challenges,
and unclaimed rewards are tracked in TRACKER.md, updated every run.

## Session shapes
- **Seat session (the only game shape):** JJ opens Sol or Sonnet; the seat
  refreshes state -> works the queue top-down -> logs + updates STATE ->
  reports to Fin in the Muse chat.
- **Fin desk work:** research, plans, audits — no game contact.
A session starts when JJ opens one, says "run it," or the PC launcher
(below) fires.

## Schedule windows (PT; PC is often left on)
Late morning: chore circuit + upgrade-trigger check. Afternoon: attack
blocks. Evening: chores + triggers + claim sweep. Overnight: timer
verification only. Fin runs a daily oversight check (~9am PT): reads the
repo, flags finished timers with no follow-up start, seats idle >24h with
queue items pending, and stale state — actionable items only, else silent.

## Trigger rules (every session, in order)
1. Any builder/lab/pet slot free + next queue item for that slot affordable
   (menu-verified price, post-Jam) -> start it. Builder verified free BEFORE
   any Treasury collect; collect only funds a same-session start.
2. Claims sweep: free claims logged; choice nodes seat-decided + logged.
3. Attack blocks run as packaged series under their predeclared governance.
   Routine farming (Tier 2) unlocks per seat only on a B2 pass.

## Rails (unchanged, always)
No gems, no money, no Ranked sign-up, no event-obstacle clearing, no clan
social actions, no items without a Fin ruling, no CC payload requests.
Unexpected dialog = stop + log. Goblin Builder dialog = close, never pay.

## The one missing machine piece (CLO1 build item)
A PC-side launcher that opens the Scout session at the schedule windows
with the queue brief attached (Windows Task Scheduler + the session's
standing start prompt). First runs of each shape attended (AFK-0
discipline). Until it exists, sessions start on JJ's word or when a seat
session is already open. Fin cannot launch PC sessions from the VM.
