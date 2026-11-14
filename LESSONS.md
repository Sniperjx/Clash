# LESSONS — What The Game Taught Us

Entry format:
`## YYYY-MM-DD — [Agent] Short title`
then: **Observed:** what happened · **Evidence:** session-log # / numbers · **Rule:** what we do differently now.

A rule needs two observations, or one undeniable failure. Rules that fail twice get
demoted here with a strike-through and a note. This file is the system's actual brain —
keep it honest and current.

---

## 2026-11-14 — [GPT] Collecting is reliable; verify by balance, not by animation
**Observed:** Resource collection worked across two sessions; balances rose verifiably
(gold +~1.75M in one session; Loot Cart +1.8M G / +1.8M E / +18k DE).
**Evidence:** JJ-relayed session reports, 2026-11-14.
**Rule:** Collect boldly at Tier 0, but always confirm success by the balance change or
result state — never by the tap animation alone.

## 2026-11-14 — [GPT] Select-and-deploy in one motion misses inputs
**Observed:** Selecting a troop and immediately tapping the drop point sometimes didn't
register; deliberate select -> verify -> deploy worked (bulk drops of 5 Healers, 10 Hogs,
11 Miners all succeeded).
**Evidence:** GPT control tests, 2026-11-14.
**Rule:** Universal technique in PLAYBOOK.md. Speed is earned later; accuracy first.

## 2026-11-14 — [GPT] A lone hero dies; support is not optional
**Observed:** Practice attack ended 31%, 0 stars; the Queen was deployed without support
and died before the army engaged.
**Evidence:** GPT practice test, 2026-11-14.
**Rule:** Never deploy a hero without its support already committed or deploying with it.

## 2026-11-14 — [GPT] Hero ability activation is unconfirmed
**Observed:** Ability controls were attempted but successful manual activation could
never be confirmed on the result state.
**Evidence:** GPT control tests, 2026-11-14.
**Rule:** Treat ability timing as an open skill gap (Benchmark B1 drill) — plan attacks
that don't hinge on a perfectly timed ability until B1 passes.

## 2026-11-14 — [GPT] Spell timing lags the army
**Observed:** A Freeze was placed successfully (mechanics work) but tactical timing was poor.
**Evidence:** GPT practice test, 2026-11-14.
**Rule:** Spells go down as troops reach the target cluster, never pre-emptively on an
empty area. Drill in practice before farming.

---

## Proposals for JJ (rails changes, tier-3 asks — JJ rules, Fin relays)

(none yet)

## 2026-11-14 - [GPT/Codex] Camera and collection findings
Observed in session #6: native drag did not usefully pan. Zoom in at the desired lower area then out at the upper area moved the viewport and exposed the boat. One collection bubble per resource type cleared the other visible same-type bubbles in both villages; balances verified the collection. Gem Mine added19, a normal Trunk cost1000 BB elixir and yielded6 gems after disappearing. Use fresh screenshots, verified balances and explicit obstacle labels; never infer an event obstacle is safe. Hotkeys read in the controls panel are mappings only, not demonstrated ability activation.

##2026-11-14 [GPT/Codex] Control evidence #7
Queen portrait re-click can activate ability; proved once with grey portrait, substantial health and effect visible. This is a mechanism observation, not timing reliability.10Hog clickCount deploy succeeded. First siege drop rejected red zone; use clearly legal outer tile. Spell count reduction proves consumption, not effect timing. Re-observe menu animations before retry: stale immediate screenshots can hide a completed action. No claimed combat reliability from55%/1star drill.


## #11 current combat lessons
Batched native inputs deployed all troops/four heroes in16.981s campaign and13.019s/13.279s live,zeroobserveddeploymentmisses in these complete deployments. This improves execution, not proof against solid TH17. Scouting must distinguish TownHall from Eagle; SB1 entry planning misidentified them. RCauto already fired before SB2 manualattempt (explicit used-already message);manualtimingcannot be assumed. Boost expired naturally beforeSB2,so boosted and unboosted results remain separate;noitemused. Pet levels from boosted result are effective,not reliableownedlevels.

## #11 practical attack lessons - current
- Batching demonstrated all troops/four heroes deployed in13.019-18.231s over five real battles,one recovered rejectedRCpoint. Mechanism works; input accuracy is not universal perfection.
- Locate TH separately from Eagle. SB1 misidentification recovered on a soft base; don't rely on that recovery. Low walls do not establish low air-defense risk.
- Mainforce splitting/attrition now dominates:74%,59% afterTH;36% withTHstanding on centralring. Ability mechanism cannot rescue every poor path. Opponent variation prevents proving a single causal explanation.
- Warden/MP core-entry attempts beat latehealth clicks in observed examples. RC usuallyAUTO;Queen sometimesmanual. No load-bearing preciseabilitytiming. Earlier50-60%Queen policy remains hypothesis.
- Rage needs CURRENT occupied group,largestgroup for reserve;oneframecounts lag. SB5 coreRage before25% was deviation. ThreeRagesused/oneheld aftercollapse is honestly reported,not exactscript execution or proof no earlier opportunity existed.
- Unboosted result petsUnicorn10/Frosty3/Owl8;directownedcheckpending. Army-screen8/3/10 read withdrawn. SB3 AttackLog RC45 supersedes mistaken50 resultread,causeunknown.
- Overall4/5two+ is mixedconditions;unboosted ownspells3/4 at67.25%avg. No reliabletwo-star/B2promotion. Recheck everyfive and preserveallfailures.
