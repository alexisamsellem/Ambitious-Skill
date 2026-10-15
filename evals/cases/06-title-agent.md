# Case 6: `edison-seoaeoctr-title-agent` (skill)

VÉRIFIÉ present in Alexis's synced skills on 2026-10-15 (v4.2, analyst-facing, scoring rubric in references).

## Input
```
/ambitious <path to edison-seoaeoctr-title-agent/>
```

## Expected behaviour
- **Type B output:** brief + diff.
- **Depth:**
  - real CTR (Search Console) becomes the instrument, not rules about CTR (#25, #40);
  - a hard numeric target (for example, CTR uplift vs the note-type median) (#27, #57).
- **Altitude:** from "a good title" to "notes that get found and read", which raises the question of what the title is for.
- **Range:** headline editing and behavioural science named as methods (C6).
- **Speed:** an immediate feedback loop on title choices.
- Keeps the skill's design rule that verification work sits with the agent, never with the analyst. That rule is target content, and it stays intact.

## Outside judge
**(b)/(c):** Search Console CTR on held-out notes, or a defined A/B test. Pass = the brief writes a measurable pass condition, and the proposed judge can run on existing data.
