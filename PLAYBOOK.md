# PLAYBOOK — How To Do Each Thing

Technique here comes from GPT's 2026-11-14 control tests (what actually worked on this
PC + this game client) plus Fin's research library. When you discover better technique,
update this file and cite the LESSONS entry that proved it.

## Universal input technique (learned the hard way, 2026-11-14)

- **Select -> pause -> verify -> deploy.** GPT's missed inputs came from selecting a troop
  and deploying in the same motion. Tap the troop, take a fresh look, confirm it's
  selected, then tap the drop point.
- **Animations lie.** After any action, wait for the animation to finish and re-observe
  the screen before concluding what happened. Balances and result screens are truth;
  mid-animation screens are not.
- **Confirm on the result screen.** Whether a spell was consumed, a siege deployed, or a
  hero ability fired is only known from the post-action/result state — check it and log it.
- **One hero is not an army.** The 31% practice attack died because the Queen went in
  alone and unsupported. Never deploy a hero without its support plan (see Attacking).

## Chores (Tier 0)

- **Collecting:** tap each mine/collector/drill with a visible full bubble; then check
  the balance actually rose. Loot Cart: collect whenever present — it was worth
  1.8M/1.8M/18k in the seed session. Builder Base collectors too.
- **Obstacles:** remove ONLY normal vegetation (trees, bushes, stumps, mushrooms) and
  Gem Boxes. **NEVER clear event obstacles** — anniversary, holiday, seasonal, or
  anything decorated/unique (JJ's emphasized rule; CHARTER rails). Work a rough circuit
  of the base so none hide behind buildings; re-check after camera moves. Doubt = leave it.
- **Order of operations for a chore session:** Loot Cart -> home collectors -> obstacles ->
  Builder Base collectors -> update STATE.md.

## Housekeeping (Tier 1)

- **Starting an upgrade:** open the building, confirm the item is on PRIORITIES.md,
  confirm cost <= balance with a sensible reserve left, start it, then immediately log
  what finishes when (building, level, duration) and write it into STATE.md's builder table.
- **Lab research:** same discipline — queue items per PRIORITIES Tier C; log finish time.
- **Donations:** only when a request is visible in clan chat and names (or clearly shows)
  the troop. Donate exactly what's asked. If the request is ambiguous, skip it and log why.
  (GPT reached clan chat fine but found no open request — unproven, hence Tier 1 gating.)
- **Armies:** the army of record is AIR. Don't redesign the saved army casually; changes
  go in the log with the reason, and attack benchmarks use the army of record.

### Army of Record v1 (exact composition — added v1.1)

Fits JJ's 320 housing / 11 spell space. Derived by Muse from the research library's
TH17 Dragons/Hydra sections [community sources]; it is a STARTING composition — practice
logs may amend it (that's the learning loop working, not disobedience).

- **Troops (320):** 12 Dragons (240) + 2 Dragon Riders (50) + 6 Balloons (30)
- **Spells (11):** 4 Rage (8) + 3 Freeze (3)
- **Heroes:** Archer Queen, Grand Warden (set to AIR), Minion Prince, Royal Champion
- **Siege:** Battle Blimp (Stone Slammer acceptable if Blimp unavailable)
- **Clan Castle:** whatever air troops + Rage are donated/available; never delay an
  attempt solely for CC — note in the log whether CC was filled.
- **Shape:** heroes + a few Balloons/Dragons cut the funnel on both edges; main line of
  Dragons/Riders through the middle with the Warden; Rage on the densest defense
  cluster as the line arrives; Freeze the Inferno Artillery / strongest air-targeting
  defense engaging the pack; Blimp toward the Town Hall / core.

## Attacking (Tier 1 practice -> Tier 2 farming)

Current honest level: **poor** (GPT seed test: 31%, 0 stars, Practice). The path up:

1. Practice stages are B1 control drills only (preset armies); B2 attempts use the army of record in eligible venues (campaign maps / pre-existing Friendly Challenges). Tier 1 is required.
2. **Attack shape (air):** scout the base -> pick the side where air defenses/queen are
   weakest -> funnel with heroes + a few Balloons/Dragons on the edges -> main force in a line, not a
   clump -> spells on the densest defense cluster, timed as troops arrive, not before ->
   heroes with the main force or cleaning the far side, abilities when health drops
   (ability activation is UNCONFIRMED as reliable — practice it as its own drill, B1).
3. **Deploy in waves, verifying selection between waves** (universal technique above).
   Bulk deployment works when done deliberately (5 Healers / 10 Hogs / 11 Miners all
   succeeded in seed tests when not rushed).
4. **After every attack:** log stars, %, army used, what died first and why, which inputs
   missed. An attack without a written cause of failure teaches nothing.
5. **Farming (Tier 2, once earned):** loot first, stars second; target dead/full-collector
   bases; surrender once the loot is taken or the attack is clearly lost — don't burn
   hero health and spells on a dead attack.

## What "good" looks like (targets)

- Chores: zero missed collectors, balances verified, < 10 min.
- Practice: consistent 2–3 stars on level-appropriate practice bases (gate B2).
- Farming: positive loot per attack after army cost, heroes rarely left at 0 HP.

## Verified control lessons - Fin audit, 2026-11-14, #10

- Verify troop identity from selection, visible deployment and the result screen before recording it. #10 initially mislabeled Electro Dragon as Ice Golem in tool titles; the result corrected this. Troop visual identification is a tracked skill.
- Manual ability activation mechanism is proven on two heroes: Queen in #7 and Warden in #10. Timing reliability remains unproven. Queen's automatic low-health activation in #10 adds no manual evidence.
- Slow, piecemeal support remains a combat failure. The 54%, one-star preset Practice result is a baseline, not improvement or B2 credit. Verify legal placement and selection, then coordinate support; re-observe when transitions make the frame stale.
- Future model comparisons require labeled, comparable trials and measured time. The Terra-to-Sol handoff alone proves neither a speed advantage nor usage savings.

## Current attacking procedure - #11 closeout
Use the CURRENT ATTACK RUNBOOK at the top of ATTACK-PLAN.md, not the historical line/Blimp script above. JJ authorizes regular Battles;no Ranked/BuilderPvP. S1-B0 baseline completedfive withmixedconditions,unboostedsubset67.25% andnoB2pass. NextS1-BNarrow isproposedpackage,notstarted. Portraitbatchinputworks;THidentification,currentspelloccupancy,legalboundaries andfreshsettledcounts remainmandatory. No assumedfilledCC orTHkillfromBlimp;inspectdirectlybeforeanysupportedvariant. All12Dragons=6+6. See datedATTACK-REVIEW forfailures/metrics.

## Scout-seat lessons - 2026-11-16
- Treasury is NOT a map building. Route: tap Clan Castle -> Treasury button in its menu -> read -> Collect -> Okay. Verify a builder is free BEFORE collecting.
- Deploying: wait out the countdown (~35 s), scroll the wheel down 10-20 ticks to zoom out, deploy from open grass with no cannons or walls (here the RIGHT edge; left/top-left edges gave red-area misses). Heroes first, Dragons clustered, then Riders/Balloons/MP; Rage on the path to the TH; Freeze on the named engaging threat.
- Priority-check before any currency-competing spend; state the priority item's status in the log first.
- Builder panel has no Lab tab. If a Confirm returns the Goblin Builder "all builders busy" dialog, close it, never pay.
- Idle disconnect ("Anyone there?") happens after a long pause: tap RELOAD GAME, then zoom out again.
- Scroll picker lists from empty margins, no batched clicks across popovers, never press Upgrade on a map selection unless intended.
- Lab location is still unknown on this layout: it is not in the left, top or right outside areas; hunt inside the walls only with read-the-label taps.
