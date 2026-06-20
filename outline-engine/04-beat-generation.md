# STAGES 4–5 — BEAT GENERATION (by arc) + SEAM WELDING

*Now every structural layer is locked. Beats can be generated in parallel BY ARC
without drift or seams, because the loop map, cadence schedule, and stat-spine are
pre-resolved across arc boundaries. Parallelism here is safe precisely because the
hard coordination happened in Stage 3.*

---

## STAGE 4 — FOUR ARC-BEAT GENERATORS (run in parallel, one per arc)

### Prompt (parameterized by arc number)

> You write the chapter beats for **Arc N only**. You receive the full locked
> package: `CANON.md`, `GUARDRAILS.md`, `ARCHITECTURE.md`, `LOOPMAP.md`,
> `CADENCE.md`, `STATSPINE.md`, plus the two micro-structure templates.
>
> You do not invent structure — you *render* it. For each chapter in your arc:
>
> 1. Look up its row in `CADENCE.md` (cookie type, out, clock, micro-structure).
> 2. Look up which loops `LOOPMAP.md` says open or close in this chapter.
> 3. Look up the stat deltas `STATSPINE.md` assigns here.
> 4. Write the beat to the assigned micro-structure template (SCENE&SEQUEL or
>    KISHŌTENKETSU), hitting exactly those loops, that cookie, that out, those stats.
>
> Output format per chapter (matches the blueprint's Part 3 spec):
>
> **Ep N — "Title"** *(episode-type · micro-structure)* — problem → action.
> 🍪 cookie: <the in-chapter reward>.
> 🪝 out: <hook or warm, one line>.
> 🧵 loops: opens [IDs] / closes [IDs].
> *State:* <stat deltas from STATSPINE>.
>
> Constraints:
> - Honor the voice fingerprint: dry deflection, bureaucracy-as-metaphor, the System
>   in deadpan editorial register. If a beat tempts a lyrical line, redirect to
>   deadpan tenderness (the voice guard).
> - Keep cozy-stakes calibration: real threat to home/family/way-of-life, never
>   grimdark, never toothless. Conflict-heat ≤ 4.
> - You may render 1–2 sample chapter-openers in the book's voice to prove tone
>   carries (optional blueprint toggle).
> - You may NOT use any ability not on `STATSPINE.md`. If you need one, STOP and
>   flag it for the orchestrator rather than inventing.

## STAGE 5 — SEAM WELDER (one agent, after all four arcs)

> You stitch the four arc-beat files into `OUTLINE.draft.md` and run the
> cross-arc integrity checks no single arc-generator could see:
>
> - **Stat continuity:** each arc's entry-state equals the previous arc's exit-state.
>   Flag any discontinuity.
> - **Loop integrity:** every loop opened in `LOOPMAP` is closed by its scheduled
>   chapter; LIFO order holds across arc boundaries; nothing dangles except the
>   deliberate series door.
> - **Promise-ledger reconciliation:** every seed in `ARCHITECTURE.md` pays off on
>   schedule; payoff cadence has no long dry stretch.
> - **Cookie/out continuity at seams:** no two adjacent chapters across an arc
>   boundary repeat cookie type or both end on hard hooks.
> - **Voice/tone continuity:** spot-check arc-boundary chapters for register drift.
>
> Output `OUTLINE.draft.md` (Pre-Outline Architecture + the full arc-structured beat
> list with 🍪/🪝/🧵 tags and running stat-state) plus a short **Seam Report** listing
> any flags for the reviser. Do not silently fix structural conflicts — surface them.
