# SCENE-BEATS SPEC (Stage 9) — how every episode's scene outline is built

*Each episode (`scenes/ep-NN.md`) renders its locked episode-beat into the actual
scene sequence a drafter will write. Scenes are a RENDERING of locked structure
(CADENCE micro-structure + LOOPMAP loops + STATSPINE deltas + the 🌦️/🍲 atmosphere
tags) — not new invention. Continuity is guaranteed because every scene writer works
from the same locked artifacts; this is why per-episode generation parallelizes safely.*

## Per-episode file format

```
# Ep N — "Title"   ·   micro-structure: K& (Kishōtenketsu) | S&S (Scene&Sequel)
**Episode promise (1 line):** what this episode delivers.
**Tags (from outline):** 🍪<cookie> · 🪝<out> · 🧵 opens[…]/closes[…] · 🌦️<atmosphere> · 🍲<recipe if any>
**Word target:** ~2,000–2,800 · **Scenes:** 3–6.
**Entry state → Exit state:** <key stat deltas from STATSPINE>.

## Scene 1 — <short label>   [stage tag]
- **Function / POV state:** what this scene is FOR; Liora's want entering it.
- **Beats:** 2–4 bullets — concrete action/dialogue, with the turn (yes-but / no-and
  for S&S; the gentle recontextualizing *ten* for K&).
- **System box (if any):** the deadpan Ledger/System cue that fires here.
- **Sensory / atmosphere:** the 🌦️ texture grounded in THIS scene (season-appropriate,
  dry register).
- **Lands here:** which of {cookie · loop open/close · stat tick · 🍲 recipe ·
  bestiary +1 · room unlock} fires in this scene (only what the outline assigns).
- **Exit:** the transition / hook into the next scene.

## Scene 2 … (repeat)

## Out — <hook-out | warm-out>
- The closing beat + the final line's intent (page-turn pull or settle-in warmth).
- Confirm the episode's 🪝 out-type is delivered here.
```

## Scene-count guidance by micro-structure

- **S&S (tension episodes):** 4–6 scenes. Map to goal → escalating obstacle →
  yes-but/no-and turn → disaster/cost → short **sequel** (reaction, dilemma, new
  decision that fires the next episode). Cookie lands at the turn; hook-out.
- **K& (cozy episodes):** 3–5 scenes. Map to **ki** (cozy status-quo + a small want)
  → **shō** (gentle development / process — the literary-ASMR zone) → **ten** (an
  unexpected, non-threatening recontextualizing turn) → **ketsu** (warm reconciliation
  + quiet progress). Cookie lands in the *ten*; warm-out.
- The 5 ✨ SET-PIECE episodes (7/16/28/31/49) get one dedicated WONDER scene — the
  atmosphere is foregrounded as its own beat (rain-hearth / brook / firefly-Lull /
  sporeglow-aurora / storm-break-sunrise).

## Hard rules (every scene writer obeys)

1. **Render, don't reinvent.** Hit exactly the outline's cookie, out, loops, stats,
   atmosphere, and any 🍲/room/bestiary the episode assigns. Use only abilities on
   STATSPINE; if a beat needs one not yet unlocked, STOP and flag.
2. **Voice fingerprint** (CANON): dry deflection; bureaucracy-as-metaphor; System in
   deadpan editorial register; staccato one-beat lines for comedy; tenderness stays
   IN the dry register — NO lyrical-literary lines (the voice guard).
3. **Cozy-stakes** (G1): threat to home/family/way-of-life only; heat ≤4; resolve-then-
   open (G6). Anti-plateau (G5): a live clock/mystery present even in cozy scenes.
4. **Continuity at the seams:** open on a beat that flows from the previous episode's
   out; end delivering this episode's assigned out-type so the next flows from it.
5. Canon episodes (Ep1–2) render the existing manuscript faithfully; do not contradict
   `manuscript/chapter-0{1,2}.md`.
