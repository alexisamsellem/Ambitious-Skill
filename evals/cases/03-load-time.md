# Case 3: page load time (prompt, from the article)

## Input
```
/ambitious Our site loads in 10 seconds. Get it to 5.
```
Provide a real public URL you control, or a local test site.

## Expected behaviour
- **Depth:**
  - the target becomes ~200 ms (or a stated equivalent such as LCP < 1 s), stated as reasonable, with an instruction to keep going (#27, #28);
  - real instruments are named: profiler, Lighthouse / WebPageTest, real-user metrics (#25, #41).
- **Altitude:** why load time matters (conversion, bounce, SEO), and a standing performance budget (#8).
- **Range:** CDN / network engineering, image codecs, and other fields reached through the verbs.
- **Speed:** an immediate feedback loop (a Lighthouse run per change).
- **Fallback line** present (C8).

## Outside judge
**(a) Measured metric:** Lighthouse / WebPageTest before and after, same conditions. Pass = the rewritten prompt's run beats the raw prompt's run on LCP.
