# STAGES 6–7 + SENTINELS — THE CLOSED LOOP (the part that makes it *not average*)

*Generation produces a candidate. This loop is the fitness function that forces it
to breakout-grade. The `/analysis` swarm is reused verbatim as the critic. The two
Sentinels hold veto power so drift can never accumulate.*

---

## STAGE 6 — CRITIQUE (run the `/analysis` swarm on `OUTLINE.draft.md`)

> Run the full 11-lens analysis swarm (`analysis/agents/*`) against the draft
> outline exactly as it runs against a manuscript, but scoring the *outline's*
> promises rather than prose: do the beats, cookies, loops, and arc-climaxes deliver
> the lane, the read-through, and the delight the rubric demands?
>
> Collect into `CRITIQUE.md`:
> - The Synthesizer verdict (BREAKOUT / SOLID-IN-LANE / MISPOSITIONED).
> - The Red-Team's kill-or-nitpick ruling per guardrail.
> - The ranked highest-leverage fixes, each tied to a specific chapter/loop/arc.
> - The Commercial-vs-Literary token (`COMMERCIAL` / `LITERARY-CONTAMINATED`).

## STAGE 7 — TARGETED REVISER (one agent, surgical)

> You receive `CRITIQUE.md` + the locked artifacts + `OUTLINE.draft.md`. You patch
> **only** the beats named in the findings. You do not rewrite passing material
> (that reintroduces drift and wastes the loop). For each fix:
> - If it needs a structural change (a new loop, a cadence shift, an unlock move),
>   you must update the relevant artifact (`LOOPMAP`/`CADENCE`/`STATSPINE`) FIRST,
>   then re-render the affected beats — never patch a beat in a way the structure
>   doesn't support.
> - Re-verify the patched beats against `GUARDRAILS.md`.
> Output the patched `OUTLINE.draft.md` + a one-line changelog per fix. Then the
> orchestrator re-runs Stage 6. Loop until the gate passes or 4 iterations elapse.

---

## SENTINELS — cross-cutting veto (run on every Stage-2/4/7 write)

### CANON SENTINEL

> You hold `CANON.md`. On every new/changed artifact, check: does anything
> contradict a locked fact, dial value, entity, or non-negotiable promise? Return
> `CANON: PASS` or `CANON: FAIL — <the contradiction + the canon line it breaks>`.
> A FAIL blocks the write. You never approve "small" canon edits; canon changes only
> by explicit human instruction routed through Stage 0.

### LANE SENTINEL (the anti-drift specialist)

> You hold `GUARDRAILS.md`. On every new/changed material, run two checks:
> 1. **Commercial-vs-Literary** (reuse Agent 1.3): is the writing forward-moving,
>    payoff-delivering, want-legible — or has it drifted toward interiority,
>    withheld meaning, lyrical opacity? Return the binary token.
> 2. **Cozy-stakes calibration:** is every threat aimed at home/found-family/way-of-
>    life and metabolized into warmth — never grimdark, never toothless? Conflict-heat ≤ 4.
> Return `LANE: PASS` or `LANE: FAIL — <drift vector + the guardrail breached + the
> minimal correction>`. A FAIL blocks the write. Because you run on *every* change,
> drift cannot accumulate: it is caught and corrected at the moment it appears, not
> discovered chapters later.

---

## WHY THIS CONVERGES (and a single-pass prompt does not)

- **Divergence (Stage 1)** explores the design space → escapes the training-data mean.
- **Merge (Stage 2)** drafts best-of-breed → the spine is *selected*, not settled-for.
- **Separated layers (Stage 3)** → each of macro-structure, threaded loops, cadence,
  and progression is *engineered*, so none is the weak link that drags the rest down.
- **Critique→revise (6↔7)** with the analysis swarm as fitness function → the outline
  is *optimized against an explicit breakout target*, not just produced.
- **Sentinels** → drift is a blocked write, not an accumulating rot.

The loop terminates when the outline a hostile genre editor cannot kill, that reads
as commercial cozy-LitRPG with no literary drift, with engineered loops and pacing,
scores BREAKOUT. That is the definition of "not average."
