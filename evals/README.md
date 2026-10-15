# Evaluating `/ambitious`

**Question this answers:** does `/ambitious` make the *executed work* better than the raw request, and better than `/agent-prompt-reviewer`?

## Protocol

1. **Variants.** Run each case in `cases/` three ways:
   - **(a)** the raw request;
   - **(b)** after `/ambitious`;
   - **(c)** after `/agent-prompt-reviewer` for skill and agent cases (5–8). For prompt cases (1–4, 9, 10), (c) is the article's own Depth prompt applied by hand, as an independent baseline.
2. **Execute** each variant and keep the outputs. Compare outputs, not prompts.
3. **Layer 1, structural.** Check the `/ambitious` output against `structural-checks.md`. Every check must pass.
4. **Layer 2, blind ranking.** Someone other than Alexis (or a script) shuffles the three outputs and labels them A/B/C. Alexis ranks them against the case's question. Where the case names a tool judge (level a–c), its result settles a disagreement.
5. **Record** results in `results/<date>.md` (one row per case: structural pass/fail, blind rank, judge result, notes).

## Pass thresholds for v1

| Measure | Threshold |
|---|---|
| Blind wins for `/ambitious` | ≥ 7 of 10 cases |
| Structural checks | 10 of 10 cases |
| Against `/agent-prompt-reviewer` (cases 5–8) | Informs the replacement decision; Alexis decides |

## Cases

| # | File | Type | Main thing under test |
|---|---|---|---|
| 1 | `01-qbr-deck.md` | Prompt (article) | Full altitude ladder, backtest judge |
| 2 | `02-crash-free.md` | Prompt (article) | Standing outcome, access to unlock |
| 3 | `03-load-time.md` | Prompt (article) | Unreasonable target, real instruments |
| 4 | `04-churn.md` | Prompt (article) | Raw data, held-out prediction |
| 5 | `05-monthly-audience-report.md` | Skill | Type B diff, mechanism over report |
| 6 | `06-title-agent.md` | Skill | Depth on a real metric |
| 7 | `07-hub-run-agent.md` | Agent | Type C output, no silent downgrade |
| 8 | `08-client-reach-report.md` | Skill | Existing judge reused, export automation |
| 9 | `09-trivial-email.md` | Edge: trivial | Proportion (G2), justified drops |
| 10 | `10-creative-story.md` | Edge: creative | Altitude dropped (#17), no role-play |

Running the evals is manual for v1. Automation is parked (open question O3).
