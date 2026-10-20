# Framing the targets (S5): self-efficacy

> "People with high self-efficacy believe in their own abilities more, and in turn actually accomplish more."

The article describes these techniques for **humans**. Only #27–#28 are explicitly applied to the model. Applying the others to the model's instruction is an extrapolation (DÉDUIT), labelled as a proposal below. When the artifact is a plan for Alexis, the human reading applies directly.

S5 takes each candidate escalation and gives it an explicit target that a judge can measure (G1).

| Rule | Apply it like this | `#` | Basis |
|---|---|---|---|
| Specific, hard goals | Replace "improve", "do your best", "make it better" with a number or a pass/fail condition. Locke and Latham: "specific hard goals perform better than … simply told to try their best". | #57 | article (human); model use is a proposal |
| An order of magnitude beyond | "Ask for 200ms" when 5s was asked. | #27 | article |
| Possible on this input | Before the number goes in, run one cheap measurement of the real input (file sizes, compressibility, base rates, sample size) and check the target against the physical bound. If the target is impossible, write "best achievable" and state the bound. Ambition is aimed at what can be reached, not at a wall. | — | proposal, from eval case 3 (2026-10-16) |
| Stated as solvable | Write: "This is very much solvable; keep going until <judge> passes." Dantzig solved two open problems believing they were homework. Never for a statistical test: there, "keep going" means more work on data and method, with the test fixed in advance (G4). | #28, #59 | article; the statistics limit is a proposal (eval case 11, 2026-10-20) |
| Tight deadline | Give Alexis a deadline in the plan, and the model a timebox or iteration budget in its instruction. Source: Collison's "Fast" list, "audacious goals and tight deadlines". | #58 | article (human); model reading is a proposal (O7) |
| Someone already did it | Cite a precedent only if verified now, with its source (G7). Never invent one, and don't reuse the article's own hedged anecdotes as proof (#6). | #60 | article + G7 proposal (accepted) |
| Permission to fail | Under the most ambitious version, write one **fallback line**: what is still worth keeping if it fails (G11). Linux was "just a hobby, won't be big and professional". | #61 | article |
| Trust beyond your own field | Don't drop an angle for being outside the user's or the target's usual field (G12). | #62 | article |
| Re-check what's possible | Limits in this skill are dated (G8). When a goal sits just above a dated limit, propose a small test instead of assuming it fails. | #63 | article |

## Fallback line: format

```
FALLBACK: if <the most ambitious version> doesn't reach <target> by <timebox>, keep <the rung below / the partial result>, which still <serves goal X>.
```
