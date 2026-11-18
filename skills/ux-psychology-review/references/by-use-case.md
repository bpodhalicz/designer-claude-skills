# Use-Case Index

When the user asks for help with a specific UX problem, look it up here to find the principles most likely to apply. Then check their summaries in the category reference files.

This index is opinionated — it lists 4-8 principles per use case, picked for *practical leverage*, not exhaustiveness. The point is to give a tight set of starting tools, not 30 things to try.

---

## Onboarding & first-run experience

The user has just arrived. They don't know what your product does, why they should care, or how to make it work. The window before they leave is small.

- **Aha! Moment** — design the first session to deliver real value fast
- **Mental Model** — match what users already know; don't make them learn yours from scratch
- **Skeuomorphism** — for novel concepts, lean on familiar real-world metaphors
- **Progressive Disclosure** — don't show every feature; reveal as needed
- **Endowed Progress Effect** — start the user with progress already on the board
- **Goal-Gradient Effect** — show how close they are to their first win
- **Curse of Knowledge** — actively check: what feels obvious to the team isn't
- **Picture Superiority Effect** — show what the product does, don't just describe it

## Activation & "first value"

User has signed up but hasn't yet experienced the core value. This is where most products lose people.

- **Aha! Moment** — what's the single action that makes them "get it"? Optimize for that
- **Pseudo-set Framing** — "3 of 5 steps to set up your account"
- **Endowed Progress Effect** — pre-fill some of the setup
- **Labor Illusion** — when work is happening (importing data, finding matches), show it
- **Variable Reward** — small wins along the way keep momentum
- **Cognitive Load** — strip the activation flow to the absolute minimum

## Pricing & paywall

Users decide whether to pay. The framing of options dominates the choice.

- **Anchoring Bias** — the first/most-prominent price frames everything else
- **Decoy Effect** — a third, deliberately worse option makes a target option look better
- **Centre-Stage Effect** — the middle plan in a row of 3 is perceived as the default
- **Framing Effect** — "$10/month" lands differently than "$120/year"
- **Cashless Effect** — abstract payment (credits, points) reduces felt cost
- **Loss Aversion** — frame upgrade as avoiding loss ("you'll lose access to…")
- **Social Proof** — "most popular" tag on the target plan
- **Reactance** — heavy-handed pressure backfires; users push away

## Checkout & purchase

User has decided to buy; the goal is now to remove every reason to stop.

- **Cognitive Load** — strip everything not essential to completing
- **Selective Attention** — keep the CTA visually dominant
- **Friction (reduce)** — fewer steps, fewer fields, smarter defaults
- **Default Effect** — pre-select sensible options (shipping, payment method)
- **Feedback Loops** — confirm every action; never leave the user uncertain
- **Loss Aversion** — show what's saved/in cart prominently
- **Trust signals (Authority Bias, Social Proof)** — security badges, recent buyer count
- **Sunk Cost Fallacy** — show progress through the flow

## Cart abandonment & re-engagement

User left without converting. Get them back.

- **Zeigarnik Effect** — unfinished business lingers in memory; remind them
- **External Trigger** — email, push, retargeting
- **Loss Aversion** — "your cart will expire" or "your discount ends"
- **Scarcity** — but only if real; fake countdowns destroy trust on return
- **Endowment Effect** — "your items" framing; they already feel ownership
- **Reciprocity** — small offer (free shipping, 10% off) creates obligation

## Retention & habit formation

Get the user to come back, repeatedly, on their own.

- **Variable Reward** — unpredictable positive feedback is the engine
- **Investment Loop** — the more they put in, the more they have to lose by leaving
- **Endowed Progress Effect** — streaks, levels, completion %
- **External + Internal Trigger** — start with notifications, transition to internal cue
- **Mere Exposure Effect** — repeated benign exposure builds preference
- **Peak-End Rule** — make the end of each session feel good
- **Method of Repetition** — daily structure cements habit

## Cancellation, downgrade, deletion

User wants out. Ethical design respects this. Dark-pattern flag territory.

- **Reactance** — making it hard creates active resentment, often public
- **Sunk Cost Fallacy** — *can* be used ethically ("you've earned X — sure?") or as a trap
- **Loss Aversion** — show what they'll lose, briefly and honestly
- **Reciprocity** — last-chance offer, but only one, and graceful if declined
- **DARK PATTERN ALERT:** confirmshaming, hidden cancel buttons, multi-step mazes, requiring phone calls — these are the canonical examples of UX patterns that cross the line. Flag them.

## Error states & failures

Things broke. The user is frustrated and ready to leave.

- **Empathy Gap** — the team writing copy isn't in the user's emotional state; test with stressed users
- **Negativity Bias** — one bad error outweighs many good experiences in memory; over-invest here
- **Peak-End Rule** — a graceful recovery can become the *positive* peak
- **Feedback Loops** — be specific about what broke and what to do
- **Self-Reference Effect** — "your file" is more emotional than "the file"; use thoughtfully
- **Pratfall Effect** — owning the failure with humor and humanity often increases trust

## Decision-heavy interfaces (settings, dashboards, search)

The user has too many options and unclear paths.

- **Hick's Law** — fewer top-level options
- **Choice Overload / Paradox of Choice** — defaults + smart filters > raw lists
- **Progressive Disclosure** — most users want 3 settings, not 30
- **Decision Fatigue** — order matters; put easy decisions first
- **Visual Hierarchy** — make the recommended path the obvious one
- **Recognition over recall** (Nielsen heuristic, outside the 106) — show options; don't make users remember them
- **Chunking / Miller's Law** — group settings into small clusters, not flat lists

## Trust-building (new brand, sensitive data, high-stakes transactions)

User has no reason to trust you yet. Earn it.

- **Authority Bias** — visible certifications, press, expert endorsement
- **Social Proof** — real testimonials, recent activity, user counts
- **Halo Effect** — quality of design itself signals trustworthiness
- **Aesthetic-Usability Effect** — pretty signals competent
- **Pratfall Effect** — small admitted limitations increase credibility
- **Familiarity Bias** — known patterns (lock icons, clear footers) reassure
- **Transparency over manipulation** (guiding rule, outside the 106) — long-term trust beats short-term conversion

## Persuasion & landing pages

You have one shot to convince a stranger to do something.

- **Anchoring Bias** — lead with a strong reference point
- **Framing Effect** — gain frame vs. loss frame, depending on audience
- **Storytelling Effect** — narratives are remembered; bullet lists are not
- **Self-Reference Effect** — "you" beats "we"
- **Curiosity Gap** — for headlines: tease, don't deliver everything
- **Picture Superiority Effect** — image > paragraph
- **Social Proof + Authority** — both, in moderation
- **Single Singular CTA (Singularity Effect)** — one ask, not five

## Notifications & engagement messaging

When and how to reach back into the user's day.

- **External Trigger** — the notification itself
- **Internal Trigger** — what emotional state should the message catch?
- **Reactance** — too many notifications → uninstall
- **Variable Reward** — make it worth opening (not just "you have an update")
- **Self-Reference Effect** — personalize, but don't be creepy
- **Peak-End Rule** — what's the last thing they remember the app doing? Make sure it was good

---

## Reverse lookup: "I want to use principle X — where does it apply?"

If the user names a principle and asks where it's used, search this file for the principle name and check the use cases it appears under. That gives you concrete contexts where it's a high-leverage tool.

For principles not appearing here, check their entry in the category reference file — the "When to apply" section is the answer.
