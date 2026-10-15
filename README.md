# Ambitious

A Claude skill that turns "How to be more ambitious: A tutorial for humans with models" into a repeatable way of working.

`/ambitious <target> [apply | run it]` takes a prompt, a skill or a multi-folder agent and returns its **most ambitious version that can still be checked**, raised on four dimensions:

- **Altitude:** which outcome are we really after?
- **Depth:** how would the best in the field do it?
- **Range:** which other fields would change the method?
- **Speed:** the same ambition in less time.

Every escalation names the goal it serves and an outside judge. By default the skill only proposes; `apply` writes the changes, and `run it` executes them and has the judge evaluate the result.

## Layout

| Path | What it is |
|---|---|
| `SKILL.md` | The skill: the S0–S8 chain, guardrails, routing to references |
| `references/` | One file per dimension, plus access, judges, framing, input types, output templates |
| `docs/spec.md` | The full specification (2026-10-15) |
| `docs/inventory.md` | The 66 items extracted from the article, with quotes |
| `docs/traceability.md` | Each inventory item → where it is implemented, or why it is excluded |
| `evals/` | Protocol, structural checks and 10 cases |

## Install

- **claude.ai:** upload the folder as a skill. The frontmatter uses only `name` and `description`, because claude.ai rejects any other key. The "EXPLICIT-INVOCATION ONLY" wording at the start of the description is what keeps it from triggering on its own.
- **Claude Code only:** you can also add `disable-model-invocation: true` to the frontmatter. Don't do this for a claude.ai upload, which would fail.

## Status

v1, not yet evaluated. Run `evals/` before trusting it. Pass thresholds: ≥ 7/10 blind wins and 10/10 structural checks.
