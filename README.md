# Designer Claude Skills

Free Claude skills for product work: UX reviews tied to named principles, and research where every claim is traced to a source. Made by Bogusław Podhalicz, published by [Hotkeys Supply](https://hotkeys.supply).

## Skills

| Skill | What it does |
|-------|--------------|
| [`ux-psychology-review`](skills/ux-psychology-review) | Reviews a screenshot, a flow or a live page against 106 named cognitive biases and design principles. Lists strengths, issues with a priority, dark-pattern flags and fixes, each tied to a principle you can look up. Also checks a team's research synthesis or roadmap rationale for bias. |
| [`no-bullshit-research`](skills/no-bullshit-research) | Research where every number, date and quote is traced to a page Claude opened, labelled as uncertain, or dropped. Answers open with a confidence summary and end with a sources table and a verification log. |

### Example prompts

`ux-psychology-review`
- Review this onboarding flow and name what's working and what isn't [paste screenshot]
- Why might users drop off on our pricing page?
- Is this paywall using any dark patterns?
- Check this research synthesis for bias

`no-bullshit-research`
- What's the current state of AI design tools, with sources?
- Compare these three analytics vendors, verified facts only
- Find the actual numbers behind this claim, or tell me they don't exist

### What an answer looks like

The top of a `no-bullshit-research` answer, from the worked example in [`EXAMPLES.md`](skills/no-bullshit-research/EXAMPLES.md) (its sources are placeholders):

```
🟡 Bottom line: AI design tooling is production-ready for early-stage and
   front-of-funnel work, but claims of full end-to-end production readiness
   don't hold up. Repeat the specifics below, not a blanket "it's ready."
Confidence: ✅ 3 verified · ❓ 2 partial · 🧠 1 inferred · ⚠️ 1 unverified
Freshness: newest source 2026-06 · oldest cited 2025-11 · topic velocity: high
```

## Requirements

- A Claude plan with skills (Free included) and code execution turned on in Settings → Capabilities.
- `no-bullshit-research` also needs web search turned on. Without it, the skill says so and labels claims as unverified instead of guessing.
- `ux-psychology-review` needs Claude to be able to open web pages only when you give it a live URL.

## Install

**Claude Code, Cursor, Codex and other agents:** use the [skills CLI](https://skills.sh).

```bash
# both skills, for every Claude Code session
npx skills add bpodhalicz/designer-claude-skills -g -a claude-code

# one skill
npx skills add bpodhalicz/designer-claude-skills --skill ux-psychology-review -g -a claude-code
npx skills add bpodhalicz/designer-claude-skills --skill no-bullshit-research -g -a claude-code
```

For other agents, swap `-a claude-code` for `-a cursor`, `-a codex`, `-a github-copilot` or `-a gemini-cli`. Drop `-g` to install into the current project only.

**Manual install**

1. Download the `.skill` file from [`dist/`](dist), or the folder from [`skills/`](skills).
2. Add it to Claude:
   - **Claude Desktop:** right-click the `.skill` file, choose Open With → Claude, then confirm.
   - **claude.ai in the browser:** turn on code execution in Settings → Capabilities, then go to Customize → Skills → + → Upload a skill and pick the `.skill` file. Current steps: https://support.claude.com
   - **Claude API / Agent SDK:** use the Skills API: https://docs.claude.com/en/docs/build-with-claude/skills
   - **Claude Code:** put the unzipped folder in `~/.claude/skills/`, so the path is `~/.claude/skills/<skill-name>/SKILL.md`.

Claude loads a skill when a task calls for it. You can also call it by name, for example `/ux-psychology-review review this checkout`.

## More from Hotkeys Supply

Paid skills for the same kind of work, at [hotkeys.supply](https://hotkeys.supply):

- **wcag-master:** checks a screenshot, a Figma frame or a live URL against WCAG 2.2 AA and the European Accessibility Act, and gives the fixes.
- **design-token-builder:** builds or audits design tokens from a Figma file or a brand colour, checks contrast and exports to CSS, Tailwind or TypeScript.

The two skills in this repo stay free and work without them.

## About

Made by **Bogusław Podhalicz**, design lead and senior product designer. Find me on [LinkedIn](https://www.linkedin.com/in/boguslaw-podhalicz/). Questions: hello@hotkeys.supply

## Attribution

`ux-psychology-review`: the selection and four-stage structure follow public catalogues of cognitive biases, chiefly Buster Benson's cognitive bias codex and growth.design's *Psychology of Design* (not affiliated with either), with applied research from Nielsen Norman Group, the Interaction Design Foundation, and behavioral economics (Kahneman, Thaler, Cialdini). The one-line descriptions and the review method are original. The reference files hold summaries, not citations; the skill does not quote study results it cannot source.

## License

[MIT](LICENSE). The writing, organization and packaging are mine to share; the frameworks and research cited above remain the work of their authors, so credit them accordingly.
