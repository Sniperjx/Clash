# BASE-TYPES — Recognition, Verdicts, Go/No-Go (v1.3)

Call the type BEFORE deploying, write it in the trial entry, and let the verdict pick
the strategy. Mis-calls are data: if the result contradicts the call, the post-attack
note says what the telltales actually were — that's how this file gets smarter.

All verdicts are starting hypotheses for trial venues (campaign/practice/B2-eligible),
tightened by trial data. In real farming (Tier 2), the same calls decide attack vs Next.

## 1. DEAD / COLLECTOR base — ATTACK (easiest real reps)

Telltales: collectors/mines visibly FULL and sitting on the outer ring; tombstones
scattered; traps likely unarmed; heroes possibly absent; storages emptier than
collectors. [community telltales — verify against your own trial results]
Verdict: S1, edge = the collector-densest side. Loot first; stars are a bonus here.
LLM difficulty: LOW. This is the Tier-2 training-wheels target.

## 2. COMPACT base — ATTACK with S3 (or careful S1)

Telltales: buildings touching or ~1 tile apart across most of the base; defenses
clustered. Chain lightning gets full value here.
Verdict: S3 (Electro Dragons) if levels allow, else S1 with a narrow entry.
LLM difficulty: MEDIUM — the base does your funneling for you, but spell triggers
come faster.

## 3. SPREAD / ANTI-CHAIN base — S1 only, NEVER S3

Telltales: consistent ~2-tile gaps between buildings (built to break chains);
defenses in separated pods.
Verdict: S1 line push; Electro Dragons are banned here (their chain finds nothing).
LLM difficulty: MEDIUM — wide lines can split around pods; funnel discipline matters.

## 4. RING base — S1 with funnel emphasis, Blimp value HIGH

Telltales: resource/defense ring around a walled core holding the Town Hall;
a visible moat or gap ring inside the walls.
Verdict: S1, but the funnel step is the whole attack — if both funnels fail, the
line circles the ring and never enters. Blimp path to the core is usually clean,
which serves the 2-star plan. If the funnels look hard (strong corner defenses),
consider NO-GO in real venues.
LLM difficulty: MEDIUM-HIGH (single point of failure: the funnel).

## 5. ANTI-AIR base — NO-GO for S1/S2 (skip in real venues; trial venues: log and learn)

Telltales: Air Defenses centralized (not on edges), covered by Wizard Towers;
Air Sweepers covering the obvious air entries; Seeking Air Mines likely on air lanes.
Library warning: centralized ADs under Wizard Tower cover punish grouped air hard.
Verdict: our whole current program is air. In Battles: press Next. In trial venues,
attack only as a deliberate hard-mode rep and label it that way.
LLM difficulty: HIGH. A ground strategy for these bases is a future program phase,
not an improvisation.

## 6. RUSHED / PROGRESS base — ATTACK, expect overperformance

Telltales: defense levels visibly mixed/low for the TH (wooden/low walls segments,
low-level Infernos), TH upgraded far ahead of its defenses.
Verdict: S1 standard script. Good confidence reps.
LLM difficulty: LOW.

## 7. MAXED / META TH17-18 base — NO-GO (for now)

Telltales: max-level merged defenses placed per current meta, Firespitters covering
the TH zone, nothing visibly behind. In trial venues these are stretch goals only
after a strategy is measured-reliable vs types 1-4; in farming, Next, always.
LLM difficulty: VERY HIGH. Pride is not a strategy input.

## Pre-attack GO / NO-GO checklist (every attack, out loud in the log)

1. Base type called? (If "none of these," describe it in one line — new type candidate.)
2. Blimp path to TH: crosses <= 1 Air Defense's range and no Sweeper blowing against it?
   If not -> NO-GO for the 2-star plan (farming: Next; trials: attack only as 1-star loot/learning rep, labeled).
3. Funnel corners: can Queen and RC plausibly clear their corners vs the corner defenses?
4. Strategy matches the type per this file? If improvising — stop. Improvisation is
   how unlogged failure modes are born.
5. Army of record fully trained, spells complete, heroes awake? If not, don't start.

## v1.3 local review corrections

Dead/collector is a tentative visual classification, not proof of absent heroes, CC troops or traps. Types may overlap (compact plus anti-air, rushed plus ring); record all material tags. Visible AD/Sweeper screening does not reveal trap placements or ensure Blimp survival. Treat anti-air/maxed classifications as conservative current-program exclusions, not universal rules of the game. S2/S3 remain research-only until an exact composition is logged.

## Current no-siege baseline scouting - #11 review
Current ATTACK-PLAN runbook supersedes any requirement above that assumes a filled Blimp. For S1-B0/Narrow noCC/siege use: positively identify TH separately from Eagle; record entry,cornerdefenses,AD/Sweepers,centraldamagecluster and where pack can path. A ring moat/centralTH is a serious split risk;lowwalls aren't safeairdefenses. TwoSweepers facingsegment ->re-pickentry/NO-GO;hiddenCC/traps remainunknown. SupportedBlimp path is a separate unreadyvariant,not guaranteedclean. Record allskips/failures;strongcentralring stretchtests distinctfromnormaleligiblecomparisons.
