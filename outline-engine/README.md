# THE OUTLINE FORGE — a parallel agent swarm for breakout cozy-LitRPG outlines

This is the **generation** counterpart to `/analysis` (the critique swarm). Together
they form one closed loop: the Forge produces an outline, the analysis swarm scores
it against the breakout rubric, a reviser patches only the weak beats, and the loop
repeats until the outline clears the **BREAKOUT-COMMERCIAL** gate with no Red-Team
kill and no genre drift.

## Why this beats a single-pass prompt

A single model call — even a great one — regresses to the mean of its training
data. That is *literally* what "average" and "genre drift" are. Three mechanisms
fight that here:

1. **Divergence before convergence.** Don't ask one agent for one outline. Run N
   architects in parallel from *different structural theses*, then merge best-of-breed.
   You select the strongest spine instead of accepting the first idea.
2. **Separated structural layers.** Macro-structure, threaded loops, cadence, and
   stat-progression are engineered by *different* specialists against a *locked*
   architecture — so each layer is optimized, not hand-waved inside prose beats.
3. **A closed critique→revise loop.** The `/analysis` swarm is the fitness function.
   Nothing ships until it scores breakout. This is the part that makes it *not average*.

## Anti-drift is structural, not hopeful

Two dedicated agents hold veto power on every iteration:
- **Canon Sentinel** — enforces `CANON.md` (immutable facts + dials + promises).
- **Lane Sentinel** — runs the Commercial-vs-Literary discriminator + cozy-stakes
  check. If a revision drifts toward literary fiction or grimdark, it is rejected
  *before* it enters the outline. Drift cannot accumulate because it cannot land once.

## The pipeline

```
STAGE 0  Canon Lock & Constraint Compiler        → CANON.md, GUARDRAILS.md   (1 agent)
STAGE 1  Architecture Swarm (DIVERGENT)          → 5 candidate architectures (5 parallel)
STAGE 2  Spine Selection & Merge                 → ARCHITECTURE.md           (1 agent)
STAGE 3  Structural-Layer Engineering            → LOOPMAP / CADENCE / STATSPINE (5 parallel)
STAGE 4  Beat Generation (BY ARC)                → arc-1..4 beats            (4 parallel)
STAGE 5  Continuity & Seam Welder                → OUTLINE.draft.md          (1 agent)
STAGE 6  Critique  = run /analysis swarm         → verdict + fixes + kills   (11 lenses)
STAGE 7  Targeted Reviser                         → OUTLINE.draft.md (patched)(1 agent)
         ── loop 6↔7 until BREAKOUT & no KILL ──
SENTINELS  Canon + Lane veto on every write       (cross-cutting, 2 agents)
```

File map:
- `00-orchestrator.md` — the conductor prompt; owns the loop and the shared artifacts
- `01-canon-lock.md` — Stage 0
- `02-architecture-swarm.md` — Stages 1–2 (divergence + merge)
- `03-loop-and-cadence.md` — Stage 3 (the structural crown jewels)
- `04-beat-generation.md` — Stages 4–5
- `05-critique-revise-loop.md` — Stages 6–7 + the two Sentinels

## The structural theory it encodes (named, not vibes)

- **Macro:** nested **Promise / Progress / Payoff** (Sanderson) — series-door →
  book-door → 4 arc-doors → chapter-door; every level pays its own promise *and*
  opens a bigger one. Never a cruel cliffhanger.
- **Threaded loops:** **MICE + LIFO nesting** (Card) — open loops in order A→B→C,
  close them in reverse C→B→A, so the outline breathes like matryoshka dolls and
  nothing dangles.
- **Micro (tension chapters):** **Scene & Sequel** (Swain/Bickham) — goal→conflict→
  disaster, then reaction→dilemma→decision.
- **Micro (cozy/warm chapters):** **Kishōtenketsu** — a 4-part structure that
  satisfies *without* manufactured conflict (ki/development/twist/reconciliation).
  This is the secret weapon: it lets warm-out chapters land emotionally without
  betraying cozy by inventing a fight. Alternating Scene&Sequel with Kishōtenketsu
  is how you keep momentum *and* keep it cozy.
- **Cadence:** one cookie per chapter, a larger upgrade every ~3, a live clock or
  deepening mystery in every arc, tension-out / warm-out alternation.
