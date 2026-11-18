# Checking a Team's Decision — Designer-Side Biases

The other half of design psychology. The 106 principles describe how **users**
think; the same biases shape how **the team** researches, decides and defends
its work. This file covers the ones that most often bend design decisions, with
the signal to look for in a document and the check that tests it.

Every entry maps to a principle already in the index (number in brackets), so
names stay consistent across reviews.

## How to use it
1. Read the artefact: a research synthesis, a decision log, a roadmap
   rationale, an A/B test write-up, a pitch deck, an estimate, a design
   rationale.
2. Note the decision and the evidence offered for it.
3. Walk the biases below. Flag only the ones with a visible signal in the
   artefact. Quote or point to the signal.
4. For each flag, give the check (a question or a small test) and a concrete
   step that would reduce the risk.
5. Close with a verdict: the decision holds as it stands, holds after the
   checks, or should be revisited.

**Tone rule.** These are risks to test, not accusations. Write "this could be
confirmation bias; here's how to check" rather than "you are biased". A bias
flag is a hypothesis about the process, never a judgement of the people.

---

## Confirmation Bias [29]
**Shows up as:** research synthesis that quotes only what supports the idea the
team already liked; test questions that lead toward the hoped-for answer.
**Signal:** every quote agrees; no "against" or "surprising" section; the
hypothesis was written before the research and survives unchanged.
**Check:** what would we expect to see if we were wrong? Is that evidence
missing, or was it never looked for?
**Step:** add a "disconfirming evidence" section; have someone outside the
project tag the raw notes before reading the synthesis.

## Anchoring Bias [7]
**Shows up as:** estimates, prices or targets that stay close to the first
number anyone said.
**Signal:** the final figure sits near an early guess, a competitor's number or
a client's budget, with no independent estimate.
**Check:** where did the first number come from, and was a second estimate made
before seeing it?
**Step:** estimate independently first, then compare; use ranges, not points.

## Sunk Cost Fallacy [65]
**Shows up as:** keeping a feature, a direction or a vendor because of what was
already spent on it.
**Signal:** "we've already built…", "after three months of work…" used as the
reason to continue.
**Check:** if we were starting today with what we know now, would we choose
this?
**Step:** judge the next step on future cost and value only; write down what
would make you stop.

## False Consensus [61]
**Shows up as:** "users will obviously…" based on how the team itself works.
**Signal:** claims about users with no user evidence; personas that look like
the team.
**Check:** which users said or did this? How many, and how were they found?
**Step:** mark assumptions as assumptions; test the riskiest one with real
users before building on it.

## Curse of Knowledge [60]
**Shows up as:** labels, flows and onboarding that make sense only to people
who know the product.
**Signal:** internal jargon in UI copy; "it's self-explanatory" without a test
with someone new.
**Check:** has anyone outside the team tried this without help?
**Step:** a five-minute test with someone who has never seen the product.

## Survivorship Bias [31]
**Shows up as:** copying the patterns of successful products while ignoring the
ones that used the same patterns and failed.
**Signal:** benchmarks drawn only from market leaders; "Company X does it, so it
works".
**Check:** do we know it works for them, or only that they do it? Who tried it
and dropped it?
**Step:** treat benchmarks as ideas to test, not evidence.

## IKEA Effect [58]
**Shows up as:** overvaluing a solution because the team built it.
**Signal:** an internal design defended against user feedback; alternatives
rated lower without the same scrutiny.
**Check:** would we rate it the same if another team had made it?
**Step:** compare options against the same criteria, ideally scored blind.

## Planning Fallacy [89] and Optimism Bias [88]
**Shows up as:** timelines and adoption forecasts that assume everything goes
right.
**Signal:** no buffer; no reference to how long similar work took before; best
case presented as the plan.
**Check:** how long did the last comparable project take, against its plan?
**Step:** plan from past actuals (reference class), and show a realistic and a
pessimistic case next to the best one.

## Hindsight Bias [44]
**Shows up as:** post-mortems that say the outcome was obvious.
**Signal:** "we always knew…" with no record of that prediction beforehand.
**Check:** what did the team actually predict before launch? Is it written
down?
**Step:** record predictions and confidence before launches and tests.

## Survey Bias [45] and Framing Effect [20]
**Shows up as:** research results shaped by how the question was asked.
**Signal:** leading or double-barrelled questions; options that frame one answer
as the default.
**Check:** read the exact wording. Would a neutral version change the answer?
**Step:** rewrite questions neutrally; pilot them with two or three people.

## Authority Bias [39] and Bandwagon Effect [41]
**Shows up as:** decisions made because a senior person or the industry trend
said so.
**Signal:** "the CEO wants it", "everyone is doing AI" as the main reason.
**Check:** what evidence would convince us if the same idea came from a junior
person or a small competitor?
**Step:** separate the source of the idea from the evidence for it in the
decision record.

## Status Quo Bias [67]
**Shows up as:** keeping a pattern because it's what exists, not because it
works.
**Signal:** "we've always done it this way"; changes judged on risk only, never
on the cost of not changing.
**Check:** what does staying the same cost us?
**Step:** write down the cost of no change next to the cost of change.

---

## Output shape
- **Decision under review:** one sentence.
- **Evidence offered:** a short list.
- **Bias risks:** 2–5 flags, each with the principle and number, the signal (quoted
  or pointed to), the check and the step.
- **What looks solid:** where the reasoning is well supported.
- **Verdict:** holds / holds after checks / revisit, with the one check that
  matters most.

## Further reading
- Cognitive Bias Index by Jon Yablonski, <https://cognitivebiasindex.com>:
  descriptions of common biases with how they occur and how to avoid them.
  Linked for reading only; none of its text is included here.
- Daniel Kahneman, *Thinking, Fast and Slow* (2011), for the mechanisms behind
  anchoring, planning fallacy and hindsight.
- David Dylan Thomas, *Design for Cognitive Bias* (2020), on biases in design
  teams and how to design against them.
