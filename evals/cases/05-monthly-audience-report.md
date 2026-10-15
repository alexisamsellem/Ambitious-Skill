# Case 5: `monthly-audience-report-v2` (skill)

VÉRIFIÉ present in Alexis's synced skills on 2026-10-15 (v13.1.0, explicit-invocation only, with many reference files).

## Input
```
/ambitious <path to monthly-audience-report-v2/>
```

## Expected behaviour
- **Type B output:** brief + unified diff against `SKILL.md` and the reference files it changes. **No file written** (C10).
- Reads **every** reference file before proposing (S1).
- **Altitude:**
  - names why the report exists (leadership acts on audience shifts early; mirrors #11);
  - proposes a detection mechanism that flags shifts as they happen rather than once a month (#12), backtested on past months (#13).
- **Depth:** checks whether each method in the skill is a real analyst instrument or only vocabulary (#25), and keeps what already is.
- **Range:** a red team on the causal theses (#51); methods from forecasting or epidemiology for early signals.
- **Speed:** parallel source pulls; backtest before any shadow month.
- Doesn't duplicate gates that already exist (G2).

## Outside judge
- **(b) Backtest:** the proposed mechanism, run on past months, flags a known past event earlier than the monthly report did.
- **Plus:** Alexis's blind ranking against `/agent-prompt-reviewer`'s output on the same skill.
