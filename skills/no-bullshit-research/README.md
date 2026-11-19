# No Bullshit Research

A Claude skill for producing research, facts, and source-backed answers that hold up to scrutiny. Built to protect the person from the reputational cost of repeating something the AI made up.

**Verify, label, cite, or abstain.** Every claim ties back to a source that was actually fetched and read. Anything that can't is dropped, marked as inference, or labeled unverified with a reason.

| | |
|---|---|
| **License** | MIT, see `LICENSE.md` |
| **Version** | 2.0.0 |
| **Author** | Bogusław Podhalicz (Hotkeys Supply) |
| **Category** | Research |
| **Output language** | Matches the language of the person's question |

## Requirements
- Any Claude plan with skills, including Free, with code execution turned on
  (Settings → Capabilities).
- **Web search turned on in Claude.** Without it the skill can't fetch sources;
  it says so and labels claims as unverified instead of guessing.
- Works in claude.ai (web and desktop) and in Claude Code.

## Install

- **claude.ai:** turn on code execution (Settings → Capabilities), then go to
  Customize → Skills → **+** → Create skill → Upload a skill, and pick
  `no-bullshit-research.zip`.
- **Claude Code:** unzip into `~/.claude/skills/` so the path is
  `~/.claude/skills/no-bullshit-research/SKILL.md`.

The skill loads `SKILL.md` when it triggers, and pulls in `REFERENCE.md` or `EXAMPLES.md` only when the situation calls for it. `README.md` is for humans and isn't loaded at runtime.

```
no-bullshit-research/
├── SKILL.md        # core: triggers, protocol, output format, self-audit
├── REFERENCE.md    # situational playbook + full red-flag catalog (loaded as needed)
├── EXAMPLES.md     # one full worked answer in the correct format (loaded as needed)
├── LICENSE.md      # MIT
└── README.md       # this file: why, install, author
```

## What changed in v2.0.0

- **Progressive disclosure.** The single monolithic file is split into a lean core plus reference and example files, following Anthropic's skill-authoring guidance to keep the core focused and load detail only when needed. Situational and brand content no longer consumes context on every trigger.
- **Redesigned output.** Research answers now open with a **Confidence Snapshot** (traffic-light bottom line + label counts + freshness), keep the answer body scannable with inline chips only on non-verified claims, present sources as a **compact table**, and close with a tight **Verification Log**. The old wall-of-text format is gone.
- **Shorter inline labels.** Inline markers are emoji + one-word tag (❓ *partial*, 🧠 *inferred*, ⚠️ *unverified*); the snapshot carries the legend so short chips stay unambiguous. Verified claims carry no inline chip, so the eye lands on what needs care.
- **Trimmed the trigger `description`** to leave headroom under the 1024-character limit, without losing its deliberately "pushy" bias toward triggering.
- **Added a worked example** so the finished output shape is unambiguous (pattern-matching beats prose instruction).
- **Same discipline underneath.** The five-stage protocol, "search again before giving up" rule, recency taxonomy, banned phrases, abstention guidance, and self-audit are all preserved.

## Why this skill exists

The cost of one fabricated AI-generated fact is never paid by the AI — it's paid by the person who repeated it.

We're living through a flood of AI-generated content that is fluent, confident, and frequently wrong in ways that aren't visible until someone external checks. A made-up statistic in a strategy deck. A fabricated quote attributed to a real expert. A "best practice" that doesn't exist. A tool comparison where one of the features was hallucinated. A 2024 fact dropped into a 2026 presentation as if the world hadn't moved. Each of these is a future moment where a client, a teammate, or a public audience says *"actually, that's not true"* — and the person who shared the AI output loses authority, even though they were trying to be helpful.

The problem compounds in fast-moving fields. AI tooling, model capabilities, framework versions, platform features, pricing — these change in weeks. The AI doesn't know it's working from a stale snapshot, because everything still *sounds* right. And the more people copy AI outputs into decks, posts, and emails without verification, the more slop enters circulation as if it were reporting — citations to papers that don't exist, statistics nobody can trace, quotes nobody actually said. The reader can't tell the difference. The person whose name is on it carries the consequence.

The skill forces a different default: verify, label, cite, or abstain. The output looks slower and more cautious than typical AI research. That's the point — it trades fluency for the ability to defend every line.

This skill is for anyone whose name gets attached to AI-assisted output — designers, leads, consultants, founders, researchers, writers, students, journalists. If your reputation depends on what you share being true, this skill is the floor under which the AI is not allowed to drop.

## Author

**Bogusław Podhalicz** — Design Lead & Product Designer working at the intersection of product design and business. Mobile apps, web platforms, design systems, research, workshops, product strategy. The thing that actually matters isn't the craft — it's the moment a client realizes that good design isn't a cost, it's a business decision.

Bogusław focuses on outcomes — not just how something should look, but why it should exist, what problem it solves, and whether it's worth building at all.

He's led a design team in a software house environment; run discovery workshops, user research, and usability tests across fintech, healthtech, mobility, and SaaS; designed hands-on while managing teams, client relationships, and product strategy; mentored early-stage startups; and spoken at industry events and co-organized design community meetups. Still designs, every day — because a design lead who stops designing stops understanding.

LinkedIn: [linkedin.com/in/bogusław-podhalicz](https://www.linkedin.com/in/bogus%C5%82aw-podhalicz/) · More tools: [hotkeys.supply](https://hotkeys.supply) · hello@hotkeys.supply
