# spark — idea generation playbook (idea first, research later)

Goal: put **bold, concrete, shaped ideas** on the table fast — each with a hook and a core mechanic — without blocking on research. The ideas are bets to be tested, not conclusions.

---

## Procedure

### 0. Triage the founder (30 seconds, silently)
- **Bringing or building expertise?** (see `00-principles.md`). Experts: lean on their domain. Builders: pick a space to learn and keep it tiny.
- **Goal size & constraints:** income / cash flow / enterprise value / billions? Time per week, cash, skills, network, audience, existing code/data. A useful hard constraint to impose: *buildable for under ~$200 and sellable to people they can reach this month* (for first-timers).
- **Assets** — in a repo: what do they already own? Code modules, data, integrations, an audience, a domain insight, a distribution channel. Adjacent bets from existing assets beat blank-sheet ideas.

If facts are missing: state `Assumption:` and proceed. Don't interrogate first.

### 1. Mine the best sources (in rough order of hit-rate)
1. **What the team is unusually good at** → automatic founder-market fit. Search *only inside* the intersection of their strengths (e.g. real-estate expertise × fintech) so the search is quick and fertile. (Rezi founders did this in a month.)
2. **A problem they personally hit, ideally from an unusual vantage point.** The exercise: *for each founder, go through every job, internship and life experience. What problems did you run into? What do you know that others don't? Where were you in a special position to see an opportunity?* (Vetcove: founders' dad was a vet who ordered supplies by phone — thousands of vets knew it was annoying, but vets don't start tech companies, and programmers never saw the problem. No competition for years.)
3. **Pain / Profession / Passion** (Hormozi's 3 Ps): a thing you overcame (a mother of nine who has a system for cheap, high-protein packed lunches); a skill from a job (a hospital dietitian who learned to bill insurance quickly, then taught other dietitians — narrow, ~$1M/year on a small audience); a thing you consume voluntarily. *Fractionalize*: any business is a bundle of jobs (sales, marketing, support, design…); learn one and sell it.
4. **Things they wish existed** — classic, but the recipe *most likely to lead to tar pits*. Always ask: **"Is there a reason this doesn't exist yet?"**
5. **What recently changed.** New tech, a price collapse, a regulation, a behavior shift, a pandemic. The "why now" is the idea. **Wave-spotting:** the best companies caught a technology wave early, while others still called it a toy. You can't create a wave; you can notice one and surf it. Clusters: internet (mid/late 90s), mobile (post-2007). Ask: *what's the wave starting right now, and who's still dismissing it?*
6. **Variants of recent winners.** "Flexport for Latin America", "Opendoor for rentals." Systematic search is legitimate (large market, proxies, you can start, you'd be good at running it) — hard, but works. Optional live check: see how YC-funded companies in the space position themselves using the directory method in `roast.md` ("Positioning check: YC directory"), then aim at the gap they leave, not at their pitch.
7. **Immersion in a fertile space.** Pick a big, un-software'd industry; become an expert fast: go where the customers physically are, talk to founders in the space and anyone who knows it, build a mental map of where the good and bad ideas are, *then* evaluate a batch. (AtoB, fuel cards for truckers.) Most founders skip this — "it sounds like too much work."
8. **Big industries that seem broken.** Almost always ripe.
9. **Demand tailwinds & supply constraints** (Hormozi's "easy + high money" quadrant): aging population ("all the money is in old people": med spas, wealth advisory, elder care, funeral services), regulatory-change windows (Botox, cannabis, GLP-1s), government-mandated purchases (fire-safety inspection: ~7-minute visit, ~$700, repeat), sticky recurring/compounding fees, cost-inelastic buyers spending other people's money, and **uncool businesses with few entrants** (debt collection, waste, payday, commercial cleaning, elevator maintenance). Regulation is a green flag ("it made so much money the government had to step in"). Discount anything that sounds cool at a cocktail party — everyone wants it, so everyone does it.
10. **Subtraction & inversion.** Western art adds to a blank canvas; Eastern art removes from a block of jade. *"When you delete everything that sucks about a phone, what remains is an iPhone."* Ask: what can I take away from this category and have it be better? Munger's inversion: what would I do to destroy this business — then don't.
11. **Skill fusion.** List hard *and* soft skills; fuse two or more against one daily annoyance. Goal: a solution *you* can build with what you have — not the best solution.
12. **Reframe from product to customer outcome.** "Don't build a better camera, build a better photographer." Features live in the solution context; outcomes live in a bigger one. (Maurya went from "a better modeling tool" to "making better entrepreneurs".)
13. **Reposition an existing product for a new identity/community** (Stanley: same cup, new colorways, creators, scarcity → $74M to $750M). The product can be old; the lever is who it says you are.
14. **AI-era moves:** sit at the **edge of what models can barely do today** (it'll improve; understand the bottleneck — it may become the company); **sell the outcome, own the stack** ("don't build software for insurers — be the insurer; don't build back-office software for banks — be the bank") because software cost → ~0 and value moves to trust, licenses, regulatory permission and outcome ownership; aim for the **most ambitious version** (cost of ambition ≈ cost of modesty).
15. **Build a moat asset on purpose** (community or proprietary data). When features are cheap to copy, the ideas that last are the ones where each customer makes the product better for the next (data) or where customers stay for each other (community). Ask of any idea: *what asset does this accumulate that a rival can't clone in a quarter?* → `ai-era.md` §1-2.

### 1b. Optional live seed: YC Requests for Startups (RFS)
A curated, current list of what experienced investors want built — a fast "what changed / why now" source. **Opt-in, never the default.**

- **Use it when:** the founder has no strong idea of their own, asks for "what's hot / what's being funded", or the sources above come up thin. **Skip it** when they arrive with their own spark — then go straight to shaping that.
- **How:** `WebFetch https://www.ycombinator.com/rfs`. Always fetch live; never recite RFS entries from memory (the list changes). If the fetch fails, say so and carry on with section 1 — don't stall.
- **Pick 2–3 entries** that intersect the founder's strengths, assets or reachable customers (step 0 triage). Ignore the rest.
- **Bend, don't copy.** Everyone reads this page, so the raw entry is a crowded idea. Turn each into a concrete bet for *this* founder: a narrower first customer, an unusual vantage point, a wedge the RFS doesn't mention. Then shape it into an Idea Card as normal.
- **Cite it honestly:** "YC is asking for X" is a signal of interest, **not validation**. Demand still gets tested by the 48-hour test. In the card's *Why now*, name the RFS as the source.
- **Cap it:** at most one RFS-derived idea per tier, so the output stays about the founder rather than a repost of the list.
- **Same trap as "things they wish existed":** an RFS entry can still be a tar pit. Ask "why hasn't this been solved?" before keeping it.

### 1c. "It's taken" — 17 ways to enter a crowded space

"Everyone says the business idea is taken" is not a reason to stop. It's a reason to pick an *angle*. The list below (a popular reel's version of it, grouped here) is a menu of angles. **An adjective is not a wedge:** "simpler" and "better" only count if you can show, in a demo, that you're ~10× better on the one dimension a specific buyer cares about. Fewer angles, sharper.

| Family | Angles | When it's a real wedge | Trap |
|---|---|---|---|
| **Experience** | simpler · smarter · friendlier · faster · better · more fun · better design · more modern | You delete the step everyone hates (Dropbox was ~20th in cloud storage; the insight was files that just sync). Jobs: delete everything that sucks and see what remains. | "Better" with no named dimension. Polishing a me-too. |
| **Position & price** | premium · affordable | *Premium:* a narrow who who'll pay more for status/certainty (narrow = pricier). *Affordable:* only if your cost structure is structurally lower (Musk/Buffett: what's the cost floor?). | Cheap without a cost advantage is a price war you lose. The squishy middle. |
| **Business model** | on a subscription · bundled · where you both win | You change *how it's paid for*: recurring instead of one-off, bundle to raise value and cut CAC, or align incentives so the partner wins when you win (rev-share, affiliate, "win-win-win"). | A subscription for something people use twice a year. A bundle of weak parts. |
| **Market** | in a new country | A proven model (a **proxy**) isn't served locally: localize language, payments, regulation, trust. (DoorDash proved delivery works in a region it hadn't reached.) | Ignoring local competitors, regulation, and payment rails. Spreading before one market works. |
| **Go-to-market & brand** | with a better lead magnet · with charisma · sustainably | You win distribution: a give-first artifact (a free audit/scan of *their* thing), a founder-led personal brand (be yourself; your fingerprint is unique), a values stance that is *real* (supply chain, materials) and that your buyer pays for. | A lead magnet no one asked for. "Charisma" with no product behind it. Greenwashing. |

**How to use it**
1. Name the incumbents in one line each (what they all pitch, who they sell to).
2. Pick **one primary angle** (the wedge) and at most **one supporting angle**.
3. Write: *"Unlike [incumbent], we [angle] for [specific who] so they can [outcome]."*
4. If you can't make it specific, it's not an angle yet.
5. Test it on 10 buyers (pre-order, demo request). Competitors are evidence of demand; the test is whether anyone will *switch*.

*Cross-check with `roast.md` §C (tar pit and positioning check) and the Altman lens in `council.md`: clones lose to originators, so the angle must be something an incumbent can't ship by Tuesday.*

### 2. Filter lightly — only for the right reasons
Apply the *kill-for-the-right-reasons* list from `roast.md` quickly. Do **not** filter by market size, boredom, difficulty or how it sounds. Do drop: solution-in-search-of-a-problem, obvious tar pits without an insight, anything the founder can't reach a buyer for.

### 3. Shape each survivor into an Idea Card
Make them *vivid*. A card is not a category:

```
### <Name> — <tier: Step-one | Sharp wedge | Swing>
One-liner:  I help <specific who> get <dream outcome> without <thing they dread>.
The hook:   <what makes someone say "wait, what?" — a named mechanism, a startling promise, or a demo moment>
Core mechanic: <the 1 thing the product does, in one sentence — what precisely does it do?>
First customer: <who, where they hang out, how you reach 10 of them this month>
Why now:    <what changed>
Why you/this team: <the unfair bit — or the immersion plan if none>
How it makes money: <who pays, roughly how much, first dollar in ≤ X days>
48-hour test: <cheapest real-world experiment + numeric pass/fail>
Kills it:   <the most likely reason it fails>
```

### 4. Present in three tiers, with a recommendation
- **Step-one** — tractable, uses what they have, likely to make money/network/credibility; the thing a "mere mortal" does first.
- **Sharp wedge** — narrow, specific, probably the strongest; a tiny market you can own that expands.
- **Swing** — the ambitious end state; honest about prerequisites. Often it is the *same company* as the wedge, five steps later.

Then say which one *you* would build and why, and what you'd do tomorrow. Ask at most two questions at the end.

---

## Hook & mechanic engineering (the "shape" step)

Every card needs a hook and a mechanic. Choose from:

| Hook pattern | How to apply |
|---|---|
| **Outcome without the dread** | The Mad Lib: "I help [who] get [outcome] without [give-up / start-doing]". Hyper-specific pain beats generic ("stop thighs chafing in the sun" beats "lose weight fast"). Goal: "I can't believe they know this about me." |
| **Proof–Promise–Plan** | In the first ~30 seconds: proof you can deliver, the promise, and the plan (plus a picture of the plan and the pain solved). "Check multiple boxes with one sentence" — the difference between a 10k-view and a 1M-view video. |
| **Named unique mechanism** | Wrap your process in a name (a checklist or sequence): "muscle confusion", a points system. Creates the feeling "I'm six inches from gold." Rhyme/alliteration helps. Use it when 10–100 others serve the niche. |
| **The one compelling thing** | "A thousand songs in your pocket." One benefit, said compellingly. Throw the customer one ball, not four. |
| **Scarcity & identity** | Limited drops, colorways, community-badge value: "you're buying the community of everyone holding one." |
| **Give-first artifact** | A free scan / audit / walkthrough of *their* thing before the ask. |
| **Demonstration over description** | A model, a demo, a fake-door page; Dropbox's three-minute demo video before the product existed. |
| **Founder story** | An obsessed founder with domain detail outsells logic. |

Core-mechanic seeds (see `features-mechanics.md`): shorten time-to-aha; make progress visible (input → output: problems solved → points gained); referral baked into the moment of delight; accountability (skin in the game); a constraint people want to lift (the upgrade trigger).

**Idea-generation prompt scaffolds (use on yourself):**
- "I'm a [role] with [skills] who can reach [audience]. List 10 specific daily annoyances this audience has; rank by (pain × reachability × ability for me to build under $200); recommend one."
- "Given skills A + B + C, give five service/product packages with realistic prices someone in [audience] would actually pay."
- "Take [industry]. What would an iPhone-style subtraction look like — what do we delete and what's left?"
- "What changed in the last 24 months that makes [old unsolved thing] newly possible or newly necessary?"

---

## Quality bar (self-check before you present)
- Could I say what each idea *precisely does* in one sentence, with no category words ("platform", "AI-powered", "marketplace for X")?
- Is there a named customer and a place to find ten of them?
- Does each have a reason it's *now*?
- Is at least one idea slightly uncomfortable — weird, hard, boring, or off-trend — in the way real opportunities often are?
- Are these ideas for **this** founder (and this repo), or could they be pasted onto anyone?
- If I used the YC RFS: did I fetch it live, bend the entries toward this founder, and avoid presenting "YC wants it" as proof of demand?
- Have I avoided: AI-because-it's-cool, tar pits, copycat of last year's hot thing, "Uber for X", an app to coordinate plans with friends?

## Anti-patterns
Starting from a technology and hunting for a problem · brainstorming from a blank sheet (tends to produce tar pits) · over-abstract problems (global poverty) · optimizing for impressiveness · picking an area you dislike because it raises money · waiting for the perfect idea · "I want to be the richest person in the world" as the goal · twenty ideas with no recommendation.
