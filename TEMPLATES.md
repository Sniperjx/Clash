# TEMPLATES — Trial Entries + Agent Handoffs (v1.3)

The folder is the player; agents are interchangeable hands. These two formats are how
one agent's experience becomes every agent's skill. Copy them exactly.

## A) TRIAL entry — one per attack, appended to SESSION-LOG.md under a "Trials" marker
    or kept in a TRIALS section of the log entry for that session.

```
TRIAL #<n> — <YYYY-MM-DD> — [<Agent>] <venue: campaign / friendly / practice-drill / battles>
Base type called (BEFORE deploying): <DEAD / COMPACT / SPREAD / RING / ANTI-AIR / RUSHED / META / new: ___>
Strategy: <S1 / S2 / S3>  Army: <as trained — note any deviation from Army v1>
Blimp path check: <pass / fail — what blocked it>
Result: <stars> stars, <%>%, TH <taken / missed>, loot <G/E/DE or n/a>
Execution notes: <which script steps worked; which inputs missed; ability fired? Y/N/unconfirmed>
Cause code: <FUNNEL / SPELL-TIMING / ABILITY / INPUT-MISS / BASE-MISREAD / COMP / NONE>
One-line lesson: <the single thing the next agent should steal from this attack>
```

Rules: the base-type call is written before the result exists — no retro-fitting the
call to the outcome. Cause codes are how reviews find patterns; pick the dominant one.

## B) HANDOFF block — end of any session where a DIFFERENT agent may play next.
    Append to SESSION-LOG.md as the last block of your session entry.

```
HANDOFF — <YYYY-MM-DD> — [<Agent leaving>]
Account state: <balances; builders: what is upgrading + finish times; Lab: item + finish>
Tier status: <any tier/benchmark changes this session, with evidence>
In-flight: <anything mid-way the next agent must not duplicate or interrupt>
Watch-outs: <base-specific or client quirks noticed; dialogs seen; obstacles left for doubt>
Next best actions (ranked): <1..3, in order, with the file/section that authorizes each>
Open questions for JJ/Fin: <or "none">
```

Rules: a handoff is a promise that the next agent can start from STATE.md + your block
alone, without re-reading the whole log. If it can't, the block is incomplete.

## C) Review block — after every 5 trials of one strategy (append to LESSONS.md)

```
REVIEW — <strategy> — trials #<a>-<b> — <YYYY-MM-DD> — [<Agent>]
Record: <stars distribution; avg %; TH rate>  By base type: <split>
Dominant cause codes: <top 1-2>
Decision: <KEEP / AMEND one variable: ___ / SHELVE> — evidence: <trial numbers>
Reliability claim now justified: <none / "2-star in X of last 10" / ...>
```

## Extra evidence required in each trial

- Strategy version / operator / venue / target TH range / overlapping base tags.
- Exact heroes, equipment, pets, CC payload and siege availability (unknown stays unknown).
- Predeclared trial series and eligibility; all attempts and skips recorded.
- Actual input/observation latency, triggered abilities and missing evidence.
- No campaign-to-PvP reliability extrapolation. Report X/Y for the tested slice only.

## S1-B additional trial metrics (2026-11-14)
Record deployment window in wall seconds and tool calls (first deployment through last main-force deployment), selection/deployment misses, observation delays, each spell on-plan/improvised/skipped with location/effect evidence, each hero ability attempted/fired/AUTO/unconfirmed, exact loadout snapshot, series ID and predeclared target. Unstarted/aborted attempts and eligibility failures remain in the record. A campaign series is not PvP reliability evidence.

## #11 future trial comparability fields
Record strategy/packageversion,booststatus,CCspells/troops/siegeUSED,completeknownloadoutandunknowns,operator,venue,baseclass/THrange. Report fullsetandmatchedsubset separately;allfailures included. Count manualattempt/effect/AUTO separately;spellsassigned/onplan/improvised/skipped plus observedcurrentoccupancy;mark early/late deviations. Store deployseconds,misses/recovery,THkill,stars/destruction,loot/bonus/searchcost,Homeheaders. No promotion from mixedoverallaverage. Current baseline and proposedSeriesC are in ATTACK-PLAN/ATTACK-REVIEW-2026-11-14.md.
