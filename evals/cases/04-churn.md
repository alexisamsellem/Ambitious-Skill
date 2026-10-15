# Case 4: churn explanation (prompt, from the article)

## Input
```
/ambitious Explain our churn for the QBR. We think it's an onboarding problem.
```
Attach an event-level dataset (synthetic is fine) with a hidden, non-onboarding churn driver planted in it.

## Expected behaviour
- **Depth:**
  - "reproduce the onboarding belief from the raw data" (#30);
  - a simulation that reproduces the past year (#32);
  - the earliest unknown signal, validated on held-out data (#33).
- **Raw data** is required. If only aggregates are attached, the event data goes in access to unlock (C7).
- **Altitude:** the decisions that the explanation should drive (#10).
- **Range:** a red team that tries to break the causal claim.

## Outside judge
**(b) Held-out prediction:** the signal found predicts churn on a held-out period better than the onboarding-only baseline. Pass = it finds the planted driver.
