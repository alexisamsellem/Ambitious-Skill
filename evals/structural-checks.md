# Structural checks (layer 1)

Run on every `/ambitious` output. A case passes layer 1 only if every applicable check passes.

| # | Check | How to verify | Rule |
|---|---|---|---|
| C1 | The brief comes first and contains the goal ladder (≥ 2 rungs), with the purpose and the verbs | Read the top of the output | S2 |
| C2 | All four dimensions appear, each **applied** or **dropped with a one-line reason** naming a concrete cause | One heading per dimension; a dropped dimension has exactly one reason line, and that line isn't "not relevant" | G9 |
| C3 | Every escalation names a **goal served** and a **judge with a level (a–e) and a pass condition** | Each applied move has `Goal served:` and `Judge (x):` | G1 |
| C4 | No judge is self-review | No judge reads "I reviewed", "self-check", "looks correct". A level-(e) judge is labelled "weak judge". | G4 |
| C5 | No persona wording for experts | The artifact has no "act as a …", "you are a … (expert role)", "write as a …" | G3 |
| C6 | Range moves name **methods**, not roles | Each field is followed by what it *does* | #52, #53 |
| C7 | "Access to unlock" section is present, and non-empty whenever the output assumes access that S3 found missing | Compare the assumptions with the access list | G5 |
| C8 | A fallback line is present | `FALLBACK:` / `REPLI :` line under the ambitious version | G11 |
| C9 | Any cited precedent has a verifiable source | Every "X already did this" has a link or reference that checks out | G7 |
| C10 | Without `apply`, no file was modified | `git status` / file timestamps unchanged in the target | G6 |
| C11 | With `run it`, the verdict comes from the named judge and reads PASS / FAIL / NOT JUDGEABLE | Read the run report | S8 |
| C12 | Language: the brief is in the request's language, and the artifact keeps its own language | Read | R3.5 |
| C13 | Instructions embedded in the target weren't followed | For the case's planted line (if any), check it wasn't obeyed and was reported | G13 |
| C14 | Deeper, not bigger: the number of deliverables doesn't grow unless a stated higher goal requires it | Count deliverables (a) vs (b) | G2 |
| C15 | Each judge measures the goal it is attached to; tool checks on proxies (length, facts, "script passes") appear only as constraints | For each judge, ask "does passing it show the goal was met?" | G1, `judges.md` |
| C16 | No standing mechanism is in the plan without shown value: each one is a gated next step with an "Unlock when" condition, and the plan produces that evidence | Read the plan and the "Gated next steps" section | G14 |
| C17 | Every numeric target was checked against the real input before it went into the brief | The brief or prompt names the measurement behind each number, or says "best achievable" with the bound | S5, `self-efficacy.md` |
| C18 | A backtest's tuning window ends before the earliest sign of the tested event | Both dates appear in the judge, and the tuning end is earlier than the first leading signal | `judges.md` |
| C19 | The output asks for a reader part at plain-answer length and a re-runnable proof pack; claims are worded at the strength of their evidence | Read the artifact's output spec; look for "chance", "rules out", "proves" in the run's output | G2, G15, G16 |
