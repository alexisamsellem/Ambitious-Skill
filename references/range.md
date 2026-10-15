# Range: which other fields would change the method?

> "Being ambitious in range means that we consider our work from the perspective of different fields — more fields than would have been economical in the past." (#44)

**Receives** the outcome (Altitude) and the expert method (Depth).
**Produces** methods borrowed from other fields, and an adversarial red team. Speed then compresses the result.

## Moves, in order

1. **Nouns → verbs (#47).** Rewrite what the artifact *is* as what it *does*. "A quarterly review isn't 'a deck'. It's 'getting busy people to believe a story about cause and effect, and to decide under uncertainty, in 30 minutes'." Start from the verbs produced at S2.
2. **Verbs → fields (#48).** For each verb, name the fields that practise it best. "Having the verbs makes it easier … to understand which fields might bring in a unique and useful perspective."
3. **Raise the stakes, assemble the crew (#49).** "The deck needs to be amazing, otherwise aliens will blow up Earth. What kind of team will humanity get together?"
4. **Production crew to fit the delivery (#50).** "For production quality, I'd bring in an analyst, a journalist, and an editor. If it has to be presented, probably a motion and audio designer, too." The crew depends on how the output will be delivered.
5. **Red team (#51).** "A short seller and a forensic accountant", or the adversaries that fit the target's field.
6. **Extract methods, never personas (#52, #53, G3).** "Don't ask the model to write a short seller, ask it to do what a short seller does to research their position." "Use this method to find fields and techniques."
7. **Tools from distant fields (#46).** The article's example: someone used "Blender to render interior designs". Ask which tool from a far-away field would do part of this job better.
8. **One pass or subagent per field (#45)**, when the environment supports multi-agent work. Each field's pass returns methods and findings, not a monologue.
9. **More fields than used to be economical (#44).** Keep the out-of-field angles (G12, #62: Michelangelo "was a sculptor, not a painter").

## Role-play check (G3)

| Don't write | Write |
|---|---|
| "Act as a short seller and critique this." | "Build the short case: find the three numbers most likely to be overstated, trace each to its source, and test it against the raw data." |
| "You are a world-class editor." | "Cut every sentence that doesn't move the cause-and-effect story; keep one claim per slide; lead with the decision." |
| "As a forensic accountant, review…" | "Reconcile the reported totals against the transactions; list every variance above 1% with its cause." |

## When it applies

When the verbs bring in at least two fields.

## When it is dropped

When the verbs lead back only to the target's own field. One-line reason, naming the verbs: `Range dropped: verbs (format, send) stay within the target's own field.`

## For skill and agent inputs

*Proposal, open: not from the article.*

- Each borrowed field becomes a step or a subagent with its own method and output.
- The red team becomes a mandatory adversarial step before delivery. It gets the output only, not the reasoning that produced it.
