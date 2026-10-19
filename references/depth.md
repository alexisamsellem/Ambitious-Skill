# Depth: how would the best in the field do it?

> "Being ambitious in depth means pushing the model to use the tools, techniques, media, and knowledge employed by the best professionals in the field — and to keep pushing until even those people might learn something new from your work." (#24)

**Receives** the target outcome from Altitude.
**Produces** an expert-level method: raw material, real instruments, an unreasonable but explicit target, and an outside judge. Range then widens that method with other fields.

## Core protocol (the article's own prompt, run internally)

> "I want a deeper version of this task, not a bigger one. Before rewriting it: (1) say what a top professional in this field would do here that I'm not asking for; (2) name the rawest material they would start from instead of what has already been digested for me; (3) name the specific methods and tools they would use; (4) say what, other than you or me, would show the result is right. Then rewrite my prompt to ask for exactly that."

| Step | Answer it for this target | `#` |
|---|---|---|
| 0 | Deeper, not bigger. Raise rigour; don't add deliverables (G2). | #38 |
| 1 | What a top professional would do here that wasn't asked for. | #39 |
| 2 | The rawest material they'd start from: logs, events, source files, transcripts, not the summary or the template. | #40 |
| 3 | Their specific methods and tools, by name. | #41 |
| 4 | What, other than you or the user, would show the result is right. This is the judge (`judges.md`, G1). | #42 |
| 5 | Rewrite the artifact to ask for exactly that. For skills and agents, the "rewrite" is the diff. | #43 |

## Moves around the protocol (pick the one that matters, G10)

- **Instruments, not vocabulary (#25).** "When prompted to act like a professional, models often switch vocabulary without actually switching methods." Check every Depth escalation: does it change the *method* (a database, a statistical model, a profiler, a controlled test), or only the words? A markdown table of averages is not a statistical analysis.
- **The user doesn't need to know the tools (#26).** "You don't necessarily have to know what the experts use, Claude usually does." Name them yourself.
- **Unreasonable target (#27).** "You need your website to load in 5s instead of 10s? Ask for 200ms." Aim an order of magnitude beyond the ask.
- **Keep going (#28).** "Does something seem impossible to the model? Reiterate that it's very much solvable, it just needs to keep going." Write that into the rewritten artifact.
- **Challenge what you know (#29, #30).** Get raw data and test the belief adversarially: "We believe churn is an onboarding problem. Try to reproduce that from the raw data."
- **Produce new knowledge (#31–#33).** Once deep in the data, look for blind spots: "Build a simulation of our customers that reproduces the last year from our logs. Then find the earliest signal of churn we don't know about yet, and show it predicts on data it has not seen."
- **Claims at the strength of the evidence (G14).** A test that fails to reject is "not shown", not "chance". A stable aggregate doesn't rule out a cause at the level below. *Proposal, from eval case 1 (2026-10-16).*
- **Outside judge (#34, #35).** "Do not ask the model to judge itself." Ideally use "a tool the model can run to get feedback immediately". See `judges.md`.
- **A mix, not a checklist (#37).** "I've found a mix of the following techniques useful."

## When it applies

Almost always: whenever execution quality matters and the material can be checked.

## When it is dropped

Drop it when no checkable material and no judge can exist, even with more access. One-line reason, naming what is missing: `Depth dropped: no material a judge could check (pure preference task).`

## For skill and agent inputs

*Proposal, rewritten in v2 after eval cases 6, 7 and 11 (2026-10-19).*

Ask the four questions about the skill's **core step**, the one step that produces its value (the title it writes, the number it reports, the verdict it gives). The answer is a rewrite of that step, not new steps around it.

1. What would a top professional do in this step that the skill doesn't? → the method that replaces the current one.
2. What raw material would they start from? → the input that replaces the digested one.
3. Which instrument would they use? → the tool that replaces prose instructions or manual checks. The skill's checklist written as prose becomes a script the skill runs.
4. What, other than the skill or Alexis, would show the step is right? → the judge the skill runs on every run.

Before any of this, the S1 look: run the skill as it is, and fix what breaks first. A fix to code or to a method is run once on an example built to break it (G14).

The guardrails, gates and QA layers a skill already has are not where depth lives. Adding more of them is the usual way a skill becomes bigger without becoming better.
