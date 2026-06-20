# THE MONSTER NURSERY — BREAKOUT ANALYSIS SWARM

A forensic, multi-agent system for answering one question:

> **Is this cozy-LitRPG breakout-grade commercial genre fiction — true to its
> lane, engineered for read-through, delightful — and NOT literary fiction
> wearing a genre coat?**

## Why a swarm (not one reviewer)

A single reviewer suffers the halo effect: one great chapter-opener inflates every
score. This swarm enforces **forensic specialization + adversarial cross-check +
a single synthesizer**. Each agent reads the *same* manuscript through *one* lens,
scores against a fixed rubric with line-cited evidence, and must survive a skeptic.

## Structure

```
analysis/
├── rubric.md                      # shared scoring contract — read first
├── agents/
│   ├── wave1-positioning.md       # 4 agents: is it the right book?
│   ├── wave2-craft.md             # 7 agents: is it delightful?
│   └── wave3-adversarial.md       # red-team + adjudicator + synthesizer
└── reports/
    └── pilot-ch1-2.md             # synthesized verdict on the Ch1–2 pilot
manuscript/
├── chapter-01.md                  # extracted from "Chapter 1.pdf"
└── chapter-02.md                  # extracted from "Chapter 2.docx"
```

## How to run

1. **Inputs, identical to every agent:** `manuscript/*.md` + `analysis/rubric.md` +
   that agent's section from `analysis/agents/`. Isolated context per agent so
   scores don't cross-contaminate.
2. **Wave 1 + Wave 2 in parallel** (11 agents). Each does a *blind* read (gut 1–10)
   then a *forensic* read (line-cited scores) and returns the rubric output block.
3. **Wave 3 after** the reports exist: Red-Team attacks the guardrails, the
   Evidence Adjudicator rejects unsupported scores and surfaces conflicts, the
   Synthesizer applies the aggregation rule and writes the verdict.

## Verdict gate (see rubric.md for the full rule)

**BREAKOUT-COMMERCIAL** requires: Wave-1 positioning gates pass · ≥5/7 craft agents
score their headline dimension ≥8 with none <5 · Red-Team lands no structural kill.
Otherwise **SOLID-IN-LANE** or **MISPOSITIONED**.

## Scaling to the full book

This pilot runs on Chapters 1–2 to calibrate the rubric. For the full draft, run
the same swarm **per arc** (the outline's 4 arcs), then a meta-synthesizer over the
four arc-verdicts to judge whole-book read-through, plateau-middles, and Promise
Ledger payoffs that two chapters cannot reveal.
