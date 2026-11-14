# CLAUDE-SEAT — operating design for the Claude seat (v0 PROPOSAL, 2026-11-14, Sonnet)

Status: PROPOSAL on branch `claude/seat-design`. Nothing here is a ruling. Tiers, rails and
gates are the CHARTER's; this file only says how a Claude seat would run inside them.
Designing needed no gate; touching the game does. The seat is at **Tier 0** until B0/B1 evidence says otherwise.

Labels: **[MEASURED]** = observed in a logged session. **[ESTIMATE]** = my arithmetic or
expectation, to be replaced by a measurement. **[UNKNOWN]** = needs a probe. Nothing below
labeled ESTIMATE may be quoted as a qualification (the Series B habit applies to me too).

## 1. Shape

- **Seat = Sonnet.** Owns the session plan, decisions, verification, STATE/log edits, and answers for everything the hands did.
- **Hands = Haiku** (a Haiku subagent started by the seat). Capped subset per CHARTER "Supervised hands". Evidence is labeled `[Haiku], supervised by Sonnet`.
- **Director** work (writing session plans, reviewing folder results) is text-only and needs no game gate.
- One PC operator at a time (HANDOFF protocol v2). If Sonnet drives directly, Haiku is idle; if Haiku drives, Sonnet does not touch the controls.
- Sonnet driving the controls itself is the fallback and the early default. Today's only Claude game evidence is Sonnet direct (SESSION-LOG #14), so Haiku has zero evidence and zero envelope.

## 2. Haiku envelope (provisional: envelope = intersection of passed probes)

Mirrors TERRA-SCOPE but starts EMPTY. Each row below is the maximum it could ever be, and is
granted only after its probe passes. No row is imported from Terra's evidence.

| Task class | Candidate hands scope | Gate to enter | Probe |
|---|---|---|---|
| Read-only screen reads | Balances, builder/lab status, troop counts, hero levels | P1 >= 95% field accuracy on 10 screens | P1 |
| Home/BB collection | Tap collector bubbles, Loot Cart, Gem Mine | P1 + P2 (hit rate) + P5 (recovery) + one reviewed live circuit | P1, P2, P5 |
| Normal obstacle removal | Name read, then confirm | Same plus first 3 name reads reviewed by seat (TERRA-SCOPE rule) | P1, P2 |
| Free claims | Zero-choice only | Same; first live check per surface reviewed | P1, P5 |
| Base search (Next + classify) | Cheap-frame searching, call seat on ELIGIBLE | P4 latency inside the ~30s scout window and P1 classification agreement with seat on >= 20 bases | P1, P4 |
| Attack execution | NOT proposed. Its own track, after search works. | n/a | n/a |

Hands never: start upgrades/research, resolve choice nodes, donate (until TERRA-SCOPE graduation applies to them), edit STATE/PRIORITIES, or touch Tier 3 surfaces. Any rail breach ends the experiment and is logged against the seat.

If P4 shows Haiku latency busts the scout window, its envelope legitimately shrinks to non-time-critical work (chores, between-battle search review, drafting). That is a valid recorded outcome.

## 3. Probe plan (HANDOFF P1-P5), cheapest first

Run on look-only or Practice surfaces. Ground truth for P1 comes from the settled Home screen and STATE, read by Sonnet first.

- **P1 screen literacy** (10 screens, >= 95% fields): Haiku reads, Sonnet compares to its own read of the same screen. Both reads cost frames; log frames.
- **P2 targeting** (20 clicks on named buildings, Practice or scout view): hit rate and miss distance.
- **P3 input channels:** one test per channel per action type (click, hotkey, drag, click-count deploy). Record which exist at all inside the Play Games window.
- **P4 latency:** timestamp instruction-to-action across the session. Report median and p95, and the 2x-baseline degradation trigger.
- **P5 recovery:** induce a wrong screen (e.g. open the clan panel). Pass = stop and report. Fail = keeps clicking.

Before P1, the **prerequisite check** (assumption A1 below): can a Haiku subagent even call the computer-use tools in this harness? That is a yes/no test costing one tiny task.

## 4. Sonnet frame / context budget per session type

These are budgets to test. Numbers are ESTIMATES until measured; every session logs actuals.

| Session type | Sonnet frames (budget) | Haiku frames | Notes |
|---|---|---|---|
| Chore circuit (B0) | <= 10 total if Sonnet drives; <= 3 if Haiku drives (verify before/after Home + final) | many, capped per session and logged | Read STATE as text first; one before-Home and one after-Home frame minimum. |
| Search + attack | scout confirm 1-2, batch boundaries 3-4, Attack Log 1 per battle (ORCHESTRATION) | search frames cheap, capped | Seat decides within ~15s or hands press Next. |
| Review | 0 frames. Text only. | 0 | Settled sources: Attack Log, STATE, SESSION-LOG. |
| AFK scheduled chore | seat only reads end-state frame(s); budget set in the brief | per brief | Section 6. |

Rules of thumb (from ORCHESTRATION and HANDOFF fallbacks, adopted verbatim): ~15s decide fallback = Next; takeover only at a batch boundary; degrade to chores-only at > 2x baseline latency; every fallback firing is logged.

Efficiency is the north star, so each session's log line records: frames by role, wall time, chores done, retries/recoveries. Retries and recoveries are the hidden sink; reliability is the main lever.

## 5. Learning loop

1. Every session writes a SESSION-LOG entry (format as #14): handoff line, config, what ran, ledger, incidents including self-inflicted ones, frames by role.
2. Seat applies STATE changes only after verifying them. Hands draft.
3. Weekly (or every 5 sessions) the seat writes a short review: what failed, which fallbacks fired, usage shape. Fin audits asynchronously.
4. Lessons: procedure improvements inside a tier go to LESSONS.md under a `[Claude]` tag. Anything touching tiers/rails goes to "Proposals for JJ" and is obeyed-not-assumed until ruled.
5. Promotion: item graduation per TERRA-SCOPE graduation rule (seat decides and logs after the stated clean count). Tier promotion only through BENCHMARKS gates, ruled by Fin, gated by JJ.
6. One standing hygiene rule from my own first session: **read the pack before touching the game** (not after).

## 6. Benchmark path for the seat

- **Sonnet at the controls:** B0 (3 chore sessions, zero wrong-screen errors, balances verified) then B1 drills, exactly as written in BENCHMARKS. My session #14 is a collection data point only; it is not a counted B0 session because I did not run a full circuit and logged two navigation incidents (wall select, quit prompt). Honest count: B0 = 0/3 for Claude.
- **Haiku hands:** the supervised B0 runs inside Sonnet's session under the seat's cap. Independent (unattended) Haiku sessions need Haiku's own B0/B1 evidence, per CHARTER.
- **B2 / Series C:** unchanged and owned by whoever is cleared. A Claude seat may run Series C after B1 only if the Series C package is available to it and JJ says attacks; note the same 5-trial conditions apply (including the equipment snapshot Fin required).
- Per-item graduation uses the TERRA-SCOPE rule; per-tier gates unchanged.

## 7. AFK session shapes (Config C proposals)

Common requirements for every scheduled brief, in the folder BEFORE launch: workstream, exact chore list, stop conditions, account/model assignment, expected duration, logging path. A schedule grants no tier, no spend, no exception. A missed or failed launch is logged, never retried in a loop. JJ can cancel any schedule.

| Shape | May run | Must not | Stops on | Logs |
|---|---|---|---|---|
| **AFK-0 chore circuit** (Tier 0 only, available to a seat that has Tier 0) | Home + BB collections, Loot Cart, Gem Mine, normal obstacles with name read | Anything Tier 1+, claims, donations, upgrades | Any unknown dialog/cost, balance decrease, wrong-screen twice, latency > 2x baseline, 15 min wall | SESSION-LOG entry + STATE before/after, frames by role |
| **AFK-1 housekeeping** (needs Tier 1) | AFK-0 + queued upgrade/research start when a builder is free and PRIORITIES says so, army training, zero-choice free claims | Choice nodes, off-queue upgrades, spend conversions | Same + any choice/overflow node | Same + queue item named |
| **AFK-2 farming** (needs Tier 2; locked) | Not proposed | n/a | n/a | n/a |
| **Daily claim pass** | Daily Tasks free track zero-choice, Trader FREE item | Paid tracks, choice nodes, gem/medal items | Any price, choice, overflow | Per-claim line |

Design constraint found, not solved (assumption A3): computer-use grants require an access approval in the desktop app, so a truly unattended launch may be impossible without JJ present at session start. AFK shapes are therefore a design, not a capability, until a test shows otherwise.

## 8. Three riskiest assumptions and the cheapest test for each

- **A1: A Haiku subagent can operate the game's controls at all.** I have only used the computer-use tools from the main Sonnet session. If subagents cannot call them (or approval does not carry over), "Haiku as hands" does not exist in this harness and the seat is Sonnet-only. *Test:* one subagent task, "take a screenshot and report the visible Home balances." One frame. Pass = it returns numbers that match mine.
- **A2: Haiku's visual reads and targeting are reliable enough to save usage.** If Haiku's accuracy forces Sonnet to re-verify every step, the verification frames cost more than Sonnet doing the chores directly (the hidden-retry sink from the north star). *Test:* P1 plus a measured comparison, one chore circuit done two ways, with frames and retries counted in both.
- **A3: The scheduled/unattended path works without JJ.** Config C needs an unattended launch, the Play Games window opened, and computer-use access granted without a person. *Test:* with JJ present, schedule a 5-minute no-action session (open game, read Home, close) and see if every approval prompt can be satisfied without a human. If not, AFK means "JJ at the PC but not engaged", and the design says that plainly.

Runner-up risk, not in the top three: **Play Games window latency**. My own direct session worked, but no timings were taken. P4 will give the first.

## 9. Open items for Fin's ruling

1. Whether "Sonnet direct, Haiku idle" counts as the legitimate default seat shape until A1 resolves.
2. Whether AFK-0 may be proposed to JJ before Claude has B0 3/3, or only after.
3. CHALLENGE-INVENTORY.md tier mapping (separate file, same branch).

## Addendum A2-1 (2026-11-14, measured) — Haiku is a batch worker
- [MEASURED] A1: 1 screen read by a Haiku subagent = 71,605 tokens (SESSION-LOG #15). P1-lite: 5 saved screenshots = 71,300 tokens (#17). The ~70k cold start dominates; marginal image cost is near zero.
- Rule: a Haiku spawn must carry a circuit's worth of frames to pay for itself. Single reads stay Sonnet-direct.
- [MEASURED] P1-lite accuracy 14/15 (93%) on game fields; the miss was a currency icon (Elixir read as Dark Elixir). Standing constraint (Fin ruling): any Haiku read involving currency icons or prices is re-verified by the seat before anything acts on it, whatever P1 eventually scores.
- Still open: full P1 (10 live screens), A2 two-way circuit token count (subagent + seat), P2-P5.
