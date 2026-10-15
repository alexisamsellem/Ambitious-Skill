# Access and prerequisites (S3)

> "All the ways in which I describe ambition require the model to have a computer with the ability to install software and access to all kinds of relevant data (either using MCP connectors or other means). Plenty of tools make this possible and I recommend that you use one." (#55, #56)

Ambition in Depth and Altitude runs on access: raw data, real instruments, environments in which to verify. S3 finds out what is actually reachable *now*, so that S4 can be ambitious and the brief can be honest about what it assumes.

## What to check

| Check | Why it matters | Inventory |
|---|---|---|
| Can the model run code and install software in this session? | Real instruments (databases, statistical models, profilers) need a computer, not a chat window. | #55, #25 |
| Is the **raw** data reachable, or only digested data (a template, a summary, a dashboard export)? | Depth starts from "the rawest material", not what "has already been digested for me". | #29, #40 |
| Which connectors and MCP servers are connected, and which failed to connect? | A failed connection is not a missing capability. Name it so it can be fixed. | #55 |
| Can the model reproduce and verify on its own (environments, test data, logs, version → commit mapping)? | This is what makes the higher-altitude goal possible: "so it can actually independently reproduce and verify fixes". | #23 |
| Which outside judges are reachable (a runnable test, held-out data, a live metric)? | G1 needs a judge for each escalation. The judge hierarchy is in `judges.md`. | #34, #35 |
| What workflow change would have to happen first? | "Doing this well often involves changing your workflow." | #22 |

A blocked route (403, WAF, login wall) is not the end of the road. Name the alternative: the connected Chrome, the built-in browser, a Search Console export, or a screenshot from Alexis.

## The "access to unlock" list (goes in the brief)

```
ACCESS TO UNLOCK
- <what is missing>: enables <dimension / escalation>. How: <connector | MCP | file export | Chrome | environment | permission>. Effort: <minutes/hours>.
```

Example:
```
- Raw churn events (not the monthly churn chart): enables Depth #30–#33 (reproduce the onboarding belief, simulation, held-out signal). How: warehouse read access or a CSV export of the events table. Effort: ~15 min for Alexis.
```

## No silent downgrade (G5)

- Always write the artifact that **assumes** the access. Never quietly rewrite it to fit what is reachable today.
- If Alexis asks for `run it` and access is missing, run a reduced version only if they ask for one, and label it `reduced: <what was missing>`.
- The article recommends using a tool that provides access but names none (#56). Name the concrete tool from context: the connector, the export path, the environment.
