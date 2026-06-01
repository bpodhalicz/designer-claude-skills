# Designer Claude Skills

> A growing library of Claude skills that encode how experienced practitioners actually think - UX psychology, rigorous research, sharp critique, and more. For people building digital products, not only designers. AI that reasons like a craftsperson, not a generic prompt.

## Why this exists

Generic AI gives you text. These skills give you judgment.

Each one teaches Claude a specific way of working - a named framework, a discipline, a way of reasoning, and makes it apply that every time instead of defaulting to a confident-sounding average. The result is output you can actually ship: a UX critique grounded in real principles, research that survives a fact-check, a decision you can defend.

Built by a working design lead, not scraped from a prompt pack. New skills get added as the practice grows.

## What's inside

| Skill | What it does |
|-------|--------------|
| [`ux-psychology-review`](skills/ux-psychology-review) | Reviews and critiques UI/UX through 106 named cognitive biases and design principles. Tells you what a design does well, what it violates, and where it risks dark patterns - every point tied to a principle you can challenge. |
| [`no-bullshit-research`](skills/no-bullshit-research) | A research discipline that refuses to make things up. Every claim traces to a real, fetched, date-checked source; anything unverified gets flagged. Built to protect you from repeating something the AI invented. |

More on the way.

### Example prompts

`ux-psychology-review`
- Review this onboarding flow and name what's working and what isn't [paste screenshot]
- Why might users drop off on our pricing page?
- Is this paywall using any dark patterns?

`no-bullshit-research`
- What's the current state of AI design tools, with sources?
- Compare these three analytics vendors - verified facts only
- Find the actual numbers behind this claim, or tell me they don't exist

## Install

A skill is a folder (`SKILL.md` plus optional references). The packaged `.skill` files in [`dist/`](dist) are just zipped versions, ready to import.

1. Grab a skill from the [latest release](../../releases/latest) - or download the folder from `skills/`.
2. Add it to Claude:
   - **Claude.ai / Claude apps** - open Settings, find Skills, upload the `.skill` file. Current steps: https://support.claude.com
   - **Claude API / Agent SDK** - use the Skills API: https://docs.claude.com/en/docs/build-with-claude/skills
   - **Claude Code** — drop the unzipped folder into your skills directory.

That's it. Claude loads the skill automatically when a task calls for it.

## About

Built and maintained by **Bogusław Podhalicz**, design lead and senior product designer. These are the skills I use in real client and team work - sharpening how AI handles the parts of the job that need actual craft and judgment.

Find me on LinkedIn: [your-linkedin-url]

## Attribution

`ux-psychology-review` adapts the *Psychology of Design* framework from [growth.design](https://growth.design) and Buster Benson's cognitive bias codex, with applied research from Nielsen Norman Group, the Interaction Design Foundation, and behavioral economics (Kahneman, Thaler, Cialdini). Per-principle citations live in the reference files.

## License

[MIT](LICENSE). The writing, organization, and packaging are mine to share; the frameworks and research cited above remain the work of their authors - credit them accordingly.
