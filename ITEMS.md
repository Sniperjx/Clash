# ITEMS — Magic Item & Potion Policy (Fin ruling, 2026-11-14)

**Status: ADOPTED** from the research draft (~/workspace/clash-army-research/07-items-policy-draft.md),
under JJ's 2026-11-14 delegation of item use to the system. **Approval gates: Books,
Hammers, and Runes require Fin's per-use approval in chat before a seat fires one.**
Routine potions fire on the policy conditions below without per-use approval; every
use is logged. Gem-priced or money-priced anything is banned outright.

---

# 07 — Magic Item & Potion Policy (DRAFT for Fin's ruling)

**Date:** 2026-11-14 · **Account:** TH17, 6 builders, Lab 15, Pet House 10.
**Mandate (JJ, 2026-11-14):** item use is delegated to the system and must be
optimal per research. The owner admits he fires items carelessly ("I just
activate the resource potions") — this policy exists to replace that habit.
**Hard rails, no exceptions:** seats never spend money, never spend Gems, and
never burn a one-shot item (Book / Rune / Hammer) outside the fire rules
below. Seats also never *sell* an item for Gems without a Fin ruling — a sale
is an irreversible burn at a bad rate (Books/Runes 50 Gems, Hammers 100,
Potions 10, Wall Rings 5 [wiki — opened]).

**Inventory is not yet read.** Every rule below is keyed to a *situation*, not
to a holding. When the seat reads the inventory in-game, it also records:
collector levels (needed for §1 math), Lab Assistant recruitment status
(§11), and current storage levels (needed for §8 thresholds).

**Source key:** [primary] = Supercell · [wiki — opened] = 1337wiki/Fandom
page opened in the project library · [wiki — snippet] = wiki via snippet ·
[community] = guides/forums · [repo] = live-checked in this project's repo ·
[inference] = arithmetic/reasoning from labelled inputs · [unknown] = could
not be verified; do not act on it.

---

## ⏰ IN FORCE RIGHT NOW — Hammer Jam (ends Nov 16, 08:00 UTC)

Hammer Jam is live: 50% off eligible Home Village upgrade costs *and* times,
plus 2× collector production/capacity. Excludes Supercharges and Crafted
Defenses [primary — snippet, library §13]. Jam-specific rules override the
standing rules below until it ends:

- **Start planned upgrades before the Jam ends** — half price, half time.
  This is the cheapest the camp pipeline (17M E each [snippet]) will ever be.
- **Builder / Research / Pet Potions gain value** — their saved hours chew
  through halved timers, effectively double throughput [community, library
  §13]. The Jam is the one window where firing a Builder Potion on a full
  6-builder board is clearly correct (see §2).
- **Hold Books and Hammers** — they skip a timer that is already halved, so
  they return half their normal value [community]. Exception: a Book in the
  Jam's final hours that frees a builder to *start* one more half-price
  upgrade. Hammers also gain a second reason to wait: TH19 "lands mid-month"
  [primary — snippet], and a Hammer carried into a new Town Hall buys its
  most expensive upgrade.
- **Hold Resource Potions** — the Jam already doubles collector production.
  Whether a Resource Potion stacks on top of the event boost is [unknown];
  never burn an item on an unverified interaction.

---

## 1. Resource Potion

**What it does:** doubles production of *all* Home Village collectors —
Gold Mines, Elixir Collectors, **and** Dark Elixir Drills — for 1 day
[wiki — opened]. It does not touch storages, the Treasury, or loot from
attacks. Stacking potions extends duration, never strength [wiki — opened].
Cap 5 held.

**The math (why the owner's habit wastes it):** at max level, 7 Mines and
7 Collectors at 7,560/hr [wiki — 1337wiki] produce 52,920/hr ≈ **1.27M per
day** of Gold and of Elixir; the potion adds one extra day of production ≈
**+1.27M Gold and +1.27M Elixir**. At L16 collectors (7,000/hr) it's
≈ +1.18M each; at L15 ≈ +1.06M each [wiki rates; arithmetic = inference].
JJ's actual collector levels are [unknown until read]. Drills: 3 × L11 at
200/hr [wiki — 1337wiki/Fandom agree] = 600/hr ≈ 14,400 DE/day, so the
potion's DE third is worth up to **+14,400 DE** — *but* drill capacity is
only 4,600 each (13,800 total), which fills in ~11.5 hours at doubled rate
and then production **stops**. Uncollected, the DE bonus mostly evaporates;
collected once mid-window, nearly all of it is real. Mine/Collector capacity
(420,000 × 7 ≈ 2.94M) comfortably holds a full doubled day, so Gold/Elixir
have no cap problem if emptied at the start.

**Fire rule — all four must hold:**
1. Gold **and** Elixir storages both below ~70% (room to absorb ~1.2M each
   without sitting at raid-bait levels).
2. Collectors emptied at firing (a chore circuit does this anyway).
3. A seat will run at least one more collection pass ~10–12h later (the
   drill-capacity rescue above).
4. A spend for the produced loot is queued within ~a day (camp, Firespitter
   #2, a merge) — loot produced with nowhere to go is loot donated to
   raiders.

**Never:** during Hammer Jam (see box); when any storage is full or near
full; back-to-back out of habit; as a substitute for farming — one potion
day (~2.5M combined G/E) is worth less than one decent attack session, and
it is the *weakest* potion in the inventory at this account stage.

## 2. Builder Potion

**What it does:** Home Village builders work at 10× for 1 hour = **9 extra
hours of work per active builder** [wiki — opened]. With all 6 builders
busy: **54 builder-hours** per potion. Does **not** affect the Builder's
Apprentice [wiki — opened]. Cap 5 held.

**Fire rule:**
- All 6 builders busy, **and** every running job has ≥ ~10 hours remaining
  [wiki — opened best-use arithmetic] — a job with 3h left only absorbs 3h
  of the boost and wastes the rest.
- Best moments: right after a full board of long jobs has been started
  (e.g., the day camps/merges/Firespitter are all rolling), and any time
  during Hammer Jam (halved timers double the throughput [community]).

**Never:** with a builder idle or about to idle with no next start queued;
on a board of short jobs (traps, bombs — sub-10h remainders); in the same
hour you plan to Book or Hammer the longest job (you'd pay a one-shot item
to remove the very timer the potion was accelerating — sequence them:
potion first, Book later if still needed).

## 3. Research Potion

**What it does:** Laboratory research runs at 24× for 1 hour = **23 extra
hours** — effectively one day cut off the running research [wiki — opened].
Cap 5 held.

**Fire rule:**
- The Lab is running a *priority-queue* upgrade with **> 24h remaining**
  (the potion's value is capped by the remaining time — firing it at 10h
  remaining saves 10h, not 23h).
- Best target class: the long air-program upgrades — Dragon →12 first, then
  Balloon →12 (8.75M E / 5d 12h [repo — live-checked]) [inference from
  PRIORITIES v2]. Stacking 2–3 potions at the *start* of a 5–8 day research
  is legitimate; each still returns its full 23h.
- During Hammer Jam, research times are halved, so potions chew through
  them at effectively double rate [community] — a good Jam spend.

**Never:** on a research with < 24h remaining if a longer one is queued
next (wait the few hours, start the long one, then fire); on a troop/spell
the army program doesn't use (deferred candidates — Root Rider, LavaLoon —
get zero Lab days until Fin promotes one, per PRIORITIES v2, so they get
zero potion hours too); to finish a job early just because the Lab "feels"
idle — the Lab is never idle under the standing queue.

## 4. Training Potion — REMOVED FROM THE GAME

**What it does:** nothing. It no longer exists. The Clash Anytime update
(Mar 24–27, 2025) removed all troop/spell/siege training times and hero
recovery times, and the Training Potion was removed with them; potions
players still held were **automatically sold for Gems** [primary —
Supercell; wiki — opened]. Armies are instant now, so there is no
"training speed between trial blocks" to boost — the AI attack program's
pace is set by seat decision-making, not by any item.

**Policy:** the inventory cannot contain one. Any guide, shop listing, or
third-party page that mentions Training Potions is pre-March-2025 material
or wrong. One live conflict is on record (CONFLICTS H29): a Nov 2026 guide
describes buying 10-medal Training Potions in the League Shop to convert
medals to Gems 1:1 — **unresolved**; seats must not spend League Medals
chasing it unless the item is seen in-game *and* Fin rules on it first.

## 5. Power Potion & Hero Potion

**What they do:** Power Potion — troops, spells, and Siege Machines fight
at your Town Hall's max level for 1 hour [wiki — opened]. Hero Potion —
Heroes **and Pets** fight at your Town Hall's max level for 1 hour;
**attacks only since Feb 2026** (it no longer boosts defense) [wiki —
opened]. Cap 5 each.

**What they're worth on THIS account [inference from repo snapshot]:**
- Power Potion: the attack army is nearly maxed already — Dragons 11 of
  12, Dragon Riders at cap 5, Rage/Freeze at cap. The whole potion buys
  **+1 Dragon level for one hour**. Marginal.
- Hero Potion: BK/AQ +5, Warden +5, RC +5 — but Minion Prince is +20
  (70 of 90) and the Duke +14. Its real value is concentrated in the
  Prince. Still one hour, attacks only.

**Fire rule:** only for a *declared, high-stakes attack window* — a war
attack if Tier 3 is ever opened by JJ, or a Fin-ruled special occasion —
where the boosted hour covers the attacks that matter.

**Never — the data-integrity rule:** **never during a benchmark trial
series** (Series B/C or any successor). Trials measure the operator and
the army script at true levels; a boosted trial is a different stratum and
poisons the comparison (Series B's boosted SB-1 is excluded from the
operative stratum for exactly this reason). Never for routine farming —
+1 Dragon level does not change farming outcomes enough to spend a
finite item. Default for both potions: **hold**.

## 6. Books (Building / Fighting / Spells / Heroes / Everything)

**What they do:** instantly finish an upgrade **already in progress**; you
still pay the full resource cost to start it [wiki — opened]. Cap 1 each.
A Book's value = the timer it skips, so the value rule is absolute:
**a Book goes on the longest eligible timer you own, or it doesn't go.**

**Fire rules by book:**
- **Book of Building** → the longest running building timer (Clan Castle /
  Firespitter-class multi-day jobs). Never on a < 2-day job while longer
  jobs are running or queued.
- **Book of Fighting** → the longest Lab troop/siege job in the army
  program (Dragon 12 class). 
- **Book of Spells** → the longest Lab spell job *in the program*; the
  army's spells (Rage/Freeze) are already at cap, so this book will
  usually have no worthy target — holding it is correct, not wasteful.
- **Book of Heroes** → the longest hero **or pet** upgrade [wiki — opened:
  it covers pets too]. Top hero levels run ~8 days at 340–380k DE
  [library — 05-upgrade-priority]. Classic best use: skip most of an
  8-day hero level, or return a hero instantly for a war/CWL window if
  one is ever authorized.
- **Book of Everything** → the flexible spare. Use **only when no specific
  Book fits** the timer you need finished [wiki — opened best practice].
  It is the rarest book (not sold by the Trader [wiki — snippet]) and is
  never spent on something a class Book could have done.

**Never:** on a short upgrade to "keep things moving" (start the long
upgrade first, then decide); on a job with < 24h remaining unless that
finish unlocks a queued start *today* (e.g., frees the Pet House slot for
the next chain step); two Books on the same slot-class in one week while
Hammers sit unused (Hammers are strictly stronger — §7).

## 7. Hammers (League Shop only — CWL Medals, never Gems)

**What they do:** **start and instantly finish** an upgrade with **no
resource cost at all** [wiki — opened]. This makes a Hammer strictly
stronger than a Book: it saves the cost *and* the timer. Prices: Building /
Fighting / Spells **120 medals**, Heroes **165 medals** [wiki — opened].
Cap 1 each; **7-day cooldown** before buying the same type again; the
Hammer must *start* the upgrade (it cannot finish one already running);
a free builder is still required where applicable; walls and shop items
cannot be hammered [wiki — opened]. League Medals cap at 2,500 and
overflow converts at a punitive 1 Gem per 10 medals [wiki — snippet] —
medals sitting at cap are medals burning.

**Fire rule:** the **most expensive, longest** upgrade available in the
class [wiki — opened best use], with this account's pipeline applied:
- **Hammer of Building → an Army Camp L12→13** while any camp remains:
  saves 17M Elixir [snippet] *and* ~7.5 days, and the +5 housing lands
  immediately. After camps: the most expensive queued defense (Firespitter
  #2 class, 8.5M G [repo — live-checked]). During Hammer Jam, hold (the
  Jam already halves the cost the Hammer would save) unless the medal cap
  forces a buy.
- **Hammer of Fighting → Dragon →12** (the Lab's priority job; saves the
  elixir and the multi-day timer). 
- **Hammer of Heroes → the longest DE hero level available** (up to
  ~380k DE saved [library]) — DE is this account's scarcest currency, so
  a hero Hammer is the highest-resource-value Hammer on the board. Also
  valid on a long pet upgrade (it covers pets [wiki — opened]).
- **Hammer of Spells → hold** until a below-cap spell enters the Lab
  queue; the army's spells are maxed, so there is currently no worthy
  target.

**Never:** on a cheap or short upgrade (a Hammer spent on a 2-day job
burns a 7-day-cooldown slot and ~120–165 medals for a fraction of its
value); on an upgrade the Jam currently halves if it can wait a day;
letting medals rot at the 2,500 cap — if the cap is near and no worthy
target exists in a class, that is a Fin escalation, not a seat impulse buy.

## 8. Runes (Gold / Elixir / Dark Elixir)

**What they do:** fill one storage type **completely** [wiki — opened].
Cap 1 each. Cannot be used on a full storage; the game warns above 70%
full [wiki — opened]. TH17 storage caps: **28M Gold / 28M Elixir**
[wiki-mirror — snippet]; DE storage cap [unknown — at least ~380k by
inference from top hero-level costs; verify in-game at first read].
**A Rune's value = cap − current balance.** Fired at half-full storages,
it burns half its value. That is arithmetic, not opinion.

**Fire rule — the three-part sequence, all in one session:**
1. **Spend first:** the storage of that type is spent down to **≤ 30%
   full** (stricter than the game's 70% warning — the last 30% is where
   the real value is).
2. **Fire the Rune.**
3. **Spend again immediately:** the filled storage is chained straight
   into the queued big spend it was fired for. A Rune that fills storages
   with no spend behind it just paints a target on the base — full
   storages are what raiders queue for.

**Account pairings [inference from PRIORITIES v2]:**
- **Rune of Elixir → Army Camp pipeline** (17M per camp; spend elixir
  down on Lab/walls-overflow first, rune, start the camp).
- **Rune of Gold → Firespitter #2 / merges** (gold is the scarce
  currency; 8.5M G for Firespitter #2 [repo]).
- **Rune of Dark Elixir → a hero or pet chain start** (spend DE down,
  rune, start the ~340–380k DE level).

**Never:** above 30% full except one case — if a Rune would otherwise be
displaced (see §10 overflow) and no spend-down is possible, firing it
beats losing it to a 50-Gem expiry conversion; that call is Fin's. Never
fire two Runes back-to-back into the same pipeline (the second fill has
nowhere to go). Never fire a Rune the same day a season-bank claim lands
in the same resource without Fin sequencing the two (§10).

## 9. The rest — one rule each

- **Wall Rings** (cap 25): each ring substitutes for **1,000,000** Gold or
  Elixir of a wall upgrade [wiki — opened]; a max wall segment (L17→18,
  7M [wiki-mirror — snippet]) takes 7 rings. Walls are **overflow-only**
  in PRIORITIES v2, so rings are spent only when walls are legitimately
  the overflow spend of the day — then rings-first is correct (they free
  real loot for the queue). Never buy rings with Gems; League Shop rings
  (30 medals / 10 [conflict on record — older sources say 50]) only with
  medals surplus *after* Hammer needs. Never spend rings on low-level
  walls where 1M of loot is trivially farmable.
- **Shovel of Obstacles** (cap 5): purely cosmetic — makes one obstacle
  movable [wiki — opened]. Zero progression value. Hold forever or sell
  only on JJ's word; seats never use one (and **never** on an event
  obstacle — the CHARTER rail keeps event obstacles untouched entirely).
- **Clock Tower Potion** (cap 5): Builder Base only — out of scope for
  this project. Hold; never use.
- **Builder Star Jar** (cap 5): refreshes the Builder Base Star Bonus
  [wiki — opened]. Builder Base only — out of scope. Hold; never use.
- **Pet Potion** (cap 5): Pet House upgrades run 24× for 1 hour = **23
  extra hours** [wiki — opened]. Fire only when the running pet upgrade
  has **> 24h remaining** and the Pet House is on the critical path
  (the Phoenix chain feeding the Royal Champion). Early pet levels are
  short (Phoenix 1→2 was 18h [repo]) — a Pet Potion fired there saves
  less than its face value and is a waste. Never stack two unless
  remaining time exceeds ~46h.
- **Super Potion** (cap 5): boosts one Super Troop for 3 days — the
  alternative to paying **25,000 DE** per boost [wiki — opened]. Standing
  status: Super Troop use on this account is **undecided** (Sneaky
  Goblins are a deferred, Tier 2-era farming candidate in the army
  research). Policy: **hold all Super Potions; never pay the 25k DE cash
  boost** — DE is committed to the pet/Duke chains. If a Super Troop
  farming program is ever approved, Super Potions are the *only* approved
  way to pay for boosts [inference].

## 10. Season track, Hoggy Bank, and overflow — claim-and-hold rules

**The bank (Hoggy Bank, since the Mar 2026 Gold Pass rework):** loot from
attacks fills the bank all season; Gold Pass pays a **5× multiplier when
claimed at season end**; caps scale with Town Hall — Silver up to 8M
Gold/Elixir, Gold Pass up to 40M [primary — snippet]. Exact TH17 caps and
the DE cap are [unknown]; whether the payout can overflow storages (the
old Season Bank could) is **not verified for the Hoggy Bank** — verify
in-game at the first season end the system witnesses.

- **Bank claim rule:** in the season's final days, spend storages *down*
  into queued upgrades (camp, Firespitter #2, merges) so the payout lands
  with maximum headroom, then claim at season end. Spending first is
  correct under both overflow rules, so the [unknown] above doesn't block
  the rule. Seats never buy the Gold Pass or any tier unlock (money rail)
  — if JJ holds a pass, the system just works its track.
- **Free-track items are claim-and-HOLD by default.** Claiming early is
  free and safe; *using* follows §§1–9. Claim everything claimable before
  season end — unclaimed track rewards are lost value [inference from
  track structure].
- **Choice Nodes** (pick-one rewards): pick by the pipeline, not by
  headline value — e.g., Rune of Gold vs Elixir → the resource the next
  queued big spend needs; Book of Fighting vs Spells → Fighting while
  Dragon 12 leads the Lab queue. Unclaimed nodes default to the *first*
  option at season end [community — snippet], so a seat makes the pick
  before then. If a node offers an item already at cap (Books/Runes/
  Hammers cap 1), pick the other option, or use the held item first if
  its fire rule is met.
- **Overflow / Temporary Storage:** an item won while at cap sits in
  Temporary Storage for **24 hours**; since Mar 2026 you may use it on the
  spot or sell it; an expired one converts to Gems at sell price [wiki —
  opened]. Rule: a Book/Rune/Hammer in Temporary Storage triggers a Fin
  decision the same day — find a legal fire (§§6–8), or accept the Gem
  conversion knowingly. Never let one expire *unnoticed*, and never
  panic-burn one into a bad target just to beat the clock.
- **Magic Snacks** (chest rewards — a separate, weaker family, *not*
  Magic Items [wiki — opened]) also live in 24h Temporary Storage: they
  are use-or-lose by design, so a seat may use an expiring Snack on its
  face purpose (e.g., a Builder Bite during a chore circuit) without a
  ruling — the one exception to the no-impulse-use rule, because the
  alternative is zero.

## 11. Gem-priced helpers — never (one paragraph)

The **Builder's Apprentice** costs 500 Gems to recruit and ~6,500 Gems to
max; the **Lab Assistant** is free to recruit but ~8,500 Gems to max; the
**Alchemist** costs 100 Gems to recruit [wiki — snippet; community totals].
Every Gem-priced step is outside seat authority under the never-spend-Gems
rail — seats never recruit, upgrade, or gem-boost any helper, full stop.
One free exception: if the Lab Assistant is *already recruited* (status
[unknown until read]), assigning his free daily hour of work to the
running Lab job costs nothing [wiki — snippet] and is a legitimate chore-
circuit action — assign it to the longest running research, same logic as
§3. Whether JJ ever buys helper levels himself is his decision, outside
this policy.

---

## DECISION TABLE — the one page seats actually follow

Default for every item is **HOLD**. Fire only when the row's conditions
are met. Anything not covered → ask Fin.

| Item | FIRE when (all conditions) | NEVER when |
|---|---|---|
| Resource Potion | Storages < 70% · collectors emptied · a re-collection pass will run in ~10–12h · a spend is queued within a day | Hammer Jam · any storage near full · as a farming substitute |
| Builder Potion | All 6 builders busy · every job ≥ ~10h remaining · (Jam: fire freely on a full board) | A builder idle/short jobs · same hour as a Book/Hammer on the long job |
| Research Potion | Lab on a queue priority with > 24h remaining · best at the start of a 5–8d job | < 24h remaining with a longer job next · off-program troops/spells |
| Pet Potion | Pet upgrade running with > 24h remaining · Pet House on critical path | Short pet levels (< 24h) · stacking past remaining time |
| Power Potion | Fin-ruled high-stakes attack window only | **Any benchmark trial** · routine farming |
| Hero Potion | Fin-ruled high-stakes attack window only | **Any benchmark trial** · routine farming · "because it's there" |
| Super Potion | Only inside a Fin-approved Super Troop program (none exists yet) | Paying the 25k DE cash boost instead · any use today |
| Book of Building | Longest running building timer (multi-day class) | < 2d jobs while longer ones run/queue |
| Book of Fighting | Longest program Lab job (Dragon 12 class) | Off-program research · short jobs |
| Book of Spells | Longest program spell job — usually: no worthy target, hold | Burning it because it's old |
| Book of Heroes | Longest hero/pet timer (~8d class) or to return a hero for an authorized war window | Short hero levels while longer ones queue |
| Book of Everything | No class Book fits the timer that must finish | Anything a class Book could have done |
| Hammer of Building | Starting a camp L13 (pre-camps) / priciest queued defense · free builder ready | Jam (hold, unless medal cap forces) · cheap/short upgrades |
| Hammer of Fighting | Starting Dragon →12 | Off-program research |
| Hammer of Heroes | Longest DE hero level (or long pet upgrade) | Short levels · letting medals rot at 2,500 cap instead (escalate to Fin) |
| Hammer of Spells | A below-cap spell enters the Lab queue | Today — no worthy target exists |
| Rune of Elixir | Elixir ≤ 30% full → fire → camp start same session | > 30% full · no queued spend · same day as a bank claim in Elixir (unsequenced) |
| Rune of Gold | Gold ≤ 30% full → fire → Firespitter #2 / merge same session | Same as above, Gold |
| Rune of DE | DE ≤ 30% full → fire → hero/pet start same session | Same as above, DE |
| Wall Rings | Walls are the day's legitimate overflow spend · max-level segments (7 rings) | Low-level walls · bought with Gems · ahead of Hammer medal needs |
| Shovel / Clock Tower Potion / Builder Star Jar | — (no fire condition exists in this project) | Always — cosmetic / Builder Base, out of scope |
| Training Potion | — (removed from the game Mar 2025; cannot exist in inventory) | Chasing the League Shop listing rumor without a Fin ruling |
| Season bank | Final days: spend storages down → claim at season end | Mid-season fretting — it pays at season end, not before |
| Track / Choice Node items | Claim everything before season end · nodes picked by pipeline need | Letting nodes default unexamined · claiming a capped item's twin |
| Temporary Storage (24h) | Same-day Fin decision: legal fire or knowing Gem conversion | Expiring unnoticed · panic-burning into a bad target |
| Helpers (Apprentice / Assistant / Alchemist) | Assign already-owned **free** Lab Assistant hour to longest research | Any Gem spend: recruit, upgrade, boost — ever |

---

## Gaps & unknowns (do not act on these; verify in-game or escalate)

1. JJ's actual collector levels — §1 yields are ceilings at L16–17.
2. TH17 Dark Elixir storage cap — needed for the §8 DE threshold.
3. Hoggy Bank at TH17: exact caps, DE cap, and whether payout overflows
   storages [library §15 gap].
4. Resource Potion × Hammer Jam stacking — assumed non-stacking for
   policy purposes; unverified either way.
5. League Shop Training Potion listing (CONFLICTS H29) — unresolved.
6. Dragon →12 exact Lab cost/time [not retrieved] — Balloon →12
   (8.75M E / 5d 12h [repo — live-checked]) is the anchor figure.
7. Lab Assistant recruitment status on this account.
8. League Shop Wall Ring price: 30 vs 50 medals for 10 [conflict on
   record; the 30 figure has the more recent evidence].
