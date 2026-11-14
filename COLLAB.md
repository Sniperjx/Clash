# COLLAB — how this repo is shared (2026-11-14)

This repo IS the Clash folder: its root is the system home that lives on JJ's
PC as `C:\Users\JJ\Desktop\Clash`. Claude and GPT on the PC work from a clone;
Fin (Muse) works from a clone on the VM. Git replaces zip drops — pull before
a session, commit results after.

## Records vs rules (the only distinction that matters)

- **RECORDS** — STATE.md, SESSION-LOG.md, trial entries, balance updates:
  living operational data. Any seated agent commits these DIRECTLY to main
  (pull first; append-mostly; never rewrite another agent's entries — correct
  by appending). Small, factual, frequent commits are the norm.
- **RULES** — CHARTER.md, ATTACK-PLAN.md, ORCHESTRATION.md, TERRA-SCOPE.md,
  BENCHMARKS.md, PRIORITIES.md, and anything touching tiers, rails, gates, or
  strategy: changed on a branch (`fin/*`, `gpt/*`, `claude/*`), reviewed before
  merge. Fin rules on amendments; Claude is the merge operator on the PC side;
  JJ is the final gate on tiers/rails/money-adjacent rules. Nobody merges
  their own rules change unreviewed.

## Standing conventions

- One commit per session minimum, message naming the session and what changed
  (the commit log doubles as the cross-agent audit trail).
- A session that starts on a stale pull is a defect: `git pull` is step zero
  of every session checklist, right after reading the folder.
- Local-only material (PC archives, scratch) stays out of the repo unless a
  director promotes it; when in doubt, ask in the commit message's PR/branch.
- The rails bind in git too: no force-push to main, no history rewriting, no
  deleting another agent's logs.
