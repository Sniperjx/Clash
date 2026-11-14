# AMENDMENTS v1.1 — 2026-11-14 (issued by Muse after GPT's setup review)

GPT's setup pass caught five real defects in v1.0. All five are fixed in the v1.1 files.
The original v1.0 ZIPs are preserved unchanged — archive them; v1.1 supersedes v1.0.

1. **Walls need a free builder.** v1.0 said "dump overflow into walls whenever all
   builders are busy" — impossible; walls are instant but still require a free builder.
   Corrected rule in PRIORITIES Tier E and CHARTER: walls are a free-builder activity;
   spend overflow on walls when a builder is free, never delaying a queue item and
   never spending resources reserved for the next queue item.

2. **Army of Record is now exact.** PLAYBOOK.md gains "Army of Record v1":
   12 Dragons + 2 Dragon Riders + 6 Balloons (320 housing); 4 Rage + 3 Freeze
   (11 spell space); Queen / Warden (air) / Minion Prince / Royal Champion;
   Battle Blimp. Derived from the research library's TH17 Dragons/Hydra sections
   [community]; it is a starting composition that practice logs may amend.

3. **Benchmark venues defined.** Practice-mode stages use preset armies, so they count
   toward B1 (controls) only — never B2. B2 attempts must use JJ's own army:
   single-player campaign maps (hardest available) or a pre-existing Friendly
   Challenge. B3's real-farming window can revoke a Tier 2 that B2 over-granted.

4. **Ordering fixed: Practice is Tier 1, GPT is Tier 0.** v1.0's "B1/B2 first" phrasing
   contradicted the tier table. Ruling (BENCHMARKS B0): seed sessions #1 and #3 count
   as 2 of 3 B0 sessions; one more full chore circuit in the new format completes B0,
   unlocks Tier 1, and only then do B1 drills and B2 attempts begin. No drill exception
   unless JJ grants one explicitly and it is recorded in CHARTER.md.

5. **Symbols/encoding.** Some v1.0 files arrived with damaged glyphs (a U+001A control
   character, "?" in place of symbols). Meanings, for reading the v1.0 originals:
   the star symbol = attack stars; the checkmark = earned/completed; the arrow =
   "leads to / then". v1.1 keeps symbols minimal; when writing files locally, prefer
   plain ASCII ("stars", "[done]", "->") so nothing corrupts in transfer again.

Also confirmed in setup (no file change needed): the live account check is still
pending (game window closed after the initial inventory), and the account snapshot
remains prior GPT-reported observations, not this session's — first live look is a
re-verification against STATE.md, with drift logged as drift.
