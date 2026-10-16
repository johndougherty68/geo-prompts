# Intent Chain Test Prompt for GEO / AEO Marketers
**From:** Sunny Youn, GEO Pilot (geopilot.fyi)
**Use it for:** Finding where a brand drops out of AI answers as a buyer's questions narrow down
**Works in:** ChatGPT (search on), Perplexity, Gemini, Claude (web search on), Copilot

---

## Why this exists

Most AI visibility checks test one prompt. Real buyers ask a chain of follow-ups: first the category, then price, then trust, then logistics. A brand can be on the short list for the first question and gone by the third. This prompt walks the chain and shows you where the break happens and why.

---

## The prompt (copy everything in the box)

```
You are a buyer researching [CATEGORY] in [MARKET].
Your first question is: "[SEED QUESTION]"

STEP 1: Build the chain
List the 5 follow-up questions a real buyer would most likely ask next, in the order they'd ask them. Cover price, head-to-head comparison, trust/reviews, logistics (shipping, availability, returns), and alternatives.

STEP 2: Answer each link
Answer the seed question and each follow-up the way you normally would for a real user. For each answer, give the short list of 3 to 5 brands you'd recommend and the specific sources (with URLs) you relied on.

STEP 3: Score it
Make a table with these columns:
Step | Question | Brands named (in order) | Is [BRAND] named? (Y/N) | [BRAND] position | Sources cited | Why [BRAND] was included or left out

STEP 4: Diagnose every drop
For each row where [BRAND] = N, tag the cause:
- FIXABLE: missing, outdated, or negative third-party content; claims [BRAND] makes that no source confirms; weak review coverage
- STRUCTURAL: a competitor owns the category, price position, distribution or availability, regulation
Give one sentence of evidence for each tag.

STEP 5: Source gaps
List the 3 sources that most shaped the answers where [BRAND] was missing. For each: what it says, whether it mentions [BRAND] at all, and what it says that [BRAND]'s own site does not.

STEP 6: Claim check
List up to 5 claims [BRAND] makes about itself (from [BRAND URL]). For each, say whether you could find an independent source that supports it.

Be literal. If you are unsure why a brand was included or excluded, say "unclear" rather than guessing.
```

---

## Fill-in example

- [CATEGORY]: Korean skincare (K-beauty)
- [MARKET]: United States, online
- [SEED QUESTION]: What's the best Korean sunscreen for sensitive skin?
- [BRAND]: your client
- [BRAND URL]: your client's homepage or About page

---

## Rules that make the results trustworthy

1. **Fresh chat every run.** Memory and earlier messages skew the answers.
2. **Search turned on.** Without it, you're testing training data, which isn't what buyers see.
3. **Run it 3 times per engine.** AI answers vary run to run. Count how often [BRAND] appears out of 3, and ignore a single result.
4. **Test at least 3 engines.** ChatGPT, Perplexity and Gemini disagree more than you'd expect.
5. **Click every cited source.** Models sometimes cite pages that don't say what they claim. The "why" column is the model's own explanation, so treat it as a lead to verify, not a finding.
6. **Keep the chain fixed across runs.** After the first run, paste the same 5 follow-ups back in so you're comparing like with like.

---

## Reading the results

- **[BRAND] drops at one specific step across runs and engines:** that's your leak. Start there.
- **Drop tagged FIXABLE:** the source-gap list tells you what to publish, update, or pitch to third-party sites.
- **Drop tagged STRUCTURAL:** content alone won't fix it. That's a positioning, pricing, or partnership conversation, and it's better to know before spending a month on content.
- **Claims with no independent support:** engines can't repeat what they can't find. Get those claims onto third-party pages.

---

## Limits (be honest with clients)

- This is a manual snapshot. Results shift week to week as engines and sources change.
- The model is reporting on its own behavior, which is useful but imperfect.
- Doing this across 8 engines, many queries, and every client each week is the part that needs tooling. That's what GEO Pilot automates: intent chains, leakage alerts, threat tiering, and source-gap briefs.

Free AI Readiness Audit: geopilot.fyi
