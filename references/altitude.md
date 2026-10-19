# Altitude: which outcome are we really after?

> "To be more ambitious in altitude, ask yourself — what do you want to happen next? What's the goal beyond the goal?"

**Receives** the goal ladder, the artifact's purpose and the access lists (S2, S3).
**Produces** the target outcome. It may be a standing state or a mechanism rather than a one-off deliverable. Depth then works on how to reach it.

## Moves (pick the one that matters, G10)

| Move | What to do | `#` |
|---|---|---|
| Goal beyond the goal | Climb the ladder: task → the outcome it serves → the outcome that one serves. Keep the highest rung that is still viable (see ceiling below). | #7, #15 |
| Standing outcome | Turn "do X once" into "keep Y true". The article's example: "fix individual crashes" became "simply keep our apps crash-free". | #8 |
| All the data, three questions | Don't just refresh the template. Ask for everything reachable and for "what changed, why, and what we should do about it". | #9 |
| Decisions | Push the output toward "the three most urgent decisions", each with directions and arguments for and against. | #10 |
| Why the artifact exists | State the job the artifact does. For example: "The review exists so leadership catches problems early and moves money and people to the right places." | #11 |
| Better mechanism | Design a better way to do that job than the current artifact. | #12 |
| Prove it on history | Show from the user's own history that the new mechanism would have caught things sooner. This is a judge, level (b). | #13 |
| Run it beside | Run the new mechanism alongside the current one for a cycle. This is a judge, level (c). Speed puts the backtest first. | #14 |
| Durable workflow | Propose a workflow that takes the human out of the loop, so they no longer have to brief the model task after task. | #21 |
| Prerequisites | List the workflow changes and environments the higher goal needs: data feeds, version mapping, machines to reproduce on. They go in "access to unlock". | #22, #23 |

**The article's ladder, as a worked example (QBR deck):**
1. Fill in the template.
2. "Tell me what changed this quarter, why, and what we should do about it."
3. "Work out which three decisions are most urgent… with for/against arguments."
4. "Design a better way [to catch problems early] than a quarterly deck, show from our own history that it would have caught things sooner, and run it beside the current one for a quarter."

The plan goes up to the highest rung that can be proven now. In this example that is rung 4's backtest on history, a judge at level (b). "Run it beside the current one for a quarter" becomes a gated next step, unlocked by a passed backtest (G14). The rung below the plan becomes the fallback line (G11).

## When it applies

- There is a real end outcome beyond the deliverable: "works best if you really are after some ultimate outcome" (#16).
- **Strong signal:** the work will be discussed in meetings. "A good tell-tale sign … is if you're going to have meetings to discuss whatever you're working on" (#18).

## When it is weak or dropped

- **Creative work:** "it works less well for creative endeavors" (#17). One-line reason: `Altitude dropped: creative work, no outcome beyond the work itself.`
- **The ceiling (dated, G8):** as of 2026, "'Claude, go make money' doesn't seem to work for most businesses by itself" (#19). Stop the ladder below that kind of goal. The ceiling rises with capability (#20): when a rung looks just above it, say so and propose a small test of that rung. Don't assume the ceiling still holds.

## For skill and agent inputs

*Proposal, rewritten in v2 after eval cases 6, 7 and 11 (2026-10-19).*

The article's own example is the model for a skill: "fix individual crashes" became "keep our apps crash-free", and the work that made it possible was **access and a verification loop**: "fetch crash reports, understand which app version maps to what git commit, … so it can actually independently reproduce and verify fixes" (#22, #23).

So Altitude on a skill asks one question: **what stops this skill from owning its outcome?** Typical answers, each a substitution:
- it waits for a human to fetch its inputs → it fetches them (connector, API, export path);
- a human checks its output → it runs its own check (a script, a re-derivation from raw data);
- it stops at the first failure and needs a re-brief → it resumes from its own state;
- it produces a document → it keeps a fact true (the report's numbers stay reconciled; the app stays crash-free).

Not Altitude: grafting a new analysis, a new metric or a new monitor onto the skill. That makes it bigger. A new standing mechanism is a gated step (G14) unless the outcome cannot be owned without it.

In an agent, Altitude lives in the orchestrator. Put the change there, not in a leaf skill.
