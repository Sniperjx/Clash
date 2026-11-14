# HANDOFF — supplementary, for Claude (from Muse, 2026-11-14)

Companion to KICKOFF-CLAUDE.md. New evidence landed after that brief was
written: a Terra pilot. This file carries its assessment, the revised handoff
protocol, the Haiku capability probe, and the frame/latency budget your seat
design must use. Sol's local files (SESSION-LOG #12, ATTACK-REVIEW, STATE)
are the primary record; this is Muse's reading of them.

## 1. Terra pilot — assessment (session #12, JJ-authorized, ONE pilot only)

Terra executed a real multiplayer attack under Sol's supervision: ~TH16-class
mixed-compartment base (visual assessment), Army v1 exact, unboosted, no
CC/siege. **Result: 100%, 3 stars.** Loot ledger exact to the digit
(751,194 G / 783,875 E / 7,803 DE + full bonus; entry fee reconciles).
What it proves and what it does not:

- PROVEN: supervised hands execution of a complete attack, end to end, with
  the rails and spell gates intact — one Rage correctly unused, the TH-zone
  Rage correctly skipped after the TH fell. Gate behavior transferred from
  the seat to the hands. That is the pilot's real finding.
- NOT PROVEN: TH17 competence (the base was a class below every Series B
  target); first-placement accuracy (the initial batch was rejected and the
  entry changed — deployment took 21.852s first-attempt-to-last INCLUDING
  the rejection and recovery, a different and honest metric, not comparable
  to Sol's 13-18s clean-placement windows); unsupervised navigation (two
  recoveries needed Sol: a wrong Season Pass shortcut, a stale-frame/target
  concern); ability utility (W/MP/Q "grey" is operator-reported; Sol verified
  the result and the loot, not the abilities).
- STATUS: the Terra-B (hands execution) track has its first data point —
  supervised execution proven at soft-target level. The track continues with
  graduated difficulty; it does not graduate. JJ's authorization covered ONE
  pilot; it does not extend. No usage-savings or model-superiority claim is
  made or implied by n=1.

## 2. Handoff protocol (revised, concise — all seats, all houses)

1. **One PC operator at a time.** Every handoff is an explicit SESSION-LOG
   line: who holds the PC, from when, under which config (ORCHESTRATION).
   Overlap is a defect, not an efficiency.
2. **A handoff carries four things:** the STATE pointer (balances + in-flight
   timers), open items, the receiver's authority scope (seat/tier/config),
   and the stop conditions. Anything not carried is not assumed.
3. **Records outrank recollection.** Until Claude's merge lands, PC-local
   files are authoritative; Muse mirrors from seat reports and flags drift
   (the pre-pilot up-drift in STATE is the standing example: logged,
   unattributed, never silently absorbed).
4. **Anyone can call STOP;** resumption belongs to the director or JJ.
   A stopped session logs why, mid-state, without tidying the record first.

## 3. Haiku capability probe (NO assumed parity with Terra/GPT tooling)

Terra's hotkey map, latencies, and input channels are Terra's. Haiku's
computer-use implementation gets probed on its own before any tasking —
results logged as the Claude seat's first evidence, envelope granted =
intersection of passed probes:

- **P1 Screen literacy:** read balances, troop/spell counts, and hero levels
  from live screens vs ground truth — 10 screens, >= 95% field accuracy.
- **P2 Targeting:** click named buildings on a real base (Practice or a
  scout view) — hit rate and miss distance recorded, 20 targets.
- **P3 Input channels:** EMPIRICALLY test which channels work in Haiku's
  implementation (hotkeys? click-count deployment? drag?) — one test per
  channel per action type. Import nothing from PLAYBOOK's GPT map.
- **P4 Latency:** measure instruction-to-action round trips across a session.
  Hard budgets exist (the ~30s scout window; batch deployment windows).
  If Haiku's latency busts a budget, its envelope legitimately shrinks to
  non-time-critical work (chores, searching between battles, drafting,
  review) — a valid outcome, recorded as such, not a failure to hide.
- **P5 Recovery:** induce a wrong-screen state — does it stop-and-report
  (pass) or wander (fail)? Terra needed two supervised recoveries in one
  pilot; Haiku's recovery behavior gates any unsupervised scope.

## 4. Frame/context budget, with latency fallback

Budgets (per ORCHESTRATION's frame economy, now with fallbacks):

- Seat per battle: scout confirm 1-2 frames, batch boundaries 3-4, settled
  Attack Log 1. Director: text only. Hands searching: many cheap frames,
  capped per session and logged.
- **Decide-step fallback:** if the seat has not decided within ~15s of the
  scout call, the hands Next. Pre-agreed, no debate in the moment.
- **Execution fallback:** if hands action latency exceeds the batch budget
  mid-attack, the seat takes over ONLY at a batch boundary — never mid-batch
  (two operators in one batch is how inputs collide).
- **Degradation fallback:** if round-trip latency runs > 2x the session's
  baseline, the session degrades to chores-only mode and logs it. Attacking
  on a degraded link is how red-zone rejections become lost battles.
- Every fallback firing is logged with its trigger; fallback frequency is a
  review metric, not an embarrassment.

## 5. Next validation steps (in order; none authorized by this file)

1. Claude: repo merge (MERGE-NOTE), then CLAUDE-SEAT.md design + challenge
   inventory per KICKOFF-CLAUDE.
2. Claude seat: run the Haiku probe (P1-P5) in Practice/look-only surfaces;
   publish results before proposing any Haiku envelope.
3. Treasury live inspection (balance/capacity) at the next chore circuit —
   closes the last receipts-inference in STATE.
4. Series C when a cleared seat is staffed and JJ's workstream says attacks.
5. Terra-B continues only under a fresh JJ authorization per pilot block,
   difficulty graduated (TH17-class next), Sol supervising.

Game is CLOSED as of this writing (JJ). Nothing here launches anything.
