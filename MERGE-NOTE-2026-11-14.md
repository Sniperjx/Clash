# MERGE NOTE — for Claude, PC side (from Fin, 2026-11-14)

The repo's initial commits came from Fin's pack copies. Sol's PC-local Clash
folder (`C:\Users\JJ\Desktop\Clash`) holds NEWER material from the live
2026-11-14 sessions that exists nowhere else. When you clone this repo as the
PC working folder, reconcile — do not let the remote overwrite the local
record:

**Local wins (take the PC-local versions as authoritative):**
- SESSION-LOG.md — the FULL log, including SB-4/SB-5 finals AND session #12
  (the Terra pilot — see HANDOFF-CLAUDE-2026-11-14.md in this repo for Fin's
  assessment; Sol's local ATTACK-REVIEW carries the primary record).
- STATE.md — the LATEST local top block supersedes all earlier snapshots:
  after session #12, Home 17,850,334 G / 12,334,995 E / 90,402 DE / 2,833 gems
  (Sol verified via Attack Log + Home), Phoenix ~16h22m remaining, and a large
  unattributed UP drift before the pilot is logged in STATE — preserve that
  note exactly.
- ATTACK-PLAN.md — Sol's current authoritative blocks sit atop the local file.
- ATTACK-REVIEW-2026-11-14.md — NEW local file (the dated Series B review);
  add it to the repo.
- BENCHMARKS.md, LESSONS.md, PLAYBOOK.md, BASE-TYPES.md, TEMPLATES.md,
  README.md — locally aligned by Sol at closeout; prefer local where they
  differ from the remote's first commit.

**Remote holds (Fin-side additions the local folder predates):**
- ORCHESTRATION.md (the RSI system staffing/frame-economy doc, JJ's brief).
- COLLAB.md (records-vs-rules commit discipline).
- The Series B review block, amended ability policy, Rage 4 gate, and the
  Series C package spec now in ATTACK-PLAN.md (commit 455cd2d + the 6+6
  dragon-group fix) — Sol confirmed these verbatim in chat; where the local
  ATTACK-PLAN and the remote differ in wording, the substance was agreed by
  both sides, so merge for consistency and flag any real conflict to Fin
  rather than silently picking one.

**Standing facts the merge must not lose:** B2 NOT passed; no reliable-2-star
claim; Series C not started (package comparison, new policies unvalidated);
Treasury 2.2M Gold is a receipts inference only — balance/capacity still need
a live inspection. Per JJ's AGENTS rule, git operations on the PC are yours
alone — Sol ran none and preserved everything locally for this merge.

## Rulings after Sonnet's pre-merge diff (Muse, 2026-11-14)

Sonnet's diff (scratch clone at c680bf4 vs Sol's local folder) showed the
merge is NOT mechanical. Rulings, per file — the merge is built in scratch
and shown to Muse. (JJ clarified 2026-11-14: the fresh-yes-before-push rule
belongs to his CODE projects, NOT to this Clash repo — pushes here follow
COLLAB.md discipline without a per-push JJ gate.)

- **CHARTER.md — UNION.** Local's "GPT Tier 1 earned" is the current fact
  (the remote's "Not yet" is a stale pre-ruling snapshot). Remote's
  two-model-seat / supervised-hands section is a later standing rule local
  lacks — include it. Sonnet drafts the union; Muse rules on the diff.
- **TERRA-SCOPE.md — LOCAL WINS as base.** Sol's per-section table carries
  live first-use evidence and stop conditions; the remote is Muse's older
  pre-live draft. Any scope item present in remote but absent in local gets
  listed in the conflict table for a ruling — never silently dropped.
- **DAILY-ROUTINE.md — UNION.** Local structure; insert remote's three
  substantive amendments (Tier-0 authorized exceptions, Forge free-slot
  item, Treasury-withdrawal rule); renumber cleanly.
- **PRIORITIES.md — trivial.** Normalize to ASCII arrows, keep status marks.
- **ATTACK-PLAN.md — REMOTE BASE + GRAFT.** The remote carries the Series B
  review and Series C spec as Sol confirmed them line-by-line in chat
  (incl. the precision fixes and the 6+6 dragon groups). Graft local-only
  blocks in, each listed in the conflict table; wording conflicts on the
  review/Series C resolve to the chat-confirmed text, deviations flagged.
- **Local-only files:** ATTACK-REVIEW-2026-11-14.md, SOURCE-CHECKS-2026-11-14.md,
  and CLAUDE-LOCAL-SUPPLEMENT-2026-11-14.md are ADDED to the repo. The stray
  jpg is identified in the conflict table before any decision. The archives/
  and clash-of-clans-research/ folders stay LOCAL — they are not this repo's
  contents.
