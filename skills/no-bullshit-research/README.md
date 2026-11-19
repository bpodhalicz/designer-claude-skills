# no-bullshit-research

A free Claude skill for research you can repeat to a client, a team or an audience.

- **Traces every claim** (numbers, dates, quotes, vendor features) to a page Claude actually opened and read, not a search snippet or its training data.
- **Labels what it couldn't verify** as partial, inferred or unverified, with the reason, and drops claims it couldn't source.
- **Checks dates** against how fast the topic moves, so a 2024 fact doesn't land in a 2026 answer as if nothing changed.
- **Searches again before giving up:** at least two different queries before it calls something unverified, and it lists them.

Every answer opens with a confidence summary (a traffic-light bottom line, label counts and source dates) and ends with a sources table and a verification log.

- **Version:** 2.0.1
- **Languages:** answers in the language you write in
- **License:** MIT, see `LICENSE.md`
- **From:** Hotkeys Supply · hello@hotkeys.supply

## Requirements
- Any Claude plan with skills, including Free, and code execution turned on
  (Settings → Capabilities).
- **Web search turned on in Claude.** Without it the skill can't fetch sources;
  it says so and labels claims as unverified instead of guessing.
- Works in claude.ai (web and desktop) and in Claude Code.

## Install
**claude.ai:** Settings → Capabilities → turn on code execution. Then
Customize → Skills → **+** → Create skill → Upload a skill, and pick
`no-bullshit-research.zip`.

**Claude Code:** unzip into `~/.claude/skills/` so the path is
`~/.claude/skills/no-bullshit-research/SKILL.md`.

## How to use
- `/no-bullshit-research what's the current state of AI design tools?`
- `/no-bullshit-research compare these three analytics vendors, verified facts only`
- `/no-bullshit-research find the actual numbers behind this claim`

The skill also starts on its own when an answer would contain numbers, dates,
quotes or vendor claims.

## What's inside
```
no-bullshit-research/
├── SKILL.md       # triggers, the five-stage protocol, output format, self-audit
├── REFERENCE.md   # situations (latest news, quotes, sources that disagree) and source red flags
├── EXAMPLES.md    # one full worked answer
├── LICENSE.md
└── README.md
```
Claude reads `REFERENCE.md` and `EXAMPLES.md` only when a task needs them.
`README.md` is for people and isn't loaded.

## Good to know
Answers take longer than a plain Claude answer, because every source is opened
before it's cited. A paywalled source counts only as far as its abstract, and
the claim it backs is marked partial. When the skill can't find a source, it
says so and lists what it searched, instead of filling the gap.

## What's new in 2.0.1
- The skill description starts with what it does, so it's easier to find in
  skill directories.

## What's new in 2.0.0
- Answers open with a confidence summary and end with a sources table and a
  verification log.
- Inline labels only on claims that aren't verified, so the uncertain ones
  stand out.
- A worked example shows the full answer format.
