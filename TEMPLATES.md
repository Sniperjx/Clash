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
Series metrics (S1-B trials): <deployment window (seconds AND tool calls, first->last troop);
input misses: n; spells on-plan / improvised / skipped: n/n/n; ability attempts/fired: n/n>
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
