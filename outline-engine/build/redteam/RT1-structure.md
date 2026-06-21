# RT1-structure.md — Hostile Structural / Continuity Audit
*Auditor: RT1. Target: 49-ep cozy-LitRPG outline (The Monster Nursery, Book 1).
Posture: adversarial. Every claim verified against source files; non-issues marked "checked: clean."
Tags: **[KILL]** breaks reader trust / hard contradiction · **[MAJOR]** real flaw, fixable ·
**[MINOR]** nitpick.*

---

## SUMMARY COUNTS
- **[KILL]: 2**
- **[MAJOR]: 4**
- **[MINOR]: 5**

---

## [KILL] FINDINGS

### [KILL] 1 — The Pocket Phoenix is simultaneously "placed in Arc 2" AND a permanent resident through Ep49. The pipeline's central boast ("every foster placed, list empty") is FALSE.
**Locations:** `STATSPINE.md` L172 (Arc-2 Phoenix row: "70% steady @19, then *placed*-ready") vs L195 (Arc-3 Phoenix row: **"PLACED-pending → *placed in Arc 2 window* (closed loop; no Arc-3 movement)"**); `FRICTION-SCHEDULE.md` L61 ("**fosters gone except Phoenix**") + cast rows for Eps 38–49 (Phoenix present every episode); `OUTLINE.draft.md` L277/325 ("placement-ready"/"placed-ready"); `scenes/ep-20.md` ("The Phoenix stays steady"); `scenes/ep-41.md` (pipeline "proven IN FULL… first send-off Slime@20 → last send-off Kettle@41; **no name unsent**; **placement list: empty**").
**The break:** The cast bible (`ARCHITECTURE.md` L236, `rooms-bible.md`, `CANON.md` #6) classes Phoenix as a **fostered→PLACED** transient. `L-PHX` closes at Ep19 only as "placement-**ready**" — Phoenix is never actually sent off in any episode. STATSPINE's Arc-3 row then *asserts* Phoenix was "placed in Arc 2," but **no Arc-2 send-off episode exists** for it (the only Arc-2 send-off is Slime@20), and FRICTION-SCHEDULE keeps Phoenix physically in the house through the finale (Ep49: "Cockatrice×Phoenix… Phoenix into one happy ash-puff"). Ep41 then claims the placement list is empty and every foster sent onward — which cannot be true while a foster (Phoenix) is on-page at Ep49. **A foster is both placed and never placed.** This is the most dangerous finding: it voids the book's signature emotional engine (the send-off pipeline "proven in full") on a simple roster fact a reader tracks effortlessly.
**Fix direction:** Pick one. Either (a) re-class Phoenix as a 6th permanent resident (it bonds to Cinder, never matched) and strike STATSPINE L195 "placed in Arc 2" + soften Ep41's "every foster placed" to "every foster *intended for placement*"; or (b) give Phoenix an actual on-page send-off episode and remove it from the Arc-3/Arc-4 cast rosters. Current state contradicts itself three ways.

### [KILL] 2 — Cinder's Arc-4 presence contradicts the friction schedule's hard departure ("Cinder ≤33").
**Locations:** `STATSPINE.md` L210 (Arc-4 row: **"Bond: Cinder 72% → 80% … parting deferred to Bk2"** — requires Cinder PRESENT and tended across Eps 38–49); `scenes/ep-45.md` L28 ("she breaks off… to steady **Kettle and Cinder** and the Phoenix-anchor by hand") vs `FRICTION-SCHEDULE.md` L11 ("**Cinder ≤33**"), L55 ("Cinder (DEPARTS)" @33), and the Arc-4 durability note L80 ("Cinder's frenemy [retires] at Ep33"; "fosters gone except Phoenix" — Cinder is not in any Ep34–49 cast row).
**The break:** STATSPINE has Cinder living in the house through Ep49 with a rising bond (72→80) because the **send-off is deferred to Book 2** — meaning the *match is sealed* (Ep33) but Cinder physically **stays**. FRICTION-SCHEDULE instead treats Ep33 as Cinder's departure and excludes him from the entire Arc-4 cast. So the binding stat contract says "Cinder present, bonding, Arc 4" and the chemistry-schedule says "Cinder gone after 33." `scenes/ep-45.md` sides with STATSPINE (Cinder present, steadied by hand). The two source-of-truth files disagree on whether a core creature is in the building for the climax.
**Fix direction:** Since "send-off carried to Bk2" is the deliberate design (ARCHITECTURE §2D.1 note), Cinder **stays**. FRICTION-SCHEDULE is wrong: change the legend to "Cinder present 2–49 (match sealed @33, parting → Bk2)" and add Cinder to the Arc-4 cast rows / give him core-creature friction beats. As written, Arc 4 also loses a planned humor source the durability note assumed was gone.

---

## [MAJOR] FINDINGS

### [MAJOR] 1 — Ep45 reanimates Kettle, who departed at Ep41 (internal contradiction with Ep44).
**Locations:** `scenes/ep-45.md` L28 ("steady **Kettle** and Cinder and the Phoenix-anchor by hand") vs `scenes/ep-44.md` L27 ("except **Kettle's placed now, Ep41**, so that one's quiet, a small mercy") and `LOOPMAP.md`/`STATSPINE.md` (`L-KETTLE` closes Ep41, "PLACED ~75%").
**The break:** Ep44 correctly notes Kettle is gone (placed @41) and uses that as a plot beat (one fewer creature to calm). One episode later, Ep45 has Liora hand-steadying Kettle during the seizure. Kettle used after its departure episode — a direct creature-availability error, and self-contradictory with the immediately prior scene file. (Slime ≤20, Kettle ≤41 are stated availability bounds in FRICTION L11; Ep45 violates the Kettle bound.)
**Fix:** Strike "Kettle and" from `ep-45.md` L28; the creatures to steady are Cress, Cinder (if kept), Phoenix, Cockatrice.

### [MAJOR] 2 — Acting-Matron rank desync between CADENCE arc tables and STATSPINE (@24 vs @33).
**Locations:** `CADENCE.md` L68 (Ch24 cell still reads "Acting Matron *pending* (lands @33…)") — partially corrected — but the *historical* defect is documented as RESOLVED-by-reviser in `OUTLINE.draft.md` L660–662 / L693 and `ARCHITECTURE.md` Promise Ledger L288 still lists L-LIORA progress marker "**24 Acting Matron**."
**The break:** STATSPINE (binding) + arc files land Acting Matron @33 (gated on Archive@31). The reviser claims CADENCE was fixed, but `ARCHITECTURE.md`'s immutable Promise-Ledger row for `L-LIORA` still carries "24 Acting Matron" as a progress marker, which now mis-states the gate. Low reader-facing risk (it's an internal marker), but it's a live cross-file inconsistency in the file declared "IMMUTABLE / source of truth."
**Fix:** Change ARCHITECTURE L288 marker "24 Acting Matron" → "24 Acting-Matron *pending*; 33 actual." (Note: ARCHITECTURE is marked immutable, so flag for the canon owner rather than silent edit.)

### [MAJOR] 3 — Habitat-Stability Arc-1 internal chain has an uncaused +10 jump at Ep12.
**Locations:** `OUTLINE.draft.md` Ep1 (Hab 2→12), Ep5 (12→20), Ep8 (20→24), **Ep12 (24→34)**; `STATSPINE.md` L145 (Arc-1 EXIT 34).
**The break:** The Arc-1 exit (34%) is reached by a single **+10 leap at Ep12** whose only named cause is "First Inspection survived." Every other Hab move in the arc is +2…+8 tied to a room/mechanic; a +10 step with no structural unlock (no room unlocks at Ep12) reads as a number pushed to hit the target. Compare the Arc-2 tally, where the engine went to great lengths (an Ep23 +1 idle-tick) to reconcile a *1-point* gap — yet a 10-point inspection bump passes unexamined. Not a boundary discontinuity (entry=exit chains hold), so MAJOR not KILL, but it's an on-page "number jumps without proportionate cause" (the G3 rule the spine claims to enforce).
**Fix:** Either distribute the gain across Eps 9–12 with named causes, or add an explicit Ledger cause for the inspection-driven Hab surge (e.g., "certified-safe re-rating").

### [MAJOR] 4 — `L-FEAR` progress marker "30 a townsperson softens" is mis-scheduled; the softening beat is Ep29, and Ep30 is a different loop's close.
**Locations:** `ARCHITECTURE.md` Promise Ledger L292 (`L-FEAR` markers: "**30** a townsperson softens · 36 public handling") vs `OUTLINE.draft.md` Ep29 ("one townsperson pockets it instead of fleeing" = the softening) and Ep30 (East Wing opens / `L-SPORE` closes — no L-FEAR softening beat).
**The break:** The immutable Promise Ledger pins L-FEAR's "townsperson softens" progress to Ep30, but the outline lands it at Ep29 (Public Figure), and Ep30 is wholly occupied by the SPORE→EAST handoff. A planted progress marker pays one episode off its declared slot. Minor reader impact, but it's a Promise-Ledger schedule the brief asks me to verify against payoff episodes — and it doesn't match.
**Fix:** Update ARCHITECTURE L292 marker "30" → "29" (the pocketed pebble).

---

## [MINOR] FINDINGS

### [MINOR] 1 — Cinder split-rendering label (intake Ep2 vs room/loop Ep4) is cosmetic, but STATSPINE/ARCHITECTURE still disagree on the canonical "arrives" episode.
`ARCHITECTURE.md` L228 ("Cinder | **4** (canon)") and L327 ("L-CINDER… Ep4") vs `STATSPINE.md` L151 / `scenes/ep-02.md` (intake Ep2, Bond live 0→9% from Ep2). Documented and reconciled as F3/R4; bond chain is continuous (0→9→20→…→44). Checked: not a stat break — the two-arrival rendering is internally consistent and the number never jumps uncaused. Cosmetic only.

### [MINOR] 2 — Cockatrice×Slime synergy "realized" Ep27 uses Slime after its Ep20 departure (mitigated).
`FRICTION-SCHEDULE.md` L49 (Ep27 "COCKATRICE×SLIME-fix realized"). Slime departed Ep20. **Checked: defensible** — the beat is pebbles corralling the Slime's *orphaned leftover puddles* (seeded Ep21), not the live creature. Same residue-not-creature dodge as Ep34. Borderline; flag only if a reader expects the Slime on-page. (For contrast, `scenes/ep-34.md` handles the identical issue cleanly and explicitly with a "saved residue in a stoppered jar" note — **checked: clean**, no Slime-availability break at Ep34.)

### [MINOR] 3 — Hearthglow Arc-1 micro-chain has an unstated dip-and-recover (Ep2 → ~2, then "back to 5" @Ep6).
`scenes/ep-02.md` spends Hearthglow 4→2 (cooling ring); `OUTLINE.draft.md` Ep6 says "Hearthglow back to 5" without an itemized Ep3–5 refill. Boundary values are fine (Arc-1 exit 9 holds); the within-arc reserve wobble just isn't fully itemized episode-by-episode. Checked: no boundary break.

### [MINOR] 4 — Ward-Mending I "standing Hearthglow upkeep every episode active" (S7@17) is not reflected as a per-episode drain.
`STATSPINE.md` L38 says wards cost standing upkeep "every episode they're active," but the Hearthglow chain only books two −1 ticks in Arc 2 (Ep17, Ep18) and then the ward sits "active" Eps 19–41 with no further per-episode draw until the alcove retires @41. The economy is *described* as continuous but *modeled* as two discrete dips. Defensible as abstraction; flagged because the spine sells Hearthglow as a biting per-episode leash.

### [MINOR] 5 — Book Nook (Stage-8 overlay, unlock ~Ep23) is absent from STATSPINE §1B room ledger, LOOPMAP, and CADENCE's "all 16 room beats" tally.
`OUTLINE.draft.md` L771–773 adds "The Book Nook (unlock ~Ep23)" and `rooms-bible.md` L150 lists it, but `STATSPINE.md` §1B (rooms) doesn't carry it and `CADENCE.md` L210 still asserts exactly "16 room beats." A late-added room that no binding ledger counts. Cosmetic (it grants Comfort +1 / Soothing-Song support), but it means the room count and Comfort math in the binding files are one room short of the overlay.

---

## VERIFIED CLEAN (adversarially checked, no break found)
- **Loop integrity / LIFO:** All 17 loops open-before-close; every nested inner loop closes ≤ its outer parent (spot-checked the tight pairs: L-ALARM d4@44 < L-INSPECT d3@45; L-CINDER d4@33 < L-PLACE d3@41; L-SPORE d4@30 < L-EAST d3@46). Same-depth peers (L-SPORE@30 before L-CINDER@33) don't nest — legal. **Exactly one dangle past Book 1 (`L-SERIES`, depth 0).** Checked: clean.
- **Stat chaining at arc boundaries:** Comfort 1→4→5→7→9; Compliance 13→41→58→66→100 (monotonic); Hearthglow 4→9→7→12→3; every Arc-N entry = Arc-(N-1) exit value-for-value. Checked: clean.
- **Ability-before-unlock (skills/rooms):** Strict CANON skill order preserved; no skill resolves a beat before its row (Soothing Song held @23 not used until ≥60% bonds; Advocacy@34 not invoked before 34; Archive lore-win not before 31; no Ward-Mending before 17). Cockatrice Soothing-Song fuse gated correctly to Ep43 (bond 58→78 crosses 60 there, not Ep38). Checked: clean.
- **Room buildable order:** Moonwell→Basking Nook→Welcome Desk→Gargoyle mech→Brew Pool→Tea Room→Resonance Hearth→Fledgling Wing→Mending→West Wing→Porch→Kennel→Pebble→Lull→East Wing→Archive — sensible dependency order (hospitality before matching; larder-spore before East Wing). Checked: clean.
- **Season monotonicity:** late-winter (1–12) → spring (13–24) → late-spring/midsummer (25–37) → high summer (38–49); no regression. Checked: clean.
- **Cockatrice (≤ n/a, core), Slime ≤20, Kettle ≤41 (modulo [MAJOR]1), Kraken 9+, Corehound 22+, Cockatrice 26+** arrival bounds otherwise respected in FRICTION-SCHEDULE.

**— END RT1-structure.md —**
