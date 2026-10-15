# Inventory: every actionable recommendation in the article

Phase 1 output (2026-10-15), with the corrections made during the interview:
- Speed is in scope (#2, #2b).
- Several items are re-tagged Speed.

Each item gives a quote from the article, its tag(s), and an actionability verdict. Text after **→** is an interpretation (DÉDUIT), not the article's words. The full article is deliberately not stored here (decision O9); these quotes are what justify each row of `traceability.md`.

Tags: Speed · Altitude · Depth · Range · Prerequisite · Caveat · Self-efficacy.

## A. Framing

1. **Four-type taxonomy** · Speed+Altitude+Depth+Range: "I think of ambition in four types: Speed, Altitude, Depth, and Range." Actionable.
2. **Speed: the same work in less time** · Speed: "Speed: The same work in less time, the bread and butter for AI's economic value: If you need some code written, I'll do it faster with Claude." Actionable.
2b. **Speed needs little creativity** · Speed+Caveat: "Well established and requires little creativity in how you approach AI, so I'll skip this one." Partly actionable. → Explains why the article gives no Speed method; not a scope exclusion.
3. **Uneven capabilities** · Caveat: "Models are, as Terence Tao puts it, 'astounding in some directions, while inadequate in others'." Partly actionable.
4. **Not model-specific** · Caveat: "my advice is not model-specific." Partly actionable (excluded in the matrix).
5. **Low-ambition default / rallying cry** · none: "wondering what they're good for beyond asking 'What is the capital of France'…" Not actionable.
6. **Opening anecdotes** · none: "it may have helped discover a new planet…" Not actionable; the article itself hedges them.

## B. Altitude

7. **Goal beyond the goal** · Altitude: "what do you want to happen next? What's the goal beyond the goal?"
8. **Task → standing outcome** · Altitude+Speed: "I still asked Claude to fix individual crashes for me. Eventually I asked Claude to simply keep our apps crash-free."
9. **All the data; what / why / what next** · Altitude+Prerequisite: "give the model too as much data as you can get your hands on… 'Tell me what changed this quarter, why, and what we should do about it.'"
10. **Decisions** · Altitude: "Work out which three decisions are most urgent in the face of everything you've learned, and start working on potential directions with for/against arguments."
11. **Why the artifact exists** · Altitude: "The review exists so leadership catches problems early and moves money and people to the right places."
12. **Better mechanism** · Altitude: "Design a better way to do that than a quarterly deck"
13. **Backtest on own history** · Altitude (judge): "show from our own history that it would have caught things sooner"
14. **Run beside current** · Altitude: "run it beside the current one for a quarter."
15. **Escalate step by step** · Altitude: "We'll start basic and get a little bit more ambitious with each step"
16. **Fits a real end outcome** · Caveat: "The altitude approach works best if you really are after some ultimate outcome"
17. **Less suited to creative work** · Caveat: "it works less well for creative endeavors."
18. **Meetings are the tell-tale sign** · Caveat: "A good tell-tale sign that ambition in altitude is a good idea is if you're going to have meetings to discuss whatever you're working on."
19. **"Go make money" ceiling** · Caveat: "There are currently limits ('Claude, go make money' doesn't seem to work for most businesses by itself in 2026)"
20. **Ceiling rises with capability** · Caveat: "models seem to be able to operate at higher levels of abstraction the more capable they become."
21. **Durable workflows** · Altitude+Speed: "Altitude is also where people find durable workflows that take the human out of the loop"
22. **Changing the workflow comes first** · Prerequisite: "Doing this well often involves changing your workflow"
23. **Independent reproduce and verify** · Prerequisite: "fetch crash reports, understand which app version maps to what git commit, and give it access to Windows, macOS, and Linux computers so it can actually independently reproduce and verify fixes."

## C. Depth

24. **Expert grade, until experts learn** · Depth: "pushing the model to use the tools, techniques, media, and knowledge employed by the best professionals in the field — and to keep pushing until even those people might learn something new from your work."
25. **Instruments, not vocabulary** · Depth: "models often switch vocabulary without actually switching methods… insist on the use of databases and statistical models."
26. **User needn't know the tools** · Depth: "You don't necessarily have to know what the experts use, Claude usually does."
27. **Unreasonable target** · Depth+Self-efficacy: "You need your website to load in 5s instead of 10s? Ask for 200ms."
28. **Reasonable, keep going** · Depth+Self-efficacy: "tell the model that they're very reasonable… Reiterate that it's very much solvable, it just needs to keep going."
29. **Raw information** · Depth+Prerequisite: "Give the model access to the raw information and data"
30. **Check assumptions against raw data** · Depth: "'We believe churn is an onboarding problem. Try to reproduce that from the raw data.'"
31. **Blind spots** · Depth: "once Claude is already deep inside the data, ask it to find blind spots."
32. **Model that reproduces the past** · Depth: "Build a simulation of our customers that reproduces the last year from our logs."
33. **Predict on unseen data** · Depth (judge): "find the earliest signal of churn we don't know about yet, and show it predicts on data it has not seen."
34. **No self-judgment** · Depth+Caveat: "Do not ask the model to judge itself… insist on outside validation."
35. **Judge = tool with immediate feedback** · Depth+Speed: "Ideally that's a tool the model can run to get feedback immediately."
36. **Self-judgment limit is dated** · Caveat: "I assume that this will eventually be solved with increasing model intelligence, but in October 2026…"
37. **A mix, not a checklist** · Caveat: "I've found a mix of the following techniques useful"
38. **Deeper, not bigger** · Depth+Caveat: "I want a deeper version of this task, not a bigger one."
39. **Protocol Q1** · Depth: "(1) say what a top professional in this field would do here that I'm not asking for"
40. **Protocol Q2** · Depth: "(2) name the rawest material they would start from instead of what has already been digested for me"
41. **Protocol Q3** · Depth: "(3) name the specific methods and tools they would use"
42. **Protocol Q4** · Depth: "(4) say what, other than you or me, would show the result is right"
43. **Protocol rewrite** · Depth: "Then rewrite my prompt to ask for exactly that."

## D. Range

44. **More fields than was economical** · Range: "consider our work from the perspective of different fields — more fields than would have been economical in the past."
45. **Multi-agent for fields** · Range+Speed+Prerequisite: "As AI products make it easier and easier to run multi-agent systems… I've seen really interesting results by imploring Claude to bring in additional fields."
46. **Tools from distant fields** · Range: "Until I saw my colleague Alex Albert use Blender to render interior designs, I never considered using Claude for 3D environments"
47. **Nouns → verbs** · Range: "A quarterly review isn't 'a deck'. It's 'getting busy people to believe a story about cause and effect, and to decide under uncertainty, in 30 minutes'."
48. **Verbs → fields** · Range: "Having the verbs makes it easier for both me and Claude to understand which fields might bring in a unique and useful perspective."
49. **Raise the stakes, assemble the crew** · Range: "The deck needs to be amazing, otherwise aliens will blow up Earth. What kind of team will humanity get together?"
50. **Production crew by delivery** · Range: "I'd bring in an analyst, a journalist, and an editor. If it has to be presented, probably a motion and audio designer, too."
51. **Red team** · Range+Depth: "an adversarial 'red team'… a short seller and a forensic accountant."
52. **No role-play** · Caveat: "Don't ask the model to write a short seller, ask it to do what a short seller does to research their position."
53. **Crew finds methods** · Range: "Use this method to find fields and techniques."
54. **"Where the magic happens"** · Range: "this is easily where I see the most magic happen." Not actionable.

## E. Prerequisites

55. **Computer, software, data access** · Prerequisite: "require the model to have a computer with the ability to install software and access to all kinds of relevant data (either using MCP connectors or other means)."
56. **Use a tool that provides this** · Prerequisite: "Plenty of tools make this possible and I recommend that you use one." Partly actionable.

## F. Self-efficacy

57. **Specific hard goals** · Self-efficacy: "humans who are given specific hard goals perform better than those who are simply told to try their best."
58. **Audacious goals + tight deadlines** · Self-efficacy+Speed: "chronicling the many things humans have accomplished when given both audacious goals and tight deadlines."
59. **Believe it possible** · Self-efficacy: "Accomplish hard things by believing them to be possible" (Dantzig).
60. **Someone already did it** · Self-efficacy: "Accomplish hard things after watching somebody else do them" (Bannister, Sawe).
61. **Permission to fail** · Self-efficacy: "Accomplish hard things by giving yourself permission to fail" (Inner Game, Linux "just a hobby").
62. **Trust beyond your field** · Self-efficacy: "we usually trust ourselves only in very narrow disciplines. Michelangelo famously didn't want to paint the Sistine Chapel"
63. **Re-check what's possible** · Self-efficacy+Caveat: "In a world where our abilities make leaps every couple of weeks, we need techniques that allow us to do things we didn't really consider or believe possible."
64. **"Let me know if you find more"** · none: "If you find more techniques that allow you to be more ambitious, please let me know!" Not actionable.
65. **Heist-movie analogy** · Range: "every single heist movie spends the first 30 minutes assembling a diverse cast" Not actionable.

**Count:** 66 items (1–65 plus 2b): 60 implemented, 6 excluded (#4, #5, #6, #54, #64, #65). See `traceability.md`.
