# Traceability matrix

Canonical matrix: every inventory item (`inventory.md`) mapped to where it is implemented, or to its exclusion reason.
`docs/spec.md` §9 is the 2026-10-15 snapshot; this file is the one kept in sync with the skill.
Section references (§, S, G) point to `docs/spec.md`; file names point to `SKILL.md` and `references/`.

**How to read the columns:**
- **Status:**
  - **Impl**: implemented as the article states it.
  - **Impl+P**: implemented with a proposal-labelled extension.
  - **Excl**: excluded. For these rows, the "Spec / file" column gives the reason instead of a location.
- **Spec / file:** the section of this spec, then the planned repo file.

| # | Item (short) | Tag(s) | Status | Spec / file |
|---|---|---|---|---|
| 1 | Four-type taxonomy | Altitude+Depth+Range+Speed | Impl | §1, §5 S4, §7 · `SKILL.md` |
| 2 | Speed: the same work in less time | Speed | Impl | §7.4 · `references/speed.md` |
| 2b | Speed "requires little creativity" | Speed+Caveat | Impl+P | §5 S4 (Speed last), §7.4 · `references/speed.md` |
| 3 | Capabilities are uneven | Caveat | Impl+P | §6 G8 (re-test, don't assume) · `SKILL.md` |
| 4 | Not model-specific | Caveat | Excl | Little weight for a Claude skill; the methods in §7 depend on no model quirk anyway. |
| 5 | Low-ambition default / rallying cry | none | Excl | Not actionable: diagnosis and motivation. |
| 6 | Opening anecdotes (planet, music, math) | none | Excl | Not actionable. The article hedges them itself ("may have helped"), so they can't serve as precedents under G7. |
| 7 | Goal beyond the goal | Altitude | Impl | §5 S2, §7.1 · `references/altitude.md` |
| 8 | One-off task → standing outcome | Altitude+Speed | Impl | §7.1, §7.4 · `altitude.md`, `speed.md` |
| 9 | All the data; what / why / what to do | Altitude+Prerequisite | Impl | §7.1 · `references/altitude.md` |
| 10 | 3 most urgent decisions, for/against | Altitude | Impl | §7.1 · `references/altitude.md` |
| 11 | Why the artifact exists | Altitude | Impl | §5 S2, §7.1 · `references/altitude.md` |
| 12 | Design a better mechanism | Altitude | Impl | §7.1 · `references/altitude.md` |
| 13 | Prove it on your own history | Altitude (judge) | Impl | §7.1, §7.4, judge (b) · `altitude.md`, `judges.md` |
| 14 | Run it beside the current process | Altitude | Impl+P | §7.1, §7.4 (backtest first), judge (c) · `altitude.md`, `speed.md` |
| 15 | Escalate step by step | Altitude | Impl+P | §5 S2: the ladder is internal; output = top rung, fallback = the rung below (R2.4) · `altitude.md` |
| 16 | Applies when there is an end outcome | Caveat | Impl | §7.1 "Applies when" · `altitude.md` |
| 17 | Less suited to creative work | Caveat | Impl | §7.1 "Weak or dropped", eval 10 · `altitude.md` |
| 18 | Meetings are the tell-tale sign | Caveat | Impl | §7.1 "Applies when" · `altitude.md` |
| 19 | "Go make money" ceiling (2026) | Caveat | Impl | §5 S2, §6 G8 · `altitude.md` |
| 20 | Ceiling rises with capability | Caveat | Impl | §6 G8 · `altitude.md` |
| 21 | Durable workflows, human out of the loop | Altitude+Speed | Impl | §7.1, §7.4 · `altitude.md`, `speed.md` |
| 22 | Changing the workflow comes first | Prerequisite | Impl | §5 S3, §7.1 · `references/access.md` |
| 23 | Reproduce and verify independently | Prerequisite | Impl | §5 S3, §7.1 · `references/access.md` |
| 24 | Expert grade, until experts learn something | Depth | Impl | §7.2 · `references/depth.md` |
| 25 | Instruments, not vocabulary | Depth | Impl | §7.2 · `references/depth.md` |
| 26 | User needn't know the tools | Depth | Impl | §7.2 · `references/depth.md` |
| 27 | Unreasonable target (×10) | Depth+Self-efficacy | Impl | §5 S5, §7.2 · `depth.md`, `self-efficacy.md` |
| 28 | Treat it as reasonable, keep going | Depth+Self-efficacy | Impl | §5 S5, §7.2 · `depth.md`, `self-efficacy.md` |
| 29 | Raw information | Depth+Prerequisite | Impl | §5 S3, §7.2 · `depth.md`, `access.md` |
| 30 | Check beliefs against the raw data | Depth | Impl | §7.2 · `references/depth.md` |
| 31 | Find blind spots | Depth | Impl | §7.2 · `references/depth.md` |
| 32 | A model that reproduces the past | Depth | Impl | §7.2 · `references/depth.md` |
| 33 | Predict on unseen data | Depth (judge) | Impl | §7.2, judge (b) · `depth.md`, `judges.md` |
| 34 | The model doesn't judge itself | Depth+Caveat | Impl | §6 G1, G4 · `SKILL.md`, `judges.md` |
| 35 | Judge = a tool with immediate feedback | Depth+Speed | Impl | §6 G4, judge (a), §7.4 · `judges.md`, `speed.md` |
| 36 | Self-judgment limit dated Oct 2026 | Caveat | Impl | §6 G8 · `judges.md` |
| 37 | A mix of techniques, not a checklist | Caveat | Impl | §6 G10 · `SKILL.md` |
| 38 | Deeper, not bigger | Depth+Caveat | Impl | §6 G2, §7.2 · `SKILL.md`, `depth.md` |
| 39 | Protocol Q1: what a top pro would do | Depth | Impl | §7.2 · `references/depth.md` |
| 40 | Protocol Q2: the rawest material | Depth | Impl | §5 S3, §7.2 · `references/depth.md` |
| 41 | Protocol Q3: methods and tools | Depth | Impl | §7.2 · `references/depth.md` |
| 42 | Protocol Q4: outside proof | Depth | Impl | §6 G1, §7.2 · `depth.md`, `judges.md` |
| 43 | Protocol: rewrite the prompt | Depth | Impl+P | §4 (artifact per type, extended to skills and agents) · `depth.md`, `input-types.md` |
| 44 | More fields than was economical | Range | Impl | §7.3 · `references/range.md` |
| 45 | Multi-agent setups to bring in fields | Range+Speed+Prerequisite | Impl | §7.3, §7.4 · `range.md`, `speed.md` |
| 46 | Tools from distant fields (Blender) | Range | Impl | §7.3 · `references/range.md` |
| 47 | Nouns → verbs | Range | Impl | §5 S2, §7.3 · `references/range.md` |
| 48 | Verbs → fields | Range | Impl | §7.3 · `references/range.md` |
| 49 | Raise the stakes, assemble the crew | Range | Impl | §7.3 · `references/range.md` |
| 50 | Production crew chosen to fit delivery | Range | Impl | §7.3 · `references/range.md` |
| 51 | Red team (short seller, forensic accountant) | Range+Depth | Impl | §7.3 · `references/range.md` |
| 52 | No role-play; do what the expert does | Caveat | Impl | §6 G3, §7.3 · `SKILL.md`, `range.md` |
| 53 | The crew finds methods | Range | Impl | §6 G3, §7.3 · `references/range.md` |
| 54 | "Where the magic happens" | Range | Excl | The author's preference; it gives no criterion that could become a rule. |
| 55 | Computer, software, data access | Prerequisite | Impl | §5 S3, §6 G5 · `references/access.md` |
| 56 | Use a tool that provides this | Prerequisite | Impl+P | §4 "Access to unlock". The article names no tool, so the skill names one by context · `access.md` |
| 57 | Specific, hard goals | Self-efficacy | Impl+P | §5 S5, applied to the model's instruction (extrapolated from humans) · `self-efficacy.md` |
| 58 | Audacious goals + tight deadlines | Self-efficacy+Speed | Impl+P | §5 S5, §7.4. What a deadline means to a model → §11 O7 · `self-efficacy.md`, `speed.md` |
| 59 | Believe it possible (Dantzig) | Self-efficacy | Impl | §5 S5, merged with #28 · `self-efficacy.md` |
| 60 | Someone has already done it | Self-efficacy | Impl+P | §5 S5, §6 G7 (verified precedents only) · `self-efficacy.md` |
| 61 | Permission to fail | Self-efficacy | Impl+P | §4 fallback line, §6 G11 · `self-efficacy.md`, `output-templates.md` |
| 62 | Trust beyond your own field (Michelangelo) | Self-efficacy | Impl | §6 G12, §7.3 · `range.md` |
| 63 | Re-check what's possible often | Self-efficacy+Caveat | Impl | §6 G8 · `self-efficacy.md` |
| 64 | "Let me know if you find more" | none | Excl | Not actionable as behaviour. The one-file-per-dimension layout (§8) leaves room for new techniques anyway. |
| 65 | Heist-movie analogy | Range | Excl | Illustrates #49 and adds nothing to it. |

**Inventory check (done before delivery).**
- The matrix has **66 rows**: items 1–65 plus 2b. Every item has a row.
- 60 rows are Impl or Impl+P. 6 are Excl: #4, #5, #6, #54, #64, #65.

**Correction to Phase 1.** I wrote "57 actionable and 8 not", and later "58 and 8". Both counts were wrong: only 5 items were marked non-actionable (#5, #6, #54, #64, #65). #4 was "partly actionable" in Phase 1. It is excluded here, with its reason given in the matrix.

