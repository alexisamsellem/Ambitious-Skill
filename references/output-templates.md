# Output templates (S6)

The **ambition brief** comes first, for every input type. Write it in the language of Alexis's request. Use the English or French headings below to match.

## Ambition brief

The brief is short: **400 words at most**, before the artifact. The article's own escalations are one-sentence asks; the brief keeps that form.

```
# Ambition brief: <target name>          | # Note d'ambition : <nom de la cible>

## What breaks today (B and C)           | ## Ce qui casse aujourd'hui (B et C)
- <break>: shown by <command + output line, or file:line>.
(or "None found: <which checks ran>.")

## The ladder                             | ## L'échelle
Purpose: <the job the artifact does>. Verbs: <verb phrase>.
1. <the ask as stated>
2. <one rung higher, as a one-sentence ask>
3. <one rung higher>                     ← plan stops here (judge runs now)
4. <one rung higher>                     gated: unlock when <evidence + threshold>

## Moves                                  | ## Mouvements
- Altitude: replace <X> with <Y>. Goal: <rung>. Judge (<a–e>): <pass condition>.
- Depth: replace <X> with <Y>. Goal: <rung>. Judge (<a–e>): <pass condition>.
- Range: <field> → replace <X> with <method>. Goal: <rung>. Judge (<a–e>): <pass condition>.
- Speed: replace <wait> with <loop>. Goal: <rung>. Judge (<a–e>): <pass condition>.
(A dimension may read "Dropped: <one-line reason>". An addition reads "Add <Y> (replaces nothing): needed because <rung> cannot be reached without it".)

## Access to unlock                       | ## Accès à débloquer
- <missing>: enables <move>. How: <route>. Effort: <time>.

FALLBACK: if <plan> doesn't reach <target> by <timebox>, keep <rung below>, which still <serves goal>.
```

For B and C, the breaks come first in the plan, as the first replacements. The diff carries only those fixes and the substitutions already proven on the real target. Every new script or method is a gated rung, written as: `replace <X> with <new tool>: unlock when <test on real data> passes`.

Then the artifact for the input type (`input-types.md`). For B, the diff changes the core step; a diff that grows the target by more than a fifth must name the rung that needs the extra size.

## What the artifact asks for (G2, G14)

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
