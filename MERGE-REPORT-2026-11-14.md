# MERGE REPORT - Claude (Sonnet), 2026-11-14

Job 0 from KICKOFF-CLAUDE. Merged Sol's PC-local Desktop\Clash into Sniperjx/Clash (base c680bf4).
Pre-merge local copy of every .md file: archives/premerge-local-2026-11-14/ (local only). Remote versions stay in git history.

## Per-file result (Fin's rulings in chat, applied)
| File | Result |
|---|---|
| SESSION-LOG, STATE, ATTACK-REVIEW, BENCHMARKS, LESSONS, PLAYBOOK, BASE-TYPES, TEMPLATES, README | Local (Sol closeout) wins, per MERGE-NOTE |
| CHARTER | Local verbatim. Local already holds the supervised-hands section (Sol's wording, same substance as Fin's remote two-model section) and the GPT Tier 1 row (Fin accepted). Remote's older 'Tier 1: Not yet' row dropped as stale. |
| TERRA-SCOPE | Local table is base. Fin's earlier detailed A-F draft appended as an appendix for Fin's ruling (nothing dropped). |
| DAILY-ROUTINE | Remote spine (it already carries the Tier-0 exceptions, Forge free slot, Treasury rule, renumbered CLAIMs) plus Sol's two local appended sections (v1.3 corrections, Terra amendment). Local items 6 and 16-19 superseded by the remote's officially-checked wording. |
| PRIORITIES | Local (ASCII arrows, [done] marker); content identical to remote. |
| ATTACK-PLAN | Local current-runbook block on top; remote body (Series A-D, Series B review) as the historical base; Sol's local-only sections appended as an appendix. |
| ORCHESTRATION, COLLAB, CATCHUP/KICKOFF/HANDOFF/MERGE-NOTE | Remote, unchanged |
| Added from local | ATTACK-REVIEW-2026-11-14, SOURCE-CHECKS-2026-11-14, CLAUDE-LOCAL-SUPPLEMENT-2026-11-14, fin-attack-closeout-2026-11-14.jpg |
| Stay local only | archives/, clash-of-clans-research/ (Fin: research library is his side) |

## Conflicts for Fin's ruling
1. **Series C pass wording.** Remote (confirmed text): a pass on five clean trials IS a B2 pass; Tier 2 unlocks. Local runbook (Sol): clean set 'may satisfy B2; no automatic promotion before complete audit'. Merged file carries both; the local runbook is on top. Needs one sentence from Fin.
2. **Local runbook extras not in remote's Series C text:** batch composition (Batch1 Q+RC+6 Dragons, Batch2 rest), Rage timings (Rage2 ~25%, hold if no qualifying moment by ~70%), Freeze jobs, finish rule, log fields, Anti-air/META exclusion. Kept on top; remote body says 'as written above'.
3. **Old local S1 wording** ('Star 1 / Star 2 / Blimp dedicated to the TH', 80% promotion line) exists only in local's pre-review S1 text; superseded by remote's S1 section, retained in the premerge backup.
4. **Small remote-only lines dropped under 'local wins':** BASE-TYPES v1.3.1 'Caution' line and a few lines; TEMPLATES series-metrics lines; BENCHMARKS/PLAYBOOK wording. Most are Unicode vs ASCII variants. Recoverable from git history (c680bf4).
5. **Encoding:** remote files use Unicode punctuation, local uses ASCII; merged files are LF and keep whichever side won.

6. **The jpg identified:** fin-attack-closeout-2026-11-14.jpg is a screenshot of the Muse chat showing Fin's 'All wrapped then' message and Sol's final closeout text (the 6+6 typo fix, final Home 7,712,116 / 6,660,631 / 32,093 / 2,833, Phoenix 16h46m). Evidence of Sol's closeout message; no new facts. Kept in the repo as an evidence file; Fin may rule it out.
7. **CHARTER union note:** Fin's ruling said include the remote two-model section. Local already contains the same rules under 'Supervised hands - Fin ratification' (judgment model owns the seat; hands capped; evidence labeled; hands draft, seat commits; own B0/B1 if unsupervised; rails bind hands). Inserting both would duplicate. Flagged for Fin: keep local only, or add the remote text as an appendix.
8. **Remote moved during the merge** (900e756, 065164a, 1924b38: Fin's rulings in MERGE-NOTE, push-gate clarification, ORCHESTRATION north-star). Those two files were taken from origin/main, not overwritten.

## Not done / not verified
- Content merge checked by line-presence comparison only, not read line by line. Series C / Terra scope wording needs Fin's read.
- Game untouched since gold collection.
