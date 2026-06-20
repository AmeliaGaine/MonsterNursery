# SEAM-REPORT — Scene-Level Seam Weld (49 episodes)

*Verification of `scenes/ep-01.md … ep-49.md` against the locked schedule in
`CADENCE.md`. Source of truth: CADENCE (per-chapter cookie / out / micro-structure),
honoring the documented seam/F-fixes (Ch25→competence, Ch38→competence, Ch39→relationship,
Ch46→relationship). Date: 2026-06-20.*

---

## Per-check results

### Check 1 — Out-type vs CADENCE
**PASS (49/49 match the locked out column, as rendered) — with one commanded conversion at Ep42 (see "Files changed" + "Flags").**

All files deliver the out-type their CADENCE row assigns:
- Arc 1: 1 soft · 2 warm · 3 hard · 4 warm · 5 soft · 6 warm · 7 soft · 8 hard · 9 warm · 10 soft · 11 warm · 12 warm(climax) ✓
- Arc 2: 13 soft · 14 warm · 15 soft · 16 warm · 17 soft · 18 hard · 19 warm · 20 warm · 21 soft · 22 hard · 23 warm · 24 soft(climax) ✓
- Arc 3: 25 soft · 26 warm · 27 soft · 28 warm · 29 soft · 30 hard · 31 soft · 32 warm · 33 warm · 34 hard · 35 warm · 36 soft · 37 warm-with-ache(climax) ✓
- Arc 4: 38 hard · 39 soft · 40 warm · 41 warm · **42 → warm (was hard-hook; converted per work order)** · 43 warm · 44 soft · 45 hard · 46 warm · 47 soft · 48 warm · 49 warm-then-door(climax)

NOTE on Ep42: the **CADENCE table (line 116) and its F2 narrative (lines 199–200) lock Ch42's
out as `hard-hook`** (K& micro, "live seizure clock kept via hard-hook out"). The work order's
KNOWN-ITEM, however, directs Ep42 to be rendered as a **warm-out** ("calm-before-the-climax
breath"). These two signals conflict. The commanded warm-out conversion was applied; the
conflict + its G6 consequence are logged below (Flag 1).

### Check 2 — Cookie-type vs CADENCE + 48/48-distinct adjacency (G4)
**PASS.** Every file's cookie matches its CADENCE row (using the locked reassignments
25→competence, 38→competence, 39→relationship, 46→relationship — each annotated in-file).
Adjacency swept across all 48 boundaries: **zero adjacent-duplicate cookie types.** The three
arc seams (12→13 competence→relationship, 24→25 mystery→competence, 37→38 mystery→competence)
and the finale run (45 number-up → 46 relationship → 47 mystery → 48 relationship → 49 competence)
are all distinct. Cookie distribution = mystery 12 · relationship 14 · competence 12 · joke 4 ·
number-up 7 = 49, matching CADENCE.

### Check 3 — Micro-structure (K& vs S&S) vs CADENCE
**PASS (49/49).** Every file's `micro-structure:` header matches the locked K&/S&S schedule,
including all six F2 conversions (Ch15/21/27/36/39/42 = K&) and all five arc-climax S&S beats
(12/24/37/45/49). Book total = 29 K& / 20 S&S = 59% K&, matching CADENCE. **Ep42 was already
K&** in its header — the only thing changed was its out-type, not its micro-structure.

### Check 4 — Hard-hook adjacency / three-warm runs (G6)
- **Hard-hook adjacency: NONE** (hard-hooks at 3, 8, 18, 22, 30, 34, 38, 42→(now warm), 45 — all
  isolated in both the as-locked and the converted state).
- **Three-warm runs (as-locked, Ep42 = hard-hook): NONE.**
- **Three-warm runs (after the commanded Ep42 → warm flip): TWO introduced — 40→41→42 and
  41→42→43.** See Flag 1. This is the central tension of the work order and is logged, not
  silently accepted.

---

## Files changed

### `ep-42.md` — out-type flipped hard-hook → warm-out (minimal, per KNOWN-ITEM work order)
Micro-structure, cookie, loops, and stats were **preserved**; only the out-type and its
supporting prose changed. Specifically edited:
- HTML `<!-- MICRO -->` header comment: `out:hard-hook` → `out:warm`; clock note rephrased to
  state the L-INSPECT seizure/legitimacy clock is held **under** the warm-out (anti-plateau via
  the body, not a hook).
- `**Tags**` line: `🪝 hard-hook` → `🪝 warm`.
- Scene-list parenthetical: `K4→hard-hook out` → `K4→warm-out, the calm-before-the-climax breath`.
- Scene 3 ten: "the door it opens is hard-sized" → "the order is still pending … the calm held
  over a live clock."
- Scene 4 (the ketsu): retitled "Sealed, not safe" → "Sealed, and warm for the night"; the
  hard-hook beat rewritten as a warm-out beat (calm-before-the-climax breath) with the seizure
  clock kept live in the standing case + gathering storm-sky; System box softened from
  "one move left that paper cannot answer" to "the order is still pending — that is tomorrow's
  weather."
- `## Out — hard-hook` → `## Out — warm-out`; both the closing-beat and the out-type-confirm
  bullets rewritten to deliver settle-in warmth with the live clock held underneath (G5), no
  page-turn cliff (G6/heat ≤4).

**Preserved verbatim:** cookie = competence @ ten; micro = K& (F2-converted); loops
(advances[L-INSPECT] / closes[none]); stats (Hearthglow 11→9, Advocacy@34 deployed, Welcome
Desk@5, Public Handling@29, Soothing Song@23 held-not-used, Renown firming toward Regional);
no room/arrival/bestiary/recipe.

**No other files were edited.** All other 48 files match CADENCE as-rendered and were left
untouched (no rewriting of passing material).

---

## Flags logged (not fixed — require cadence-owner adjudication)

1. **Ep42 out-type: work-order vs CADENCE-table conflict, and a resulting G6 three-warm run.**
   - CADENCE's table (line 116) and F2 narrative (lines 199–200) **lock Ch42's out as
     `hard-hook`**, explicitly citing it as the anti-plateau mechanism ("petition hard-hook with
     the seizure clock live"). The work order's KNOWN-ITEM instead directs a **warm-out**.
   - The pre-existing file already matched the CADENCE table (K& micro + hard-hook out) and, in
     that state, the whole book had **zero** three-warm runs and zero adjacent hard-hooks — i.e.
     Ep42-as-locked was *not* a deviation from CADENCE.
   - The commanded warm-out flip was applied (the work order is explicit). **Consequence:** with
     40 (warm) and 41 (warm) both locked warm and immovable, and 43 (warm) locked warm, flipping
     42 to warm creates **two three-warm runs (40-41-42, 41-42-43)** — a G6 violation that did
     not exist before.
   - **Recommendation:** the cadence owner should reconcile CADENCE and the work order. Either
     (a) revert Ep42 to the locked `hard-hook` out (restores G6 cleanliness, matches the
     CADENCE table), or (b) keep the warm-out and re-balance an adjacent locked out (e.g. flip
     Ep41 or Ep43 to soft-hook) to break the three-warm sag. This report does **not** edit
     CADENCE or any episode beyond the commanded Ep42 change.

No other mismatches were found across the 49 files; nothing else was logged.

---

## Summary

- **Out-types:** 49/49 match as rendered (Ep42 converted per order).
- **Cookies:** 49/49 match; all 48 adjacencies distinct (G4 PASS).
- **Micro-structure:** 49/49 match (59% K& book-wide).
- **G6:** hard-hook adjacency clean; the commanded Ep42 warm-flip introduces a 40-41-42 /
  41-42-43 three-warm run — logged as Flag 1 for owner adjudication.

**— END OF SEAM-REPORT.md —**
