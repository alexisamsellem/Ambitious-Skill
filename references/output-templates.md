# Output templates (S7)

The **ambition brief** comes first, for every input type. Write it in the language of Alexis's request. Use the English or French headings below to match.

## Ambition brief

```
# Ambition brief: <target name>          | # Note d'ambition : <nom de la cible>

## Goal ladder                            | ## Échelle d'objectifs
1. Stated: <what was asked>
2. Beyond: <what that serves>
3. Beyond: <highest viable rung>  ← target
Purpose of the artifact: <the job it does>
Verbs: <verb phrase>

## Altitude                               | ## Altitude
Applied | Dropped: <one-line reason>
- <move> (#n). Goal served: <rung>. Judge (<a–e>): <judge + pass condition>.

## Depth                                  | ## Profondeur
Applied | Dropped: <one-line reason>
- <move> (#n). Goal served: <rung>. Judge (<a–e>): <judge + pass condition>.

## Range                                  | ## Étendue
Applied | Dropped: <one-line reason>
- <field → method> (#n). Goal served: <rung>. Judge (<a–e>): <judge + pass condition>.

## Speed                                  | ## Vitesse
Applied | Dropped: <one-line reason>
- <move> (#n or "proposal"). Goal served: <rung>. Judge (<a–e>): <judge + pass condition>.
```

Every move in every dimension carries both `Goal served:` and `Judge (x):`, Speed included. A move without them fails G1: rewrite it or drop it (S6).

```

## Gated next steps                      | ## Étapes suivantes (à débloquer)
- <rung / escalation>: adds <what>. Unlock when: <evidence from the plan's judge, with threshold>. Then: <what changes in the artifact>.
(or "None: the whole ladder is provable now.")

## Access to unlock                       | ## Accès à débloquer
- <missing>: enables <escalation>. How: <route>. Effort: <time>.
(or "None: everything assumed is reachable.")

## Fallback                               | ## Repli
FALLBACK: if <ambitious version> doesn't reach <target> by <timebox>, keep <rung below>, which still <serves goal>.
```

Then the artifact for the input type (`input-types.md`).

## What the artifact asks for (G2, G16)

When the artifact makes something run (a rewritten prompt, a skill, an agent), it asks for the output in two parts:

1. **For the reader:** the answer, at the length a plain answer would have. Decision first, no method narrative.
2. **Proof pack:** the scripts, data cuts and reports every judge needs, next to the answer, plus one command that re-runs them all. A judge result with no re-runnable proof is reported as NOT JUDGEABLE.

## One-line drop reasons (G9)

A reason names the concrete cause. "Not relevant" is not a reason.

- `Altitude dropped: creative work, no outcome beyond the work itself.` (#17)
- `Altitude capped at rung 2: rung 3 ("grow revenue") is above the 2026 ceiling (#19); proposed a one-week test instead.`
- `Depth dropped: no material a judge could check.`
- `Range dropped: verbs (format, send) stay within the target's own field.`
- `Speed dropped: the 12-month observation window is the point of the study.`

## After `apply`

```
Written:
- path/to/SKILL.md (+34 −12)
- path/to/references/x.md (new)
Not written: <anything proposed but held back, and why>
```

## After `run it`

```
Run: <what was executed, on which case>
Judge (<level>): <judge> → PASS | FAIL | NOT JUDGEABLE (<why>)
Reduced: <what was missing>     (only if a reduced run was requested)
```
