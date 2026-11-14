# DAILY-ROUTINE — The Itemized Regular Work (v1.3)

Everything an agent does on a normal visit, itemized. Three kinds of item — keep them
distinct, they have different permissions:

- **[COLLECT]** — pure collection. No decision, no cost. Tier 0.
- **[CLAIM]** — claiming a reward. Free, but sometimes involves a CHOICE (which reward,
  which slot). Tier 1. Log what was claimed and which option was picked.
- **[CHECK]** — look only, no action. Any tier. Feeds STATE.md.

Items tagged **[VERIFY LIVE]** rest on library claims that no agent has confirmed on
JJ's actual account yet. First session that touches one: confirm or correct the item
in this file and log the finding. Until verified, treat the item as "look for it,"
not "it definitely exists."

**Tier-0 authorized exceptions (v1.3.1 ruling):** two routine actions are not literally
cost-free, and are pre-authorized inside Tier 0 anyway: (a) obstacle removal, which
costs a small amount of Elixir; (b) the Clock Tower boost, which is an activation, not
a collection. These exceptions extend to NOTHING else — no potions, no gems, no other
spend of any kind rides along with them.

## Every session — Home Village [COLLECT]

1. Loot Cart (if present) — tap, confirm balances rose.
2. Gold Mines — every mine showing a collection bubble.
3. Elixir Collectors — every collector showing a bubble.
4. Dark Elixir Drills — every drill showing a bubble.
5. Obstacle circuit — normal obstacles ONLY (trees, bushes, stumps, mushrooms) and
   Gem Boxes. **NEVER event obstacles** (CHARTER rail). Note any obstacle you were
   unsure about instead of clearing it.
6. Treasury — do NOT habitually empty it. Withdrawal follows CHECK item 20's rule
   (room in storages + a planned queue spend), otherwise leave it banked.

## Every session — Builder Base [COLLECT]

7. BB Gold Mine + Elixir Collector bubbles.
8. Gem Mine — collect accumulated gems (this ADDS gems; always allowed).
9. Clock Tower boost — free boost when available [VERIFY LIVE: current BB 2.0 flow].
   Classified [COLLECT]: it costs nothing and makes no choice.

## Every session — [CHECK]s (no actions)

10. Builders: how many free? If one is free and Tier 1+ applies, that's a PRIORITIES
    decision (see below), not a routine item.
11. Laboratory: idle or running? If idle, ditto.
12. Army: is the army of record trained for the next session's work?
13. Heroes: all present/regenerating? Note anyone down.
14. Shield/Guard status and any "you were attacked" results worth logging (loot lost).
15. War / Ranked status: LOOK ONLY. Never act (Tier 3).
16. Forge FREE daily slot [officially checked: refills every 24h, separate from
    resource-conversion slots]: CLAIM it — ruled 2026-11-14 (Muse, under JJ's
    Capital-chores workstream) as a pure collection: free Capital Gold, no resource
    cost. It is the ONLY Forge action in routine scope. Converting resources is a
    spend (see Decisions below) and contributions of Capital Gold are Sol-only.
17. Builder Base defense loot / loot cart state: note it; collection flow [VERIFY LIVE].
18. Achievements, inbox, calendar / returning-player rewards, event pages: note what
    is claimable, its cap/expiry, and whether claiming involves a CHOICE. Claims
    themselves follow the [CLAIM] rules (Tier 1) — a choice node means log the pick.
19. Helpers (Builder's Apprentice / Lab Assistant): note current assignments only.
20. Treasury: Star Bonus deposits land in the Treasury [officially checked]. Withdraw
    ONLY when storages have room AND a queue spend is planned — withdrawing into full
    storages wastes the overflow. Otherwise leave it banked and note the amount.

## Daily — [CLAIM]s (Tier 1; log every claim)

21. Daily Tasks rewards — Daily Tasks replaced Season Challenges, with a free track
    incl. chests [officially checked: task cards can STACK, and reward tracks contain
    CHOICE nodes — log which option you pick at every choice node, per the pick rule
    in Decisions below]. Claim free-track rewards only. Paid pass: skip, log it exists.
22. Trader free item — IF the Trader shows an item priced FREE, claim it [VERIFY LIVE].
    Anything priced in gems or Raid Medals is a SPEND, not a claim: skip it. (Raid Medal
    spends are Tier 3 decisions; gem spends are banned outright.)
23. Event track free rewards — claim free-tier event rewards when present [VERIFY LIVE:
    current event + track shape]. Paid track: skip.
24. Star Bonus — deposits to the Treasury automatically [officially checked]; there
    may be no separate "claim" step at all. It is earned by attacking (stars in
    Battles/Ranked), so it is not a chore-session item. Never attack JUST to finish
    it below Tier 2. Moving it out of the Treasury follows CHECK item 20's rule.

## Decisions the routine must NEVER absorb (stop, use the tier rules)

- Starting any upgrade or research — PRIORITIES queue + Tier 1 only.
- Forge slots (Clan Capital): converting home resources is a SPEND of resources.
  Default: leave the Forge alone unless a PRIORITIES/STATE note says otherwise.
- Clan Games reward picks, Season-end rewards with a choice: pick the option the
  account needs most per STATE.md (resources when storages are low, ore when an
  equipment upgrade is queued); log the pick and the reason. If genuinely unsure, leave
  it unclaimed and flag it for JJ — unclaimed beats wrong.
- Donations: Tier 1 rules in PLAYBOOK.

## Weekly rhythm (awareness only — most are Tier 3 to act on)

- Raid Weekend (Fri–Mon): Tier 3. Routine may note it is live; never raid without JJ.
- Clan Games (monthly, when live): participation is Tier 3; reward claims are [CLAIM].
- Season reset (monthly): expect reward choices; apply the pick rule above.

## Session shape (target: chores circuit under ~10 minutes)

Open game -> read STATE.md notes -> [COLLECT] home -> [COLLECT] BB -> [CHECK]s ->
any earned-tier work (upgrades/practice) -> [CLAIM]s available today -> log -> STATE.

## v1.3 local review corrections (supersedes conflicting wording above)

- Normal-obstacle removal is an explicitly authorized Tier 0 resource cost, not a no-cost collection. Verify normal identity and displayed cost; never gems, event or ambiguous obstacles.
- Clock Tower activation is a free boost, not resource collection. Verify free status; no potion, gem skip, or purchase. Availability unverified.
- Treasury: inspect room and need before withdrawing. Star Bonus is credited there; a separate claim action is not assumed.
- Do not blindly Claim All: check inventory room, overflow, choices, expiry, and whether anything starts an item timer. Never sell/use magic items, convert ores or spend currencies as collection.
- Expand CHECK ONLY inventory to free daily Forge slot, BB defensive-loot cart, achievements, returning-player/calendar rewards, inbox/event rewards and helpers. Existing Forge/claim permissions remain unchanged. Record available/unavailable/locked/unknown and current reset/expiry shown in-game; do not invent availability or timers. See SOURCE-CHECKS-2026-11-14.md.

Fin v1.3.1 final Treasury rule: withdraw only with storage room AND a planned queued spend; otherwise keep it banked. Verified in #6: home collection, BB gold/elixir and Gem Mine; other VERIFY LIVE surfaces remain pending.


## Supervised Terra routine amendment - 2026-11-14
See TERRA-SCOPE.md for controlling checklist,first-use reviews and stops. Pure FREE daily Forge slot may be collected after Sol inspects the first live flow;this supersedes prior check-only/wait-for-ruling wording for that slot only. Resource conversions and contributions are separate spending decisions;raids remain Tier3. Builder Base includes collectors,Gem Mine,free Clock Tower and verified normal obstacles;no Builder Base PvP work. Free claims require zero price,no choice and no overflow;donations require Sol-reviewed exact known troop/count from surplus,without gems or quick training.
