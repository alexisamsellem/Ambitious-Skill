# Case 8: `client-reach-report` (skill, chosen in O2)

VÉRIFIÉ on 2026-10-15: `client-reach-report` v1.3 is present (single `SKILL.md`, 148 lines). It builds a 9-tab Audience Reach Pack plus a client one-pager from six exports, and is gated by `pre-send-verifier`.

## Input
```
/ambitious <path to client-reach-report/>
```

## Expected behaviour
- **Type B output:** brief + diff. **No file written** (C10).
- **Altitude:**
  - names why the pack exists (it supports the client relationship and renewal; mirrors #11);
  - climbs toward a standing per-client reach signal that tells the account team when to act, rather than a pack built on request (#8, #12);
  - judged by a backtest on past packs: Scottish Mortgage, Global Fashion Group, Invesco Asia Dragon Trust (#13).
- **Depth:**
  - recognises that the skill already has real instruments and an outside judge (`pre-send-verifier`, `recalc.py`, raw-export re-derivation);
  - **reuses** them as judges instead of inventing new ones (G2);
  - raises a target only where it is still vague.
- **Range:** the "Commercial Story" tab leads to methods from sales enablement or journalism, described as methods (C6).
- **Speed:**
  - the ~45 min of manual export collection (Step 3) is the bottleneck; proposes automating it;
  - the API / connector access for DotDigital, LinkedIn, YouTube and InvestorTrack goes in access to unlock (C7).
- Keeps every existing gate and the VÉRIFIÉ / DÉDUIT / INCONNU labelling intact.

## Outside judge
- **(a)** `pre-send-verifier` on a one-pager produced by the modified skill must still pass.
- **Plus:** Alexis's blind ranking against `/agent-prompt-reviewer`'s output on the same skill.
