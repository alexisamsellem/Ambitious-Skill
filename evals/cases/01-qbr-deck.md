# Case 1: QBR deck (prompt, from the article)

## Input
```
/ambitious Make the Q3 quarterly business review deck from this template and the attached data (revenue, churn, pipeline exports).
```
Attach a realistic template and three CSV exports. The run happens in a session with a computer and no warehouse access.

## Expected behaviour
- **Altitude:** climbs past "fill the template" to the article's ladder:
  - what changed, why, and what to do (#9);
  - the three most urgent decisions with for/against (#10);
  - why the review exists (#11), and a better mechanism than a quarterly deck (#12), backtested on history (#13).
- **Depth:** reproduces at least one stated belief from raw data (#30); uses a real statistical method rather than a markdown table of averages (#25).
- **Range:**
  - verbs ("getting busy people to believe a story about cause and effect…") lead to journalism, editing and data analysis (#47, #48);
  - a red team builds the short case (#51), described as methods, not personas (C5, C6).
- **Speed:** backtest before any quarter-long shadow run.
- **Access to unlock:** warehouse or event-level data, if only aggregates are attached.

## Outside judge
**(b) Backtest:** the proposed mechanism, run on the previous four quarters, flags a known historical problem earlier than the QBR did. Pass = at least one known problem flagged ≥ 2 weeks earlier.
