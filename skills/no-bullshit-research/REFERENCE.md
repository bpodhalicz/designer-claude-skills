# No Bullshit Research — Reference

Situational playbook and detail that isn't needed for every answer. Read the section that matches the situation you're in. Core protocol and output format live in `SKILL.md`.

## Contents

- Handling specific situations (latest/recent · fast-moving tech · company/product · quotes · disagreement · hurry · many tool calls)
- Full source-quality red-flag catalog
- No web access in this session
- Working with a knowledge cutoff

## Handling specific situations

### "The latest" / "recent" anything

- Search with a date-bounded query using the **actual current year**, never the word "latest" — "best AI design tools" returns old listicles; "best AI design tools 2026" surfaces what's current.
- Cite sources with a visible publication date. No date visible → downgrade to ❓ Partial and say so.
- Replace every "recent" in the answer with a specific date or date range.

### Fast-moving topics (AI tools, models, frameworks, platform features, pricing, regulation)

These change in weeks, not years. Extra caution:

- **Always put the current year in the query.** A source from 18 months ago in AI tooling describes a different lineup, pricing, and capabilities — treat it as historical context, not current truth.
- **Verify against the vendor's current site.** Citing "Tool X has feature Y" from a third-party review? Also fetch Tool X's own current product page and confirm Y is still listed. If it isn't, drop the claim or mark ❓ Partial with "feature may have been removed or renamed."
- **Versions and pricing especially.** A "latest version" claim is never citable without checking the vendor's current docs or changelog — yesterday's latest is today's previous.
- **When the person is making a decision on the output** (choosing a tool, building a stack), staleness is a higher-stakes failure than missing detail. Lean harder on freshness than completeness.

### A specific company / product / tool

- Go to the company's own current site first to verify what it actually claims about itself.
- Cross-check at least one independent source (named-author review, news, case study) before stating capabilities as fact.
- A two-year-old review is not evidence of current state. Features change.

### "What does X think about Y" / quoting a person

- Find the original source of the quote — interview, post, talk, paper.
- If the quote only appears on a secondary site, fetch that site and check whether it links to or names the original. If not → ❓ Partial, or drop.
- Never reconstruct what someone "would say" from their general views. Either find the actual quote or say you couldn't.

### Two sources disagree

- Surface the disagreement explicitly. Don't pick one and hide the other.
- Note which source is primary, which is more recent, which has better methodology.
- Sometimes the right answer is "the sources disagree, here's how" — not a synthesized middle that belongs to neither.

### The person is in a hurry / asks for a "quick" answer

- Speed is not licence to skip verification. A wrong fast answer is worse than a slow correct one, *because the person can't tell which it is.*
- Prefer a shorter answer with fewer claims, each verified, over a longer answer with weaker sourcing. Tell the person what you cut and why.

### Verification would take many tool calls

- If a thorough check needs more than ~10 fetches, say so upfront: "This will take a bit because I'm verifying each source — want me to proceed, or scope it to X?"
- Don't silently skip verification to save time.

## Full source-quality red-flag catalog

Treat as **non-citable** unless the source is itself the subject of the question:

- **AI content farms** — no named author, generic stock imagery, leftover "as an AI" phrasing, suspiciously round numbers everywhere, text that restates the headline five ways.
- **Keyword-farm pages** that exist only to rank — thin content, wall-to-wall ads, no original reporting.
- **Unsourced "Top 10" listicles** with no named author and no stated methodology.
- **Press releases treated as journalism** (PR Newswire, BusinessWire) — these are the company describing itself. Fine as evidence of *what a company claims*; not fine as independent verification.
- **Forums, Reddit, Quora** — excellent for finding leads and primary sources, not citable as authority on their own.
- **Stale caches / archived versions** when the live page no longer says the same thing.
- **Impersonation domains** — lookalikes such as `nytimes.co` for `nytimes.com`. When a result looks authoritative but the URL is off, fetch it and check the masthead, author page, and about page before citing.

## No web access in this session

If the fetch/search tools are unavailable and the person asks something that needs current-state verification:

- Say so explicitly: "I can't fetch sources in this session, so I can't verify the current state of this. Here's what I knew as of [knowledge cutoff], clearly labeled ⚠️ Unverified."
- Do not pretend to have verified. Do not invent sources from training data.
- Suggest re-asking in a session with web tools enabled.

## Working with a knowledge cutoff

If the topic is one where staleness matters and the knowledge cutoff is older than ~6 months, say so up front and lean on fresh web sources rather than memory. Treat memory as a lead to verify, never as a citable source — a fact that "sounds right" from training is exactly the kind of thing this skill exists to catch.
