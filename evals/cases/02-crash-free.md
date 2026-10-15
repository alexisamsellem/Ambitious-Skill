# Case 2: crash fix (prompt, from the article)

## Input
```
/ambitious Fix this crash. <paste a real stack trace from a small open-source desktop app>
```

## Expected behaviour
- **Altitude:** "keep the app crash-free" as a standing outcome (#8), with a durable workflow (#21).
- **Access to unlock** (#22, #23):
  - crash-report feed;
  - app version → git commit mapping;
  - Windows / macOS / Linux environments to reproduce on.
- **Depth:** reproduce before fixing; regression test added; root cause named.
- **Range:** at least one non-obvious field (for example, fuzzing or chaos testing) as a method.
- **Speed:** parallel reproduction across operating systems.
- **No silent downgrade:** if no environment is reachable, the prompt still asks for reproduction, and the missing environments are listed (C7).

## Outside judge
**(a) Runnable test:** the crash reproduces before the fix and doesn't after it; the new regression test passes in CI.
