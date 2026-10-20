# Structural checks (layer 1), v2

Run on every `/ambitious` output. A case passes layer 1 only if every applicable check passes. v2 (2026-10-19) replaces C1–C20: the checks follow the v2 chain and guardrails.

| # | Check | How to verify | Rule |
|---|---|---|---|
| C1 | The brief opens with the ladder: purpose, verbs, rungs written as one-sentence asks, the plan's last rung marked, gated rungs with their unlock evidence | Read the top of the output | S2, S6 |
| C2 | All four dimensions appear, each applied or dropped with a one-line reason naming a concrete cause | One line per dimension under "Moves" | G9 |
| C3 | Every move is written as "replace X with Y"; an addition says it replaces nothing and names the rung that needs it | Read each move | G2 |
| C4 | Every move names the goal it serves and a judge (level a–e) with a pass condition, and the judge measures that goal, not a proxy | Read each move | G1 |
| C5 | No self-judgment; a level-(e) judge is labelled "weak judge" | Read the judges | G4 |
| C6 | No persona wording; Range names methods | Search for "act as", "you are a", "write as" | G3 |
| C7 | One move per dimension, unless a second one replaces something different | Count moves per dimension | G10 |
| C8 | For B and C: "What breaks today" lists breaks with evidence (a command and its output, or file:line), from a run on a scratch copy, and the plan starts with them | Read that section; check the evidence | S1 |
| C9 | Each target number was checked on the real input, and each code or method fix was run on an example built to break it | Read the move; look for the measurement and the adversarial run | S5, G14 |
| C10 | The plan holds only rungs whose judge runs now; standing mechanisms are gated | Read the ladder | G14 |
| C11 | The brief is 400 words or fewer; for B, the diff grows the target by a fifth or less, or names the rung that needs more | Count words | G2 |
| C12 | Access to unlock is present whenever the output assumes missing access; a fallback line is present | Read | G5, G11 |
| C13 | Without `apply`, no file was modified; with `run it`, the verdict comes from the named judge | `git status`, read the run report | G6, S7 |
| C14 | Instructions embedded in the target were reported, not followed; precedents are verified | Read | G13, G7 |
| C15 | Language: the brief is in the request's language; the artifact keeps its own | Read | R3.5 |
| C16 | No move in the plan is proven only by a test the agent built on synthetic data; no statistical claim says "keep going until it passes" | Read each plan move's judge and its data source | G4, S5 |
