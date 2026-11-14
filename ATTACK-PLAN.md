# ATTACK-PLAN — Strategies Built For An LLM's Hands (v1.3)

**Everything in this file is a HYPOTHESIS until trial data says otherwise.** No strategy
here is "reliable" yet, and nobody promises stars. Reliability is a measured property —
it gets earned in TRIALS (TEMPLATES.md), reviewed every 5 attempts, and only then does
language in this file upgrade from "hypothesis" to "measured: X stars in Y of Z trials."

## Design constraints (why these strategies look like this)

An LLM operator is slow, deliberate, and strong at checklists; it is weak at twitch
timing, parallel tracking, and unconfirmed controls (hero abilities — B1). So every
approved strategy must have:

1. **Few decision points** (ideally: pick side -> funnel -> deploy line -> 2 spell
   moments -> cleanup). No multi-phase hero walks as the main plan until B1 ability
   control is proven — hero-walk armies (RC Walk, Queen Charge) are explicitly
   DEFERRED strategies, however strong they are for humans.
2. **Line/spam deployment** — troops go down in one or two waves along an edge, not
   drip-fed across the base. Deployment order matters more than deployment speed.
3. **Spells on triggers, not timers** ("when the line reaches the core buildings,"
   not "at 0:47"). Triggers survive slow observation; timers don't.
4. **A built-in Town Hall path** — the 2nd star comes from a planned TH kill (Blimp),
   not from hoping the line bends toward it.
5. **A surrender rule** — a lost attack ends early to save hero health and time.

## The path to reliable 2 stars (then 3) — as a program, not a promise

- **Two stars = Town Hall destroyed AND >= 50% destruction, in either order**
  (v1.3.1 wording fix — the stars are conditions, not a sequence).
- The 50% condition: the wide line + cleanup heroes is built to make 50% the *floor*
  outcome of a correctly executed attack.
- The TH condition: the Battle Blimp is dedicated to the TH from deployment — but
  **a Blimp is a delivery vehicle, not a kill.** Its crash damage alone does not
  destroy a TH17 Town Hall. The TH plan must name its PAYLOAD: inspect the Clan
  Castle troops the Blimp carries before the attack. If the payload plus planned
  spell support cannot plausibly kill the TH, the TH path is UNPROVEN: the attack
  may still run as a TH-UNPLANNED trial. Wording matters (Sol's correction,
  2026-11-14): unproven is not a one-star maximum — if the line takes the TH
  organically, the stars are recorded as they land. The label governs what the
  trial is EVIDENCE for (not a TH plan), never what results are allowed to happen. If the Blimp path is also unsafe (Sweepers/Tornado), the base is a NO-GO
  for this strategy (see BASE-TYPES) rather than a gamble.
- **Star 3** = 100%: comes later, from funnel quality + spell timing + ability control
  improving across trials. It is a Phase-3 goal, measured as a rate, never a per-attack
  expectation.
- Promotion rule: a strategy graduates "reliable 2-star" only at >= 8/10 two-star
  trials — counted PER strategy x PER venue x PER base type, never pooled across
  any of those. Campaign/practice success establishes control competence only; it
  never certifies multiplayer (PvP) reliability, which needs its own 10 trials in
  Battles. Even then, "reliable" is a measured rate, never a guarantee.

## Strategy S1 — Army v1 Line Push (PRIMARY, hypothesis)

Comp: Army of Record v1 (PLAYBOOK): 12 Dragons, 2 Dragon Riders, 6 Balloons;
4 Rage + 3 Freeze; Queen, Warden (air), Minion Prince, Royal Champion; Battle Blimp.

Script:
1. SCOUT (30-60s, no clock pressure in campaign/practice): call the base type
   (BASE-TYPES) out loud in the log draft. Pick the attack edge: the side where the
   Blimp's straight path to the TH crosses the FEWEST Air Defenses/Sweepers.
2. FUNNEL: Queen on one corner of the chosen edge, Royal Champion on the other.
   Goal is only to delete the edge buildings so the line goes IN, not around.
   Verify each hero is down before continuing (select-verify-deploy).
3. LINE: deploy Dragons + Riders in an even line along the edge, Balloons just
   behind them. Warden with the center of the line. Minion Prince with the line.
4. BLIMP: send it on the scouted path once the line is engaging defenses (so it
   isn't tanking alone). Its only job is the Town Hall.
5. SPELLS ON TRIGGERS: Rage #1 when the line meets the first dense defense cluster;
   Freeze on the Inferno Artillery or Firespitter engaging the pack; remaining Rages
   at the core; save 1 Freeze for whatever is killing the Blimp's escort late.
6. ABILITIES (only if B1-passed; otherwise let them auto-trigger): Warden at the
   core's heaviest fire; Queen when she is targeted by a point defense.
7. SURRENDER when: TH is down AND destruction clearly stalls below the next star,
   or the line is dead and cleanup cannot reach 50% — end it, log the cause.

## S1-B — Batched Line (the trial script for LLM operators, added 2026-11-14)

Written after Sol's measured profile (strengths: pre-planning, exact counts, planned
coordinates, verification; weaknesses: slow round trips, stale frames, piecemeal
sequencing, spell timing). S1's ARMY stays; its phase-by-phase choreography goes.
One variable changed: the script. Diagnosis this tests: the army was never the
problem — the number of sequential decisions was.

Rules:
- **Everything is preplanned.** Before deploying, the trial entry names: attack edge,
  both funnel corners, Blimp path, the two Freeze targets (named defenses), and the
  two Rage coordinates. Improvisation mid-attack is a logged deviation, not a tactic.
- **Batching is required, not merely allowed.** Deployments go down in preplanned
  batches (multi-click tool calls; the clickCount precedent), with a verification
  screenshot AFTER each batch — never observation pauses WITHIN one.
  - Batch 1: Queen corner A + RC corner B + first 6 Dragons along the edge.
  - Batch 2 (immediately): remaining Dragons + Riders + Balloons, Warden + Minion
    Prince with the pack's center.
  - Batch 3 (immediately): Battle Blimp on its preplanned path, trailing the pack.
    (Replaces S1's "send when the line is engaging" judgment trigger — removed
    because a slow operator cannot time it, and an untimed Blimp is a lost Blimp.)
- **Funnel risk is real (Sol's correction, accepted):** dragons DO split and ring a
  base when the funnel fails — "air troops, no pathing risk" is not claimed anywhere
  in this plan. The funnel corners in Batch 1 are load-bearing setup, and FUNNEL
  stays a first-class cause code.
- **Spell allocation — all 4 Rage + 3 Freeze assigned (no unassigned spells):**
  - Rage 1: preplanned ENTRY coordinate, fired right after Batch 3.
  - Rage 2: preplanned CORE coordinate. Gate is DOUBLE: destruction ~25% AND a
    current frame confirming the pack is at/entering the core (Sol's correction —
    a % read on a stale frame does not prove troop location). Milestone without
    confirmation = hold; it may fire later only on positive core confirmation
    while the pack is still in the core, else it is skipped for good.
  - Rage 3: preplanned TH-ZONE coordinate, same double gate (pack confirmed
    engaging the TH-area defenses). Purpose: carry pack + Blimp escort through
    the Town Hall compartment.
  - Rage 4: RESERVE. Fires only on a frame-verified cluster of >= 4 dragons (or
    dragons + riders) under defense fire outside the earlier Rage zones — the
    LARGEST such cluster, not merely a group (amended at the Series B review:
    A1 fired it on a moved group, SB-2 on a smaller group). If the pack collapses
    below a qualifying cluster, HOLDING the Rage is correct play, not a miss
    (SB-5: held all battle because no legitimate cluster survived; the trial's
    cause sits upstream in pathing, not in spell discipline).
  - Freeze 1: NAMED defense #1 (highest threat covering the entry edge), fired
    when a current frame shows the pack entering its range.
  - Freeze 2: NAMED defense #2 (the TH-zone / Blimp-path defender), same rule.
  - Freeze 3: RESERVE — the one reactive spell allowed: the defense a current
    frame shows killing the pack fastest. No clear candidate = hold.
  - Universal: a missed moment means SKIP, never a late guess. Skipped spells
    are reported per spell in the trial entry.
- **Ability policy (optional, never load-bearing) — AMENDED by the Series B
  review (2026-11-14):** the original sub-40%-health trigger is RETIRED — at that
  health the auto-trigger usually wins the race (RC and Queen both auto-fired
  before deliberate clicks in SB-3; the corrected RC record is one manual fire,
  SB-1 in the boosted stratum, and AUTO in SB-2 through SB-5). Deliberate attempts now key to CORE ENTRY for Warden and
  Minion Prince (visible effects in SB-4 and SB-5) and to ~50-60% health for the
  Queen (clean deliberate fires in SB-2 and SB-5). RC is treated as AUTO by
  default: an attempt is optional, never budgeted, never counted against the
  operator when the auto wins. Max one deliberate attempt per hero per attack.
  AUTO is logged as AUTO — not a failure, not evidence. No plan damage assumes
  an ability fires.
- **Fallback predeclared:** if FUNNEL dominates the cause codes across Series A,
  Series B tests S1-C — the same army with NO hero funnel (heroes ride the line's
  flanks in Batch 1-2). Not before, and not mid-series.

### Series A — CLOSED INCOMPLETE (2026-11-14)

Ended by JJ's direct instruction to move to real battles. Results: A1 100%/3 stars
on Besieged (stands as deployment evidence); A2 interrupted by JJ's physical
Escape mid-deployment, settled 4%/0 stars — recorded as INTERRUPTED, excluded from
all averages and criteria (not a failure, not evidence). Series A's pass criteria
are unevaluable at n=1. The S1-B script carries forward unchanged into Series B.

### Series B — Battles (opened 2026-11-14 by JJ: "just attack in real battles idc
about my rank")

Venue: regular multiplayer matchmaking (and revenge, logged as Battles) — NOT
Ranked/League sign-up, which stays Tier 3; if the game offers Ranked enrollment,
decline and report. Rank loss is accepted by JJ's explicit instruction; trophy
count is not a success metric. Script: S1-B as written (preplanned batches,
milestone + current-frame spell gates, skip-don't-guess). Per-attack: call the
base type and the GO/NO-GO checklist (BASE-TYPES) before deploying; ANTI-AIR and
META bases are skipped with Next (a skipped base is a decision, logged as such).
Army retrain cost per attack is normal farming cost.
Predeclared: 5 Battles trials (labeled SB-1..SB-5, to keep Benchmark B1 distinct);
pass = B2's bar in this venue (>= 70% average destruction, >= 3 trials at 2+
stars). A1's campaign result does NOT transfer across venues — Series B starts
at 0/5. COMPARABILITY RULE: the script assigns exactly 4 Rage + 3 Freeze; a trial
that also fires donated CC spells runs a bigger budget and is annotated
"CC spells used — not spell-comparable." Series conclusions about S1-B are drawn
from own-spells-only trials wherever possible. Every trial records the base's
class honestly (a 100% vs a soft RUSHED-class base is weaker evidence than 70%
vs a solid TH17, and the log must make that visible).

### Series B REVIEW (2026-11-14) — pass arithmetic vs qualification

Results: SB-1 100/3 (boosted, CC spells) · SB-2 100/3 · SB-3 74/2 · SB-4 59/2 ·
SB-5 36/0 (TH standing). Full set: 73.8% avg, 4/5 at 2+ stars, 2/5 at 3 stars —
the numeric bar (>= 70% avg, >= 3 at 2+) is MET on the mixed set.
**Qualification: B2 is NOT passed and Tier 2 farming is NOT unlocked.** The full
set is a mixed stratum (one boosted trial that also spent CC spells). The
operative stratum — unboosted, own spells only, SB-2..SB-5 — is n=4 at 67.25%
avg (3/4 at 2+, 1/4 at 3), BELOW the 70% average and short of five trials. A
headline average assembled from unlike conditions is exactly the statistical
stretch this system exists to refuse. S1-B (no-siege, "S1-B0") remains the
standing script, status PROVISIONAL.

Cause review across five trials (precision fixes by Sol, accepted 2026-11-14):
deployment is DEMONSTRATED at 13-18s windows (mean 14.706s, one recovered miss
in five trials, zero aborts) — demonstrated under these conditions, not
universally solved. Spell gates mostly worked (named Freeze targets hit; two
reserve-Rage placement lessons absorbed into the Rage 4 rule above), with one
explicit deviation: in SB-5 a core Rage was cast BEFORE its ~25% milestone —
spell execution was not exact in that trial. Abilities: mechanism reliable;
the RC record is corrected to one manual fire (SB-1, boosted stratum) and AUTO
in SB-2, SB-3, SB-4, and SB-5 (no late manual clicks in SB-4/SB-5). **The
binding constraint is now pathing: the dominant failure is the line splitting
or peeling against compartment/central-TH bases (SB-5 the pure case: heroes
NW, small center force, pack collapsed under dense core defenses, TH standing)
— ability execution cannot rescue bad pathing, and no spell rule fixes
geometry.** Base-class honesty mattered: the two 100% results came against the
softest bases and results declined as bases hardened (74 / 59 / 36) — an
uncontrolled trend that SUGGESTS base hardness drove the decline; it does not
prove the cause.

### Series C — PREDECLARED (the B2 attempt series; a PACKAGE comparison)

Honest framing (Sol's correction, accepted): Series C changes geometry AND
adopts the amended ability policy AND the Rage 4 largest-cluster gate together.
It is therefore a package comparison — S1-B Narrow package vs the Series B
record — and its results support conclusions about the PACKAGE, never causal
claims about geometry alone.

Script: **S1-B Narrow package**, exact geometry (Sol's spec, confirmed —
it resolves a contradiction in the first draft, which put Q/RC both at the
corners and at the center): pick an entry segment spanning ~60% of one edge.
Queen and Royal Champion deploy at the OUTER CORNERS OF THAT SEGMENT as the
funnel pair and STAY wide — they are not redeployed to the center. Dragons go
down in two groups of 6 and 6 (12 total — Army of Record v1) across the
segment's span; Dragon Riders,
Balloons, Warden (air), and Minion Prince deploy at the CENTER, immediately
behind the line. All seven spells keep their Series B jobs; the amended
ability policy (core-entry W/MP, ~50-60% Queen, RC auto-by-default) and the
Rage 4 >= 4-largest-cluster gate apply as written above.
Selection refinements: record TH position and entry side relative to it; on
central-TH bases prefer a TH-side entry segment (hypothesis from SB-4 vs
SB-5, n=2 — weak evidence, tested here); count Air Sweepers covering the
entry — if two sweepers face the chosen segment, RE-PICK the entry segment
(or NO-GO). A strong central-ring base may be attacked deliberately and
labeled a STRETCH test in its trial entry. Never assume low walls = safe:
walls were not the variable that hurt in Series B; core density and pathing
were.
Conditions: 5 eligible Battles trials — unboosted, own spells only, no CC
troops/spells, no siege; stable equipment, pets, and readiness across the
series (any change voids comparability and is logged); every trial logged
with base class, TH position, sweeper note, and ALL failures included.
**Pass = the B2 bar on this clean set (>= 70% avg, >= 3 at 2+ stars), and a
pass here is a B2 pass** — Tier 2 farming unlocks on it. Language discipline:
even a pass earns only "B2 passed." A "reliable 2-star" claim additionally
requires a comparable 10-trial window at >= 8 of 10 two-star results.
Review splits strata as always.

### Series D — QUEUED, BLOCKED on inspections (supported TH path)

A Blimp-delivered TH plan stays untestable until: (1) CC contents read directly
in-game (still UNVERIFIED), (2) Workshop checked — is an own Battle Blimp
available or locked, and behind what, (3) JJ rules on requesting a TH-kill CC
payload from the clan. No free-Blimp assumption is made anywhere until (2)
answers. Also still owed from general play: the full live [CHECK] sweep and a
Pet House read to settle pet levels finally.

### Series A — predeclared 5-trial script validation (campaign, fixed base)

Venue: a late single-player campaign map, chosen by the operator and NAMED in the
log before Trial 1, then FIXED for all 5 trials (same base = variance measures the
operator, not the base). CONSTRAINT (2026-11-14): the map must NOT be ANTI-AIR or
META class per BASE-TYPES — the hardest map (Dragon's Lair) is a specialized
anti-air layout and would measure the matchup, not the operator; it is a later
stretch test, not the Series A venue. Army: Army of Record v1 exactly; CC/Blimp
payload inspected and recorded in STATE before Trial 1. Trial entries also record
hero BOOST status (a live boost puts effective levels at cap; results earned
under a boost are labeled as such and expectations re-baseline when it expires).

NO-TH-MECHANISM RULE: if the account has no own Battle Blimp and no plausible
TH-kill CC payload, Series A runs as a DEPLOYMENT series — no siege machine, and
pass criterion (4) is replaced by ">= 3 of 5 trials at >= 70% destruction." The
series then validates line execution only; two-star capability remains UNTESTED
(not failed) until a TH mechanism exists. Donated siege machines are finite and
are never consumed just to force matched trials.

Per-trial metrics (added to the trial entry): deployment window (tool calls from
first troop to last troop), input misses, spells on-plan vs improvised vs skipped,
deliberate ability attempts/fired, stars/%, TH taken, cause code.

**Series A passes (script validated) if ALL hold:** (1) zero input-caused aborts;
(2) input misses <= 1 per trial from Trial 3 on; (3) avg destruction of Trials 3-5
> avg of Trials 1-2 (learning is visible) — CEILING CASE: if Trials 3-5 average
>= 95%, equality with Trials 1-2 also passes (a series parked at the ceiling
cannot fail for failing to exceed it); the destruction trend is reported in the
review either way, separately from the pass/fail; (4) >= 2 of 5 trials reach 2 stars.
What a pass means — and only this: the S1-B script is executable by this operator
on this campaign base. It contributes campaign evidence toward B2 (whose own bar
stands: 5 own-army attacks, >= 70% avg, >= 3 at 2+ stars). It says NOTHING about
TH17 PvP reliability; Battles need their own trials under the venue rule.

## Strategy S2 — Hydra Group Push (RESEARCH-ONLY — not an exact army yet)

Status v1.3.1: S2 has no finalized composition/script in this pack. It is a research
direction, not a runnable strategy: do not trial it, do not switch to it during B2,
and never pool its results with S1's. It becomes runnable only via a written amendment
adding its exact comp + script.

From the library's Hydra sections [community]: same family as S1 but the whole army
deploys GROUPED on one flank (not spread), heroes funnel both sides of that flank,
Rage + Warden ability at the core. Punished by centralized Air Defenses covered by
Wizard Towers — see BASE-TYPES go/no-go. Trial only after S1 has 5+ logged trials.

## Strategy S3 — Electro Dragon Compact-Base Play (RESEARCH-ONLY — not an exact army yet)

Status v1.3.1: same rule as S2 — no finalized comp/script, Electro Dragon levels on
this account unverified. Research direction only until an amendment makes it exact.

Library verdict: mass Electro Dragons have fallen at TH17 EXCEPT against compact
bases (buildings ~1 tile apart, where the chain works). Only vs a called COMPACT base
(BASE-TYPES): narrow hero funnel, 4-6 Electro Dragons into the lane (not a full-edge
line), Rage placed AHEAD of them, Freeze saved for the Air Sweeper facing the path
and any Firespitter in the lane. Requires Electro Dragon levels from the Lab queue —
check STATE before assuming availability. Never vs spread bases.

## Deferred (human-strong, LLM-hostile — do not trial yet)

- RC Walk / Queen Charge anything (ability + pathing + invisibility timing).
- Fireball Warden walks. Multi-phase ground (Root Rider funnels with hero walks).
- Anything whose plan contains the words "precisely when."

## Trial discipline (feeds BENCHMARKS B2/B3)

- Every attack gets a TRIAL entry (TEMPLATES.md) with the base type called BEFORE
  deploying. A strategy's record is per base type — S1 vs RING bases is a different
  claim from S1 vs DEAD bases.
- After every 5 trials of a strategy: review — keep, amend (one variable at a time),
  or shelve. Amendments cite trial numbers.
- Farming (Tier 2, when earned) uses S1 on DEAD/COLLECTOR bases first (BASE-TYPES) —
  the easiest real-venue reps — before any live-base attempts.
