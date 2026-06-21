# GUARDRAILS.md — the fail-state checklist (Stage 0 lock)

*Binary checks the Canon + Lane Sentinels run on every write. A FAIL blocks the write.*

## G1 — LANE (cozy stakes)
PASS if: every threat targets **home / found-family / way-of-life** only; never
existential grimdark; never toothless. Conflict-heat ≤ 4. Darkness (the cull-economy)
is aimed *outward at the system* and metabolized into warmth, never aimed at a loved
creature on-page.
FAIL example: a loved creature dies; gore; a threat with no cozy floor; OR a conflict
so frictionless nothing is at stake.

## G2 — NOT-LITERARY (commercial genre fiction)
PASS if: forward motion over interiority; payoffs **delivered**, not withheld as theme;
prose serves the read (no lyrical opacity, no ambiguity-as-virtue); the protagonist's
concrete want is legible every scene.
FAIL example: introspection that stalls plot; a lyrical sentence that asks to be
underlined instead of read through; a withheld meaning standing in for a payoff.
→ Lane Sentinel must return token `COMMERCIAL` (not `LITERARY-CONTAMINATED`).

## G3 — BINDING STAT CONTRACT
PASS if: nothing wins a beat that wasn't unlocked earlier, in sequence; every gain
adds proportionate upkeep / a new problem (no power-creep without cost). Stats chain
continuously across chapters and arc boundaries.
FAIL example: an ability used before its unlock episode; a free power; a stat that
jumps without an on-page cause.

## G4 — COOKIE LAW
PASS if: every chapter pays ≥1 of {number-up, mystery deepened/clue, relationship
beat, landed joke, competence-display}; adjacent chapters don't repeat the same
cookie type.
FAIL example: a chapter that advances nothing the reader can feel.

## G5 — ANTI-PLATEAU
PASS if: a live clock OR a deepening mystery is active in every chapter of every arc;
no run of 2+ chapters with neither.
FAIL example: a slack middle with no rising pressure.

## G6 — NO CLIFFHANGER CRUELTY
PASS if: every chapter AND every arc **resolves its own promise, then opens a bigger
door** (full satisfaction + "the world just got bigger"). Alternate hook-outs and
warm-outs; never two cruel hooks in a row, never three warm-outs.
FAIL example: ending mid-fall with nothing resolved; a cheap fake-out; betrayal of
the cozy contract.

## G7 — AXIS ENVELOPE (the felt-experience contract)
PASS if: every episode clears its per-axis **floors** in `AXIS-ENVELOPE.md` and hits
its ★ foreground spike; AND the book-level **conservation laws** hold (humor mean ≥5.5
with ≥12 highs; ≥1 wonder spike per arc; cozy/resonance floors honored).
FAIL example: a Cozy-process episode with Humor <4; a Set-piece below Wonder 7; an arc
with no Wonder ≥7; a flat axis run of 3+ episodes.
→ Distinguishes *correctly low* (inside floor, e.g. climax Humor 2) from *deficient*
(below floor). A low score inside its envelope is PASS, not a flaw.

## SENTINEL PROTOCOL
- **Canon Sentinel:** returns `CANON: PASS` or `CANON: FAIL — <contradiction + the
  CANON.md line broken>`.
- **Lane Sentinel:** returns `LANE: PASS` or `LANE: FAIL — <drift vector + guardrail +
  minimal correction>`, plus the `COMMERCIAL` / `LITERARY-CONTAMINATED` token.
- **Axis Sentinel (G7):** on any episode write/rewrite, score its 5 felt axes and
  check against `AXIS-ENVELOPE.md`. Returns `AXIS: PASS` or `AXIS: FAIL — <axis> below
  floor / foreground soft`, plus a book-level pass on the conservation laws after a batch.
- Any FAIL blocks the write. Drift cannot accumulate because it cannot land once.

## G1-EXT — COZY EMOTIONAL REGISTER (lane guard on emotional COLOR)
The emotional palette may carry **weight and range** but must stay in the cozy register.
A cozy story is not emotionless — it earns grief, longing, indignation — but it never
makes the reader fear *for the safe place* (Promise 3).
- **IN-LANE (allowed):** tender-grief, melancholy, longing, wistfulness, righteous
  **indignation**, fierce **protectiveness**, sober/steady resolve, bittersweet,
  contentment, pride, mischief, wonder, awe, hope, catharsis, wry-defeat, curiosity,
  guarded wariness (mild).
- **OUT-OF-LANE (banned as INTERIOR emotion / hook register):** dread, terror, despair,
  menace, horror, foreboding, doom, "cold" as a feeling. These belong to grimdark/thriller.
- **Exception:** the cull-economy / Monster Control may be rendered *cold / clinical* on
  purpose (antagonist contrast) — that coldness is OUTSIDE, never Briarwick's interior,
  and never the reader's relationship to the home.
- **Hook-outs are CURIOSITY, not dread.** A cozy chapter ends on a *question, a pull, an
  appetite, an intrigue* — never a sense of doom. The Lane Sentinel checks emotional color
  the same way it checks cozy-stakes: a beat coloured `dread/menace/cold-interior` = `LANE: FAIL`.
