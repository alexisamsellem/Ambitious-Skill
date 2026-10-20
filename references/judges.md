# Outside judges

> "Do not ask the model to judge itself. I assume that this will eventually be solved with increasing model intelligence, but in October 2026, I implore you to insist on outside validation. Ideally that's a tool the model can run to get feedback immediately." (#34, #35, #36)

> "(4) say what, other than you or me, would show the result is right" (#42)

Every escalation names one judge (G1). Prefer the highest level that can be reached; if it isn't reachable, name it anyway and put the access in "access to unlock".

## Hierarchy

| Level | Judge | Examples | `#` |
|---|---|---|---|
| **a** | A tool the model can run, with immediate feedback | test suite, reproduction script, profiler / Lighthouse run, `recalc.py` with zero errors, an existing verifier step (`pre-send-verifier`), a linter, a schema validator | #35 |
| **b** | Held-out data or a backtest on the user's own history | "show it predicts on data it has not seen"; "show from our own history that it would have caught things sooner" | #13, #33 |
| **c** | A real-world signal or shadow run | run beside the current process for a cycle; live CTR / conversion; an A/B test | #14 |
| **d** | A named human expert | Alexis's blind ranking; a named analyst or editor | — |
| **e** | A separate model instance that never sees the producing reasoning | a fresh subagent given only the output and the criteria. **Always labelled "weak judge".** | — |

## The judge measures the goal, not a proxy

Pick the judge that measures the goal the escalation serves, then take the highest level available *for that goal*. A proxy that is easy to check (word count, factual accuracy, schema validity, script passes) is a **constraint**: it guards against errors, but it is never the target.

- Creative work: the goal is what a reader values, so the top judge is a reader (d), usually a blind ranking. Tool checks (length, facts, clichés) are listed as constraints only. *Why: case 10 (2026-10-15), where a story that passed 6 tool checks lost to the raw version.*
- Analysis: the goal is a true, decision-relevant cause, so held-out prediction or a planted-truth test (b) measures it; "the notebook runs" is a constraint.
- If no judge can measure the goal itself, say so in the brief, and don't present a proxy as proof.

## A backtest must not see what it tests

The tuning window (where thresholds, weights or features are chosen) ends **before the earliest sign** of the event the backtest must catch, leading signals included, not just before the event itself. Write both dates in the judge, and check them against the data before the brief goes out. *Why: case 1 (2026-10-16), where thresholds "fixed before April 2025" were tuned on the January to March ticket spike they were meant to detect.*

## Never a judge

- Your own review of your own output, in the same context (G4).
- A test you wrote and ran on synthetic data you built. It catches bugs, but it cannot show that the move works on the real target. The move stays gated until a judge on real data, or an outside one, runs. *Why: eval case 11, v1 and v2 (2026-10-19/20), where self-built tests passed and the outside judge broke the scripts.*
- A statistical test re-run with new specifications until it passes. Fix the test, the threshold and the sample first.
- "It looks right", "this should work", or any statement that names no external check.

## Writing the judge into the brief

```
Judge (b): backtest on Jan–Sep 2026; pass = flags the June drop ≥ 2 weeks before the monthly report did.
```

A judge needs a pass condition. If you can't write one, the escalation fails G1: rewrite it or drop it.

## Dated limit (G8)

The rule that the model can't judge itself is stated as of **October 2026**. Keep the hierarchy above until a stronger judge is shown to work. Don't relax it on assumption.
