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

## Never a judge

- Your own review of your own output, in the same context (G4).
- "It looks right", "this should work", or any statement that names no external check.

## Writing the judge into the brief

```
Judge (b): backtest on Jan–Sep 2026; pass = flags the June drop ≥ 2 weeks before the monthly report did.
```

A judge needs a pass condition. If you can't write one, the escalation fails G1: rewrite it or drop it.

## Dated limit (G8)

The rule that the model can't judge itself is stated as of **October 2026**. Keep the hierarchy above until a stronger judge is shown to work. Don't relax it on assumption.
