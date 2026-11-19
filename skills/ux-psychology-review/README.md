# ux-psychology-review

A free Claude skill for UX reviews grounded in 106 named cognitive biases and
design principles.

- **Reviews** a screenshot, a flow or a live page: strengths, issues,
  dark-pattern flags and fixes, each tied to a named principle. Every issue
  gets a priority (Must fix / Should fix / Could improve) and says whether it
  was seen in the design or assumed.
- **Generates ideas** for a goal (activation, checkout, pricing, retention):
  concrete tactics with the principle behind them and when they backfire.
- **Flags dark patterns** such as fake scarcity, pre-ticked opt-ins or
  confirmshaming, and suggests an honest version.
- **Checks a team's decision:** reads a research synthesis, roadmap rationale
  or test write-up and flags designer-side biases (confirmation bias, anchoring,
  sunk cost, false consensus…) with the signal, a check and a concrete step.

- **Version:** 1.2.1
- **Languages:** answers in the language you write in
- **License:** MIT, see `LICENSE.md`
- **From:** Hotkeys Supply · hello@hotkeys.supply

## Requirements
- Any Claude plan with skills, including Free, and code execution turned on
  (Settings → Capabilities).
- Works in claude.ai (web and desktop) and in Claude Code.
- Reviewing a live URL needs Claude to be able to open web pages.

## Install
**claude.ai:** Settings → Capabilities → turn on code execution. Then
Customize → Skills → **+** → Create skill → Upload a skill, and pick
`ux-psychology-review.zip`.

**Claude Code:** unzip into `~/.claude/skills/` so the path is
`~/.claude/skills/ux-psychology-review/SKILL.md`.

## How to use
- `/ux-psychology-review review this checkout` (with a screenshot)
- `/ux-psychology-review ideas to get more trials to activate`
- `/ux-psychology-review what is the Peak-End Rule?`
- `/ux-psychology-review check this research synthesis for bias`

## What's inside
```
ux-psychology-review/
├── SKILL.md       # method, the 106-principle index, dark patterns
├── references/    # principles by stage, use-case index, team-decision check
├── LICENSE.md
└── README.md
```

## Good to know
The skill names principles and explains them from established knowledge. It
won't quote study results or percentages it can't source, and it flags
principles whose research is contested. Before sending a review it runs a
short checklist: a named element and principle for every issue, no invented
numbers, a dark-pattern section even when nothing was found.

## What's new in 1.2.1
- The skill description starts with what it does, so it's easier to find in
  skill directories.

## What's new in 1.2.0
- Reviews follow one fixed layout, with a priority and an Observed / Assumed
  basis for every issue, and recommendations linked to issue numbers.
- A checklist runs before every review is sent.
- Ideas name the metric to watch and how to test them.
- Reviews take the design's stage into account (exploration or polish).
