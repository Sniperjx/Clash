# PRIORITIES — Upgrade Queue v2 (Fin ruling, 2026-11-14)

**Status: ADOPTED.** This file replaces PRIORITIES v1 in full. Drafted by Fin research
agent (~/workspace/clash-army-research/05-upgrade-plan-draft.md), verified on its
load-bearing claims by Fin (camp arithmetic 4x80=320; Blacksmith caps confirmed in
library 03: Common 18 at BS7, Epic 27 at BS9, BS10 raises no caps), and ruled the
standing queue under JJ's 2026-11-14 mandate (Fin + seats own upgrade decisions and
execution; JJ plays freely alongside).

**Fin amendments on adoption:** (1) No attack-set hero (Q/W/MP/RC) starts an upgrade
during a declared trial block (Series C included) — the rotation pauses for blocks.
(2) Every start is verified in-game at start time for cost/currency before confirming;
any figure in this file labeled [not retrieved] or [library] is a ceiling, not a price.

## VERIFIED PRICES — post-Jam (Fin, 2026-11-18; these SUPERSEDE the labeled estimates below wherever they conflict)
Menu- or Lab-screen-verified in game: Army Camp ->13 = 14,500,000 E / 7d. Dragon 11->12 = 15,500,000 E. Balloon 11->12 = 15,500,000 E. Baby Dragon 10->11 = 15,000,000 E. Ricochet Cannon merge = 12,000,000 G / 7d. Phoenix 2->3 = 95,000 DE / 2d. Dragon Duke ->8 = 110,000 DE / 2d. Angry Jelly 1->2 = 150,000 DE / 3d. Top hero levels ~340,000 DE each. The Hammer Jam ended 2026-11-16 00:00 PT; the old x2 post-Jam heuristic is retired — where a price is still unverified (Firespitter #2 above all), read the menu at the start, never the heuristic. Firespitter #2 = 17,000,000 G / 10d (menu, 2026-11-18 #38 — the gold track's target number; gold on hand 13.13M at the read). Merge prices ESCALATE: Ricochet merge #2 = 17.5M G (the first was 12M, #35), Multi-Archer merge #3 = 17.5M G, Multi-Gear Tower L2 = 18M G, Spell Tower upgrade = 17M G, Giga Bomb = 12.5M G / 5d, Squad Barracks = 1.7M E / 2d.
(3) Walls remain overflow-only (free builder + surplus), never a queued start.
(4) The Crafting Station stays rejected until its TH17 status is verified in-game
AND DE is no longer the scarcest currency.

---

# 05 — Upgrade Priority Plan (DRAFT for Fin's ruling)

**Date:** 2026-11-14 · **Account:** TH17, SNIPERJX12, clan Boysenberry — 6 builders, Lab 15,
Pet House 10, Blacksmith 9, Barracks 18. **Play pattern this plan serves:** an AI-run air-army
attack program (Army of Record v1 / Hydra candidate, heroes Queen + Warden-air + Minion Prince
+ Royal Champion) plus the owner playing himself.

**This plan REVISES `clash-repo/PRIORITIES.md`.** Every change from the old queue is flagged
with the reason. Nothing here starts an upgrade — it is a sequencing document for Fin's ruling.

## Source-quality key (nothing in this file is better than its label)

- **[repo — live-checked]** = a price/timer actually read in-game and recorded in
  `clash-repo/STATE.md` / `SESSION-LOG.md`. Strongest numbers in this file.
- **[snapshot — provisional]** = GPT-reported account level, never independently verified.
- **[library — snippet-only]** = research-library figure from wiki/database snippets, not an
  opened primary page. ⚠️ Several of these predate the Nov 2025 / Apr 2026 cost-and-time cuts
  and are demonstrably stale where a repo live-checked number exists (see §3) — where the two
  disagree, **the repo number governs** and the library figure is shown only as an upper bound.
- **[inference]** = my reasoning from labelled inputs. **[not retrieved]** = the library
  doesn't have it; verify in-game before spending.

## Starting position (2026-11-14 afternoon, per STATE.md top block)

- Balances after JJ's spending spree: **Gold 269,407 / Elixir 3,212,267 / DE 44,393 /
  Gems 2,854** [repo — JJ screenshot via Scout log #26]. Gold is effectively empty; elixir is
  low; DE is low. Treasury contents unknown (2.2M G / 2.2M E / 11k DE last read, not touched
  by Scout — JJ may or may not have drawn on it since).
- **All 6 builders busy:** Archer Tower (2h29m left), Giant Bomb (5h59m), Dragon Duke
  (23h59m), Multi-Gear Tower (~3d23h), Firespitter #1 (~4d5h), Clan Castle (~4d23h) [repo].
- **Pet House busy:** Phoenix 1→2 finishes ~2026-11-15 03:33 PT [repo].
- **Lab:** idle at last verified read [repo, #23 — indicator only]. An idle Lab is the single
  most expensive waste at TH17; see §2.
- Heroes [snapshot]: BK 95, AQ 95, GW 70, RC 45, MP 70, Duke 6 vs TH17 caps
  100 / 100 / 75 / 50 / 90 / 20.
- Army capacity **320** vs TH17 max **340** (§1). Army of Record levels [repo — live-observed]:
  Dragon 11 (cap 12), Dragon Rider 5 (AT CAP), Balloon 11 (cap 12), Rage 6 (cap), Freeze 7 (cap).

---

## 1. Army Camps — YES, this is the #1 structural priority

**Where they are:** 320 total housing ÷ 4 camps = 80 per camp. The per-camp housing cap below
L13 is 80, so all four camps must be exactly **L12** [calculated from repo/snapshot figures].
No camp can be above 80 without being L13 (85). Camp levels should still be eyeballed in the
§3-inspection pass, but the arithmetic leaves no other combination.

**What L13 takes:** **17,000,000 Elixir / 7d 12h per camp** → 85 housing each, 340 total
[library — snippet-only, 2 sources: wiki via `05-upgrade-priority-th17`, agreeing in both
library priority files; cost/time already reflect the Nov 2025 + Apr 2026 cuts per the same
sources]. **All four: 68,000,000 Elixir and 30 builder-days** if run strictly one at a time;
~15 builder-days of wall-clock if two builders run camps in parallel.

**Why it outranks everything else structural:**
- Every army decision in this project is currently made at 320. The meta comps in
  `01-meta-armies.md` are published at 340; the shortlist ruling (`04`) had to shrink all of
  them. 340 doesn't just add "a troop" — at Dragon cost (20 housing) it is exactly **+1 Dragon**,
  or +4 Balloons, or +2 Dragon Riders in every single attack, in every series, forever.
- It is the only upgrade that makes the *attack program itself* stronger without touching
  operator skill — and operator pathing, not raw stats, is the measured constraint, so free
  housing is pure margin for error (more mass = more forgiving line, cf. `02-ai-usability.md`).
- It is elixir-denominated, which matters for §6: camps compete with the Lab and Warden, not
  with the DE economy that heroes/pets are starving on.

**The honest counterweight:** 68M elixir is roughly 21× the current elixir balance. Camps are
the #1 priority *for builder allocation over the next month*, not a thing that can be bought
this week. The sequence in §7 therefore interleaves: a camp starts whenever (a) a builder is
free AND (b) elixir ≥ 17M — and until (b) is true, free builders take the cheaper gold/DE
items below rather than idling. **Revision vs old queue:** Army Camps did not appear in
`PRIORITIES.md` at all — the old queue never named the account's single biggest offensive
gap. They now sit at the top of Tier A.

---

## 2. Lab sequencing — never idle, air-army first

The Lab is one slot and TH17 research times run 5–14 days; lifetime Lab throughput, not
resources, is the long-run constraint. Rule zero, carried from the old queue and kept:
**the Lab never sits idle.** If the intended research is unaffordable the day the Lab frees,
start the best affordable army-relevant item instead of waiting — an idle day is gone forever,
a suboptimal research is merely suboptimal.

**Lab order (serves Army of Record v1 → Hydra → the deferred candidates, in that order):**

| # | Research | Cost / time | Why here |
|---|---|---|---|
| L1 | **Dragon 11 → 12** | Cost **[not retrieved]** — expect the same band as Balloon 12, ~8.75M E [inference]; time **[not retrieved]**, ~5–6d band [inference] | 12 of the 20 air slots in v1 and 9 in Hydra. The main troop at cap removes the last level asterisk on the proven army. Verify the real price in-game before starting. |
| L2 | **Balloon 11 → 12** | **8,750,000 E / 5d 12h** [repo — live-checked] | The other −1 in the proven army (6 in v1, 3 in Hydra). Price is certain because Sol read it in the menu. |
| L3 | **Baby Dragon 10 → 11** | [not retrieved] | Cleanup-variant troop (preset #3 in `04`); −1 vs cap. Cheap insurance for the farming preset. |
| L4 | **Electro Dragon → cap 8** — only if inspection shows it below cap AND the compact-base specialist preset (held item #4 in `04`) is adopted | Current level **[unreported]** | Conditional. Do not spend Lab days on a specialist until the inspection certifies the gap and Fin adopts the preset. |
| L5 | Deferred-candidate support, in this order, **only as Fin promotes each candidate**: Overgrowth (cap 4 at TH17 [library — CONFLICTS-resolved]) + Root Rider (cap 3, level unreported) if Root Rider smash is promoted; Haste + Lava Hound (cap 7, unreported) if LavaLoon is ever un-deferred (currently avoid-listed for AI) | [not retrieved] | Lab follows the army program; it does not speculate. No Lab time on ground-smash, Queen Charge, or Duke packages while they sit on the deferred/avoid lists in `04`. |
| — | **Sky Wagon: do NOT research past L2** | — | Standing repo instruction (unresolved cap conflict). Unchanged. |

**While buildings/heroes compete:** the Lab's elixir appetite (L1+L2 ≈ 17.5M E) directly
competes with Army Camps (17M each) and the Warden (elixir hero). §7 resolves this by
*staggering*, not by starving the Lab: the Lab starts L1 as soon as elixir allows, and camps
take the *next* elixir, because a camp's 7d12h builder-time and the Lab's research run in
parallel on different slots — the real contention is only the elixir pool, and farming income
(the attack program itself + JJ's play) refills it. If elixir forces a choice on a given day:
**Lab first** (its queue is longer and its slot scarcer), camp next builder.

---

## 3. Hero scheduling — one attack hero down at a time, Duke is the free chain

**The problem in numbers:** 44 hero levels remain (BK 5, AQ 5, GW 5, RC 5, MP 20, Duke 14).
Per-level costs [library — snippet-only, alviran/database]: BK/AQ 96–100 ≈ 340–380k DE;
MP 81–90 ≈ 290–380k DE; GW 71–75 ≈ 20.5–22.5M E; Duke 16–20 ≈ 275–375k DE; RC 46–50
**[not found]**. ⚠️ **These figures are stale where live data exists:** the library snippet says
8d per top-end level, but the repo's live-checked Warden 71 is **10,250,000 E / 4d**
[repo — live-checked] — roughly *half* the snippet's cost and time — and the Dragon Duke
upgrade JJ started today shows ~24h remaining for a low level [repo]. The Nov 2025/Apr 2026
cuts hit hero prices hard. **Treat all snippet hero numbers as upper bounds; read the real
price in-game at each start.** Even at half price, the DE total for the four DE heroes is in
the millions — DE income, not builder time, will pace this section.

**The rotation (the rule that matters):**

1. **At most ONE of Queen / Warden / Minion Prince / RC is upgrading at any moment.**
   The attack program fields all four; a second one down degrades every trial and pollutes
   series data (Series C conditions already require all four up — a hero mid-upgrade during
   a trial block voids comparability).
2. **Dragon Duke is the standing second hero chain.** He is *not* in the attack hero set,
   so his builder is never in contention with rule 1: whenever DE and a builder allow, the
   Duke chain runs continuously in parallel. His 14 levels are the account's cheapest
   "always-progressing" hero project, and every level also builds toward the Duke armies
   currently blocked in `04` (they need Duke ~20 + Rocket Backpack 24+ — a long road that
   only gets shorter if the chain starts now and never stops).
3. **Barbarian King is the flex slot.** Also not in the air attack set. When a third builder
   is free and DE allows, King levels proceed; when builders tighten, King pauses before
   anything in the attack set does. (His Spiky Ball 27 is the account's best equipment —
   King levels are not wasted, they are just not urgent for *this* program.)
4. **Order within the attack set:** **Warden first** (elixir-denominated — he spends the
   currency the DE heroes don't, and Eternal Tome value scales every attack), then
   **Queen** (95→100 closes the biggest per-level DPS gap in the comp), then **RC**
   (45→50, and her Electro Boots package is core to the deferred RC plays), then
   **Minion Prince as the chip project**: 20 levels is ~3–5 months of intermittent chain
   time; run MP levels in the gaps *between* trial blocks (declared series weeks are
   MP-upgrade-free), never during one.
5. **Scheduling mechanics:** start an attack-set hero upgrade only (a) outside a declared
   trial/attack block, and (b) when the DE/elixir for the *next* rotation step is already
   banked or clearly inbound — a hero upgrade that strands the Pet House (§5) without DE
   for a week is a net loss. Heroes also pause entirely during any week JJ designates for
   ranked/war play of his own, at his word.

**Revision vs old queue:** `PRIORITIES.md` Tier B said "keep one hero upgrading when DE
allows; Queen/Warden first" — directionally right, but it had no protection for the attack
set, no Duke/King parallel chains, and no trial-block blackout. The rotation above replaces it.

---

## 4. Buildings after the current six — defenses and utility order

Current six finish in this order: Archer Tower (~today), Giant Bomb (~today), Dragon Duke
(~Nov 15), Multi-Gear Tower (~Nov 18), Firespitter #1 (~Nov 18–19), Clan Castle (~Nov 19)
[repo timers]. What those builders take next, in order:

1. **Firespitter #2 — build: 8,500,000 G / 4d 6h** [repo — live-checked menu price].
   The second of the pair; TH17 cap is L2 each, so after building, one L2 upgrade per
   Firespitter remains (cost [not retrieved]). A base with one Firespitter has a soft side —
   the pair completes the TH17 defensive identity. **Gold-gated:** needs gold to rebuild
   from 269k to 8.5M first (§6). First gold builder-start once affordable.
2. **Remaining merges.** TH17 allows **3× Multi-Archer Tower, 3× Ricochet Cannon,
   1× Multi-Gear Tower** [library — opened wiki tables]. Multi-Gear is in progress now.
   Ricochet merge: **6,000,000 G / 3d 12h** [repo — live-checked]. Multi-Archer #3 cost
   **[not retrieved]**. Exactly which of the 3rd Multi-Archer / 3rd Ricochet remain undone on
   this account is unverified — the repo queue listed the Ricochet price as available, so at
   least that one remains. Merges outrank ordinary defense levels because they are permanent,
   they are one-time (once done, done forever), and the full merge set **gates TH18** later
   [library — opened]. Order between them: whichever the game offers first; Ricochet first
   if both, on the strength of its known price.
3. **Multi-Gear Tower L2 / Firespitter L2s** — after the merges exist. Costs [not retrieved].
   Defense polish, not structure.
4. **Crafting Station (suggested in-game at 30,000 DE): LAST, optional.** ⚠️ The library is
   conflicted on whether TH17 even retains Crafted Defenses in Nov 2026 (the system is
   seasonal — ~4-month phases, one crafted defense active at a time, and TH18-era notes say
   TH17 *lost* access) [library — conflicting, `01-th17-core` §9 #5 / `11-newer-systems`
   §9.4]. JJ's game *suggested* it, so something is purchasable — but a temporary seasonal
   defense is the worst possible use of this account's scarcest currency (DE) while heroes
   and pets are DE-starved. **Recommendation: skip until the DE economy is healthy
   (heroes rotating + Phoenix chain funded), then JJ's call.** It does not serve the
   attack program at all.
5. **Ordinary defense levels (Inferno/X-Bow/Monolith/Spell Tower new TH17 levels, Air
   Defense, etc.):** after all of the above, in the library's consensus order — big-ticket
   TH-weapon-adjacent defenses first, point defenses and traps last [library — community].
   One defense level changes little; this entire category is what builders do *between*
   structural items, not a project. Supercharges: explicitly not yet (maxed regular levels
   first, and they are temporary) [library].
6. **Walls:** unchanged from the old queue's Tier E — free-builder overflow sink only,
   never delaying a queue item, never spending resources reserved for one. With 213 walls
   at L16, walls are also the pressure valve when gold/elixir would otherwise cap out.

**Revision vs old queue:** the old Tier A had Firespitters → merges → Pet House → Blacksmith
→ Barracks as an undifferentiated block. The revision inserts Army Camps above all of it (§1),
keeps Firespitter #2 and merges at the top of the *gold* track, and demotes Blacksmith and
Barracks (§5) — the old queue over-ranked both.

---

## 5. Pet House 11 and Blacksmith 10 — one is a key, the other is a formality

**Pet House 10 → 11: 8,250,000 E / 4d** [repo — live-checked]. **Rank: high — first
elixir building after the camps are underway.**
- Unlocks **pet levels 11–15** — which on this account means Unicorn (10, the Queen/Warden-
  class support pet, cap rises 10→15) and Frosty (3, cap 15) can finally grow [library —
  opened wiki max chart; CONFLICTS-checked]. Unicorn is the main-army pet that matters most.
- Unlocks the **Sneezy** pet [library — snippet-only].
- The Pet House is also a *slot*: it is currently the account's DE-to-power converter
  (Phoenix chain, §7). The building upgrade pauses pet research for 4 days — start it when
  the Phoenix chain reaches a natural break (e.g., right after a level lands), not mid-chain
  if a pet level is days from done.
- **Pet order after PH11** (revises old Tier D): **Unicorn → 15 first** (top-end level ≈
  320,000 DE / 8d [library — snippet-only]; full 10→15 ≈ 2.29M DE / ~77d [library —
  snippet-only, treat as upper bounds per §3's staleness warning), then **Phoenix → 10**
  (top level ≈ 190,000 DE / 6d 12h [library — snippet-only]; Phoenix is the RC's revive
  insurance and already in flight at 1→2), then **Frosty → 15**, then Diggy/Angry Jelly
  to 10 as DE allows. Old queue had Phoenix/Diggy ahead of Frosty — Frosty moves up
  because its cap (15) and its hero (whichever of the attack set carries it — assignment
  unconfirmed, §3-inspection item) outrank Diggy's cap-10 ceiling. Do not spread DE
  across all five; two chains fed beats five starved.

**Blacksmith 9 → 10: 9,000,000 E / 5d** [repo — live-checked]. **Rank: LOW — demoted from
old Tier A.** Reason, from the account-fit audit: equipment rarity caps (Common 18 / Epic 27)
already max out at Blacksmith 9 — **BS10 unlocks no equipment level, no slot, no system.**
It is the TH17 building cap and nothing more: pure completion. It should be started only
when a builder and 9M elixir have no better home (after camps, Pet House 11, and Barracks —
see below), or not at all until TH17 is otherwise finished. The account's equipment problem
is *levels on specific pieces* (Mirror/Fireball/Electro Boots at 20 vs Epic cap 27 — an
**ore** problem, not a building problem) and *unknowns* (Eternal Tome level). BS10 fixes
neither.

**Barracks 18 → 19: 13,000,000 E / 5d 6h** [repo — live-checked]. **Rank: below Pet House 11,
above Blacksmith 10.** It unlocks **Meteor Golem** — a troop the shortlist ruling does not
use and the usability rubric does not want (ground, unverified, no trial path). Its value is
optionality (a future meta may want it; TH18 will assume it done) — real, but not worth
13M elixir while camps are unfinished. **Revision vs old queue:** both Blacksmith and
Barracks drop out of Tier A; Pet House stays high; camps take the vacated top spot.

---

## 6. Resource reality — sequencing around an empty gold storage

Balances [repo]: **G 269k / E 3.21M / DE 44.4k**. Storage caps are not the problem
(TH17 max ≈ 28M G/E, 460k DE [library — snippet-only]); *income pacing* is. Consequences:

- **Nothing gold-denominated can start today.** Firespitter #2 (8.5M G) and the Ricochet
  merge (6M G) are the two best gold starts and both are ~1–2 weeks of income away
  (collectors + the attack program's loot + JJ's own play; JJ also holds an unread Treasury
  balance — 2.2M G last read [repo] — which, if still banked, covers the Ricochet merge's
  first third the moment a withdrawal is actually funding a start, per the standing
  Treasury rule).
- **Elixir is spoken for three ways** (camps 17M each, Lab ~8.75M/step, Warden ~10.25M/step
  [repo]) against a 3.2M balance. Staggering (§7) is not optional; the order of elixir
  claims is: **Lab L1 → Camp #1 → Warden step / Camp #2 → Lab L2 → Pet House 11**, adjusted
  at each builder-free moment by what's actually affordable.
- **DE is the tightest currency relative to demand** (44k on hand; heroes + pets both eat
  DE; a single AQ level is ~340k+ [library — stale upper bound]). The DE queue is strict:
  **Pet House slot chain (Phoenix) → Duke chain → attack-set hero steps**, in that priority
  order on any given day, because the pet slot and the Duke builder are *continuous* chains
  (an idle chain-day is lost forever) while attack-hero steps are episodic by design (§3).
  Crafting Station's 30k DE is rejected for now precisely because it would jump this queue
  for a temporary defense (§4.4).
- **Flagged unaffordable now:** Army Camp ×4 (68M E total), Firespitter #2 (8.5M G),
  Ricochet merge (6M G), Pet House 11 (8.25M E), Blacksmith 10 (9M E), Barracks 19 (13M E),
  every hero level except possibly the cheapest Duke step, Balloon 12 (8.75M E).
  **Affordable now:** essentially only the Phoenix chain's next low level (1→2 cost
  40,000 DE / 18h [repo — live]; 2→3 cost [not retrieved], expected in the same low band —
  verify in-game; if it exceeds the DE balance, Frosty 3→4 is the fallback pet start) and
  wall overflow. That is not a planning failure — it is the correct picture 6 hours after
  the owner spent ~27M resources on six upgrades at once. The plan's job is to make sure
  every slot that *can* run, runs, and every slot that frees has its next start pre-chosen.

---

## 7. The next 10 starts — concrete, in order

Assumes the current six timers finish as scheduled and Phoenix 1→2 lands 2026-11-15 03:33 PT.
"Trigger" = the slot freeing + the resource condition; if a resource condition isn't met when
the slot frees, the builder takes the **fallback** listed rather than idling, and the intended
start moves to the next free slot. Lab and Pet House are single slots; builders are six.

| # | Start | Slot | Cost | Time | Trigger / fallback |
|---|---|---|---|---|---|
| 1 | **Lab: Dragon 11 → 12** | Lab | ~8.75M E band [inference — price not retrieved; verify at start] | ~5–6d [inference] | Lab is idle now; start the moment elixir allows. Fallback if elixir < price for >48h: cheapest un-maxed army spell found by the loadout inspection — never idle. |
| 2 | **Pet: Phoenix 2 → 3** | Pet House | DE, low band [not retrieved; 1→2 was 40,000 DE — repo live] | ~1–2d [inference] | Pet slot frees Nov 15 03:33 PT. Fallback: Frosty 3 → 4 if Phoenix's price exceeds DE on hand. |
| 3 | **Hero: Dragon Duke 6 → 7** (chain continues) | Builder (Duke's own, frees ~Nov 15) | DE [not retrieved at this level] | ~1d band [inference from repo timer] | The free chain (§3.2) — Duke's builder simply rolls into his next level. Fallback if DE is committed to #2: King 95 → 96 is *not* the fallback (too DE-heavy); builder takes walls until DE frees. |
| 4 | **Army Camp #1 → 13** | Builder (first non-hero builder free — Archer Tower/Giant Bomb slot) | 17,000,000 E [library — snippet-only] | 7d 12h [library — snippet-only] | Trigger: elixir ≥ 17M. Until then this builder runs walls (overflow rule) — the only honest filler at 269k gold. |
| 5 | **Firespitter #2 — build** | Builder | 8,500,000 G [repo — live-checked] | 4d 6h [repo — live-checked] | Trigger: gold ≥ 8.5M (Treasury withdrawal only as part of funding this start). Fallback: Ricochet merge if gold reaches 6M first and Firespitter is still out of reach — no: Ricochet at 6M while Firespitter needs 8.5M means *wait*; spending the 6M sets Firespitter back days. Fallback is walls. |
| 6 | **Hero: Grand Warden 70 → 71** | Builder (Multi-Gear slot, ~Nov 18) | 10,250,000 E [repo — live-checked] | 4d [repo — live-checked] | First attack-set rotation step (§3.4): elixir hero, Tome scaling, and it starts only outside a declared trial block. Fallback if a trial block is live: Camp #2 takes this builder and Warden waits for the CC slot. |
| 7 | **Army Camp #2 → 13** | Builder (Firespitter #1 slot, ~Nov 18–19) | 17,000,000 E [library — snippet-only] | 7d 12h | Trigger: elixir ≥ 17M after #1/#6 claims. Fallback: Pet House 11 (8.25M E) jumps in if elixir is in the 8.25–17M band — cheaper and high-value (§5). |
| 8 | **Pet House 10 → 11** | Builder (Clan Castle slot, ~Nov 19) | 8,250,000 E [repo — live-checked] | 4d [repo — live-checked] | Start at a Phoenix-chain break (§5). If it already started as #7's fallback, this slot takes **Ricochet Cannon merge** (6M G / 3d 12h [repo — live-checked]) if gold allows, else Camp #3. |
| 9 | **Lab: Balloon 11 → 12** | Lab (frees when #1 lands) | 8,750,000 E [repo — live-checked] | 5d 12h [repo — live-checked] | Automatic roll from #1. Completes the proven army's level profile except Baby Dragon (L3 after this, interchangeable with #9 if Fin prefers cleanup-preset readiness first). |
| 10 | **Hero: Archer Queen 95 → 96** | Builder (next free after #6's builder lands, ~Nov 22) | DE, ~340k upper bound [library — snippet-only, stale; read real price in-game] | ~4–8d [uncertain — see §3] | Second rotation step. Starts only with all other attack heroes up and no trial block declared. Fallback: if DE < price, the builder takes **Barracks → 19** only if elixir ≥ 13M *and* camps #3/#4 are already running — otherwise walls; do not let a fallback cannibalize camp elixir. |

**Immediately after the 10:** Camps #3 and #4 (17M E each) as builders free, Blacksmith → 10
only when nothing above it is waiting, Barracks → 19 per #10's fallback conditions, Multi-Gear
L2 / Firespitter L2s, then ordinary defense levels, walls throughout as overflow.

---

## 8. What this plan deliberately does NOT do

- **No TH18 rush.** The merge set, camps, and support buildings are what TH18 assumes done;
  the old queue's note stands.
- **No Lab speculation** on deferred/avoid-listed armies (Root Rider, LavaLoon, Queen Charge,
  Duke packages) until Fin promotes a candidate — Lab days are the scarcest resource in
  this plan.
- **No gem spending, no magic-item spending** — rails unchanged; nothing here assumes a
  Book/Hammer, and if JJ chooses to spend one, the highest-value targets are Camp #1
  (17M E / 7d12h) or a Warden/Queen level, in that order [inference].
- **No Crafting Station** until the DE economy is healthy (§4.4), and no Supercharges.
- Every price marked [not retrieved] or [inference] gets read in-game at the moment of the
  start — this plan sequences; it does not authorize spending on a guessed number.

*— End of draft. Prepared for Fin's ruling; supersedes nothing until ruled.*
