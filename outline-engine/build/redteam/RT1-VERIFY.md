# RT1-VERIFY.md — Re-audit after the red-team fix pass
*Auditor: RT1-VERIFY. Posture: adversarial; no rubber-stamp. Each original finding marked
CLOSED / PARTIAL / STILL-OPEN with file+line/quote evidence; NEW issues appended.*

---

## ORIGINAL FINDINGS

### [KILL] 1 — Pocket Phoenix never sent off → **CLOSED**
The Phoenix is now consistently a **foster→PERMANENT** resident that **declines placement**.
- `scenes/ep-19.md` L4/L48–53: three trial placements attempted, all declined ("self-combusted
  with strangers; re-lit only on return"); status amended `placement-ready → DECLINES PLACEMENT`;
  "Reclassification: foster → PERMANENT RESIDENT (1st)." `L-PHX` closed as *steady, home*.
- `scenes/ep-41.md` L17 / L8 / L54: the boast is corrected on-page — **"Three fosters placed
  and thriving"** (Slime@20, Cinder@33, Kettle@41) **"and one foster home, found right here"**
  (the Phoenix). "Three sent onward; one stayed." The old "every foster placed / placement list:
  empty / no name unsent" is reframed honestly (the list is empty *because the Phoenix took
  itself off it*, not because it was placed).
- `CANON.md` L104 and `STATSPINE.md` addendum L324 both carry the Phoenix-permanent reclass.
- Phoenix present through finale (`FRICTION` Ep38–49 CORE rows; `ep-49.md` L8) — now **consistent**
  with permanence rather than contradicting a "placed" claim.
**Verdict: the three-way contradiction is resolved; the boast is honest. CLOSED.**

### [KILL] 2 — Cinder Arc-4 presence contradiction → **PARTIAL (still-open residue)**
The scene-level fix is in and correct, but two binding/again-scene artifacts still carry the
**pre-fix** "Cinder present & ticking in Arc 4" rendering.
- FIXED on-page: `scenes/ep-33.md` L1–14 — Cinder is **matched AND sent off on the page**
  (DEPARTS @33; "Bond frozen at the Ep33 value; no Arc-4 Cinder ticks; removed from Arc-4 rosters
  and ep-45"). `scenes/ep-45.md` L8 / L56 — Cinder explicitly **absent** ("Cinder departed @33 …
  neither is present; no Arc-4 Cinder/Kettle ticks"). `FRICTION-SCHEDULE.md` Arc-4 rows (Ep38–49)
  carry **no Cinder** (last appearance Ep33 "(DEPARTS)", L55). STATSPINE addendum L321–324 orders
  the freeze.
- **STILL-OPEN #1 — STATSPINE Part-2 Arc-4 table body not propagated.** `STATSPINE.md` **L210**:
  `**Bond: Cinder** | 72% | **80%** | (match seeded; parting deferred to Bk2)`. This is the
  literal pre-fix text the addendum supersedes — it lists Cinder with an **Arc-4 entry (72),
  exit (80), and an in-Arc-4 tick**, plus "parting deferred to Bk2" (the rendering ep-33's header
  calls "SUPERSEDED"). The binding contract row directly contradicts the addendum 8 lines below it
  (L321) and ep-33/ep-45.
- **STILL-OPEN #2 — two Arc-4 scene entry-states still carry Cinder as a present, bonded resident.**
  `scenes/ep-38.md` L8 (and the L2 header): Arc-4 carried bonds = "Cress 74, **Cinder 72**, Bertram
  70, Kraken 68, Kettle 62, Corehound 66, Cockatrice 58" — Cinder listed as an Ep38 resident bond,
  though he departed @33. `scenes/ep-47.md` L8: "Cinder ~80 **(match seeded, parting → Bk2)**" —
  again the superseded rendering, listed among Ep47 carried bonds.
**Verdict: the on-page contradiction the KILL targeted (ep-45) is CLOSED, but the roster freeze
was not fully propagated — STATSPINE L210 + ep-38 L8 + ep-47 L8 still present Cinder as an Arc-4
resident with a deferred-to-Bk2 parting. PARTIAL.**

### [MAJOR] 1 — Kettle reanimated Ep45 → **CLOSED**
- `scenes/ep-45.md` L8 / L28 / L56: Kettle **departed @41** and is **absent** from Ep45; the
  Arc-4 alarm/shriek function explicitly **transfers to the Corehound alarm-head** ("the alarm is
  the Corehound alarm-head, the permanent synergy partner — NOT Kettle, who placed @41").
- `scenes/ep-41.md` is Kettle's send-off (departs @41); `scenes/ep-44.md` L27 still correctly uses
  "Kettle's placed now, Ep41, so that one's quiet" as a plot beat.
- No Ep45 hand-steadying of Kettle remains. **CLOSED.**

---

## NEW-CONTRADICTION HUNT (audit clock, capstone unlocks, roster changes, Cull Ledger)

### NEW-1 [MAJOR] — ARCHITECTURE Promise Ledger still encodes the superseded Cinder design
`ARCHITECTURE.md` is marked IMMUTABLE; its red-team addendum (L529–541) covers Cull Ledger,
Supersession, and Pike — but **does NOT carry the B2 Cinder/Kettle roster freeze.** As a result
the immutable body still reads the old design:
- L295 `L-CINDER` row: "**~33 Cinder's match *seeded but its send-off carried to Bk2***".
- L304–311 the explicit `L-CINDER` resolution note: "**E's carry … its *parting* deferred**".
- L327 nesting diagram: "`L-CINDER  depth 4 — Ep4 → match ~33 / send-off → Bk2`".
This is the same superseded "match @33, send-off deferred" model that ep-33 now overrides with an
executed departure. The immutable source-of-truth and the fixed scenes/STATSPINE-addendum now
disagree on whether Cinder's send-off happens in Book 1. Flag for the canon owner (ARCHITECTURE is
immutable — needs an addendum line, not a silent edit), consistent with how the original audit
handled the L288 immutable-marker issue.

### NEW-2 [MAJOR] — the Cinder freeze is asserted in addenda but not applied in the chained tables
Same root as KILL-2 STILL-OPEN, called out as its own propagation defect because it spans three
files: STATSPINE Part-2 Arc-4 row (L210), ep-38 entry-state (L8), ep-47 entry-state (L8) all still
chain a *live, ticking* Cinder bond (72→80) through Arc 4. The STATSPINE chaining-audit line (L218,
"every Arc-N entry = prior exit … PASS") was re-run against the **unfrozen** numbers, so it "passes"
only because the table was never frozen — i.e., the freeze the addendum mandates is contradicted by
the very audit that claims to validate it.

### NEW-3 [MINOR] — FRICTION Arc-4 boundary banner slightly early
`FRICTION-SCHEDULE.md` L61 prints "ARC 4 BOUNDARY: fosters gone except Phoenix" **above** the Ep38
row, yet the Ep38–40 CORE rows still (correctly) list **Kettle**, who legitimately departs @41.
Not a roster break (Kettle present 38–41 is correct), but the "fosters gone" banner reads three
episodes early. Cosmetic; flag only.

### Spot-checks that came back CLEAN
- **Capstone unlock chain (Theme C) chains in-sequence, each with upkeep:** Advocacy II @43 (builds
  on Advocacy@34, no tier skipped — `ep-43.md` L7); Habitat "Maintained→Self-Sustaining" @44
  (`ep-44.md` L5/L40, upkeep = stability hostage to Bertram's belonging); Sanctuary Charter tier
  @47–48 (`ep-47.md` L8); Bestiary/Codex Complete + Sanctuary Network (dormant) @48–49 (`ep-49.md`
  L8). No capstone ability used before its unlock. **Clean.**
- **Cull Ledger (A1) chains:** seeded `ep-01.md` L7 (refusal #1 logged) → `ep-03.md` L7/L50
  ([REDACTED] in the *same* ledger) → Archive @30/31 → paid `ep-47.md` L8 ("why her" = the Ledger
  logged her choice; detected, not assumed). **Clean.**
- **Supersession (A2) chains:** seeded `ep-06.md` L7/L36 (plant 1; 1842 charter highest) → Ep8/Ep17
  (`ep-17.md`) → paid `ep-45.md` L40–46 (charter supersedes the seizure). **Clean — a planted tool,
  not climax magic.**
- **Kettle roster everywhere else:** present only through Ep41; Arc-4 alarm reassigned to Corehound;
  no post-Ep41 Kettle presence in any scene (38/39/40 references are all pre-departure). **Clean.**
- **Audit clock (D2):** live foreground in `ep-33.md` (Request 3 incoming on the title) and Ep39;
  no dangling loop introduced. **Clean.**

---

## SUMMARY
- **KILLs CLOSED:** 1 of 2 fully (Phoenix). KILL-2 (Cinder) is **PARTIAL** — its on-page target
  (ep-45) is closed, but the roster freeze wasn't propagated to STATSPINE L210, ep-38 L8, ep-47 L8.
- **MAJOR (Kettle Ep45):** CLOSED.
- **STILL-OPEN:** Cinder is still rendered as a live, Arc-4-ticking resident (Bond 72→80, "parting
  deferred to Bk2") in STATSPINE Part-2 L210, ep-38 L8, ep-47 L8, and in immutable ARCHITECTURE
  (L295/L304–311/L327).
- **NEW issues:** NEW-1 (ARCHITECTURE immutable body still encodes superseded Cinder design — needs
  a canon-owner addendum), NEW-2 (freeze asserted but not applied in the chained tables; STATSPINE
  chaining-audit "passes" only because the freeze was skipped), NEW-3 minor (FRICTION "fosters gone"
  banner 3 eps early).
- **Net:** the fixes are real and mostly land, but the Cinder roster freeze is half-propagated — the
  most reader-trackable of the two kills is not fully closed.

**— END RT1-VERIFY.md —**
