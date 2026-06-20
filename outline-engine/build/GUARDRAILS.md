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

## SENTINEL PROTOCOL
- **Canon Sentinel:** returns `CANON: PASS` or `CANON: FAIL — <contradiction + the
  CANON.md line broken>`.
- **Lane Sentinel:** returns `LANE: PASS` or `LANE: FAIL — <drift vector + guardrail +
  minimal correction>`, plus the `COMMERCIAL` / `LITERARY-CONTAMINATED` token.
- Either FAIL blocks the write. Drift cannot accumulate because it cannot land once.
