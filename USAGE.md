# USAGE — Seat Usage Ledger (Clash RSI)

North star: LOW-USAGE competence. Usage-per-outcome is reviewed like battle
stats. Seats log at every session end; Fin reviews weekly and rules on waste.

## What gets logged (per session, in SESSION-LOG and summarized here weekly)
- Claude seat: context size at check-in and at close; weekly % when the panel
  is read; compactions (count + trigger size).
- GPT seat: account used (dabbingyeetster / plumisaiahrr), 5h % and weekly %
  at start and end of session.
- Per-outcome cost where measurable: tokens/frames per battle, per B0
  circuit, per challenge claim batch. Retries and recoveries are logged as
  cost, never hidden — they are the hidden usage sink this file exists to see.

## Known state (2026-11-14, last reads — refresh at next session start)
- GPT dabbingyeetster: 5h window resets 3:07 PM PT 2026-11-14; weekly 84%.
- GPT plumisaiahrr: 5h 3% used; weekly 68%.
- Claude (JJ's plan): weekly 21% at last panel read (~12:35 PT).
- Scout context: ~150k est at 12:35 PT check-in. Compact band: 250-300k
  (Fin sends "prep to compact"; seat saves state, replies READY; JJ fires
  /compact). Scout reports any spawned Claude chats' sizes too.
- Measured unit costs on record: Haiku subagent cold start ~64-72k tokens per
  spawn (reader-only value proven; hands experiment cancelled at ~252k total
  for zero output — the standing example of what this ledger exists to catch).

## Rules
- Rotation is BY SESSION and logged (which account, when) — never mid-session.
- Agents never type credentials; a password/2FA prompt stops the session.
  Account switching is JJ-present-only (proven 2026-11-14, log #23), so
  schedules assume the already-signed-in account.
- A seat that cannot state its usage at check-in says so; estimates are
  labeled estimates.
- **No drills that a real action can replace (JJ, 2026-11-14):** seat usage is
  spent only where it produces account value or evidence a real action cannot.
  Practice/drill runs are cancelled when the same evidence is available from a
  real battle that also pays loot — JJ waived Scout's Practice proof on
  exactly this ground ("don't have Sonnet waste usage"). Drills survive only
  where the real action is genuinely gated or unsafe.
