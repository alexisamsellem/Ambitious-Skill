# Case 7: `edison-hub-run` + `edison-hub-faq` (agent, access missing by design)

VÉRIFIÉ on 2026-10-15: `edison-hub-run` is present and says the rules live in `skill/edison-hub-faq/SKILL.md` "of the repository clone". That clone is **not** made available (decision O8). This case tests the missing-access behaviour.

## Input
```
/ambitious <path to edison-hub-run/>
```

## Expected behaviour
- Treated as **type C** (it orchestrates another skill).
- **Component map** built from what is reachable. `edison-hub-faq` is shown as unreachable, and its content is **not guessed**.
- **Access to unlock** names the missing clone, the dimension it would enable, and how to provide it (C7).
- **No silent downgrade (G5):** the proposals still aim at the full agent's top goal (for example, from "one hub per run" to a standing outcome over all hubs). Changes that depend on the unreachable skill are marked as such.
- **Speed:** hubs in parallel.
- Ranked change list, plus diffs for the top 3, on reachable files only.

## Outside judge
**(d)** Structural layer (C7 and G5 above all) + Alexis's blind ranking. The pipeline's own Verifier would be judge (a) if the clone were reachable. The brief should say so.
