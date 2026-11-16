# AUTOMATION — The Standing Runbook (JJ mandate, 2026-11-16)

JJ's directive: the system runs the account end-to-end — collecting,
attacking, building — without him present. He touches only: GPT account
switches, Tier 3 calls, and one-off owner decisions (base picks, clan
bonus medals). Everything else is the seats' work, pulled from TASK-QUEUE.md.

## Usage cascade (JJ, 2026-11-16)
Spend GPT's usage first wherever GPT can do the work; spend Claude's usage
where GPT can't (directing, verifying, Claude-seat blocks, judgment-heavy
inspections). When GPT's pool dies mid-queue: Claude-shaped work continues,
GPT-shaped work parks. When both are dry: the queue parks and Fin's
oversight notes it once. Account switching stays JJ-present (measured
constraint); reading which account is signed in is a look-only read any seat
may do itself.

## Session shapes
- **Config B (default workhorse):** Scout directs, GPT (Sol/Terra) plays.
  Chores, queued upgrades, GPT-seat attack blocks.
- **Scout solo:** Scout's own blocks, inspections, B0 circuits.
- **Fin desk work:** research, plans, audits — no game contact.
A session starts when JJ opens one, says "run it," or the PC launcher
(below) fires. Sessions always: refresh state -> work the queue top-down ->
log + update STATE -> report in the Muse chat.

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
