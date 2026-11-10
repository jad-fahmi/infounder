# roast — critique an idea, pitch or plan

A roast is a **precision strike with a repair kit**: find the most likely way this dies, say it plainly (and with some wit), credit what's real, then hand back a sharper version and a cheap test. Roast the idea, never the person. A roast with no fix is just an insult.

Intensity: `gentle` (lead with strengths), `straight` (default), `brutal` (no cushioning, still no cruelty).

---

## The shape of a roast

1. **Restate it in one precise sentence.** *Who* does *what*, *instead of what*, *for how much*. If you can't, say so — that's finding #1 ("what precisely does it do?" — the test that kills "AI trucking" / "Copilot for X" pitches where the founder replies "we'll talk to trucking companies and figure it out").
2. **Verdict** — one of:
   - `SHIP IT` — worth testing now.
   - `SHARPEN` — right problem, vague or bloated execution.
   - `MOVE THE WEDGE` — right space, wrong first customer / angle.
   - `KILL` — only for the right reasons (below). Say what to do instead.
3. **The kill-shot** — the single most likely reason it fails. Not a list of 12 worries; the one.
4. **The 3–5 lenses that matter for *this* idea** (pick from the list below — don't run all of them).
5. **What's genuinely good** — the steelman. If you can't find any, you didn't look.
6. **The fix** — a concrete, sharper version of the idea.
7. **Test it** — the cheapest real-world experiment, with a time-box and a numeric pass/fail ("10 people in a room, 3 pre-order at $X within 7 days").

Closing: **Next 48 hours** (1–3 actions; first = contact with reality) and ≤2 questions.

---

## The lenses

### A. The problem
- **Is it acute?** Good = the alternative to your solution is *nothing* (before Brex, startups literally couldn't get a corporate card). Bad = a nice-to-have. "Hair on fire" or "talked yourself into thinking there was?"
- **Is it real or made-up?** *Solution in search of a problem*: "AI is cool, what can I apply it to?" → you'll find a plausible, invented problem nobody cares about. Tell: you can state the problem in words, but users shrug.
- **Who has it, and how much do they pay today** to deal with it? (Maurya's questions: What's the real problem? Who's affected? How much do they currently pay? UVP? Unfair advantage? Repeatably scalable?)
- **Specific or abstract?** Too abstract (global poverty) can't be a starting point; need something a startup can tackle.
- **Specific pain copy test:** can you write the sentence that makes the reader think "I can't believe they know this about me"?

### B. The founder
- Founder-market fit — the single most important of the 10 questions; or the immersion plan to acquire it.
- Bringing vs. building expertise; does the plan match? (Overconfident novice with a 2-year build? Fearful expert chasing AI fashion?)
- Do they actually *want* this, or know people who do? If neither: "go talk to users."
- Would they work on it for years? (Passion follows traction — but they should be able to tolerate it.)
- Founder-dependence: does the model only work at the founder's level of skill (sales, delivery)? If so it's a job, not a business.
- Ambition mismatch: a "step two" idea (lab, hard tech, $100M raise) from someone with no step-one assets.
- Commitment: is this founder juggling several businesses? "Any can work, none will, unless you pick one."

### C. Why now / originality / crowdedness
- What changed (newly possible/necessary)? If nothing — why hasn't this been done?
- **Tar pit check** — a common, easy-looking idea many founders hit and nobody has solved. Not impossible, just harder than it seems; need a new insight. Google it, find who tried, find the hard part.
- **Copycat check** — 1,000 social networks after Facebook, 1,000 photo apps after Instagram. First mover usually wins; clones don't.
- **Competition** is normal and good. If entrenched, what is the *new insight*? What did all of them miss, or all of them do badly? If there is *none*, find out why (maybe nobody wants it).
- **Proxy** — a similar company elsewhere proving the model?
- **Positioning check: YC directory (optional, live).** When the idea has a clear category and the verdict hinges on "who else is here and how is mine different?", look at who YC funded there and how they describe themselves. Don't run it for every roast, only when it would change the advice.
  - *How (use in this order):* (1) `WebSearch` scoped to `site:ycombinator.com/companies <generic category terms>`, which is the most reliable; (2) `WebFetch https://www.ycombinator.com/companies/industry/<Industry>` (e.g. `Legal`), which renders real listings with one-liners and batches; (3) `WebFetch https://www.ycombinator.com/companies/<slug>` for the 3–5 closest companies. **Don't fetch `/companies` itself or its `?filter=` URLs:** they return an empty JS shell.
  - *Output:* 3–5 closest companies, each with the one-liner quoted, the customer it targets, and the batch. Then state the gap: what they all pitch, what none of them cover, and whether the user's wedge sits in that gap. Name it: "These three all sell X to Y. You'd be Z."
  - *Read it right:* a crowded cluster means tar pit unless the user has a real new insight. It does **not** mean the idea is validated. An empty cluster is **not** proof of opportunity either (maybe nobody wants it, maybe it's too new to be listed). The directory shows survivors only, never the many that failed, so say that. Funded does not mean working. Positioning is for finding the gap, not for copying.
  - *Privacy:* search with generic category terms only. Never put the user's project name, repo details or secrets in a query or URL.
  - *Verify before citing:* quote only what the page showed. If a fetch or search fails, say "check whether…" rather than guessing competitors.

### D. The reach — can they actually get customers?
- Who is customer one, by name or by room? Where does the buyer spend time (trade shows, job sites, Reddit, phone, WhatsApp)? Is the plan "build it and they will come" with a self-serve funnel + hope?
- **Wrong first customer:** selling enterprise-only products (useful at 500 engineers) to startups at $100/month; "willing to talk" mistaken for "easy to sell". Right-first-customer games: *Stripe* (customers when they're two people and stay through IPO), *Gusto* (startups as a proving ground, then the broader SMB market), *AWS* (bottoms-up through engineers who carry it into big companies — still needed real enterprise sales).
- **Churn-by-scaling:** does the category scale with *people* (HR, CRM, Heroku → customers rip it out as they grow) or with *revenue/activity* (payments → stays)?
- **Buyer changes:** early buyer is a founder; later a team with different needs → you'd need a new product.
- **Is there an early adopter who will pay now?** Most people aren't early adopters — finding them is a search problem, not a persuasion problem.

### E. Will they pay? (the business model)
- Who pays, what for, how much, how soon is the first dollar?
- Is it a **services business in disguise** (agency, dev shop, anything needing skilled human labor per customer)? Fine as a first dollar; not a "scalable software" story.
- Freemium with no upgrade constraint and no conversion tracking? "Freemium is a marketing tactic, not a business model" at launch.
- LTV and CAC: compute, don't opine.
- Cost-inelastic buyer / mandated spend / other people's money? (strong) vs. a consumer with a tiny total software budget (weak, esp. with AI inference costs).

### F. The ceiling & the vehicle
- **Maxed-out test:** "What does it look like at its best — does anyone get rich from it? How many service-based gym owners are worth a billion?" If nobody has maxed it, maybe you'll be the exception; but there may be a better vehicle.
- **Idiot Index placement** (see `monetization.md`): labor-heavy commodity (avoid) · easy/low-money (starter cash) · expert-dependent (a good job, not an asset; survivorship bias — "how many Joe Rogans?") · moat-built hard/high-money · demand/supply-arbitrage easy/high-money.
- **Moat:** deep skill, network effects, compounding time, regulatory, capital. "If everyone can do it, everyone will do it." AI is eroding some SaaS moats.
- **Income vs. asset:** will it be transferable if the founder leaves?
- Match to the founder's goal (income / cash flow / enterprise value / billions).

### G. Capital & funding fit
- Does the idea need millions upfront to break even? Can the founder credibly explain a path to 100x+? If neither: don't take VC money (or build for it). "You can't take $5M from a fund built for outlier returns and then decide to run a profitable business at your own pace."
- Is a profitable small software business a win for this founder? (Often yes: a product earning $30–50k/month with ~10 hours/month of upkeep "won".)
- Don't ask "is it venture-scale?" at idea stage — save that for after traction.

### H. Distribution loop & retention
- Does it have a **happy-customer loop**: activation (aha fast) → retention → referral? Acquisition obsession without that loop is a leak.
- Is there a reason for people to tell friends (identity, status, utility, incentive + low friction)?

### I. Branding / perception (light)
- A brand is a *result* — a customer's gut feeling — not a logo or a checklist. What gut feeling will the product create, and what behaviors/products/messages create it?

---

## Kill for the right reasons

- Solution in search of a problem.
- A tar pit with no new insight.
- No acute pain / nobody pays today / "nice to have".
- Can't reach the buyer, or the first customer is the wrong game.
- Customers outgrow it, or the buyer changes and you'd need a new product.
- Services business pretending to be software (when the stated goal is software scale).
- A capped or labor-heavy-commodity vehicle for the stated goal.
- Founder-dependent model.
- Capital need far beyond the founder's means with no credible raise.
- Precise-spec failure: they can't say what it does.
- The only evidence is fake traction.

## Do NOT kill for

- Small initial market ("markets can grow, or you can move to an adjacent one"; companies at $20–40M revenue never lack growth ideas).
- Boring (boring has a higher hit rate than "fun": payroll → Gusto; fun restaurant-finder apps are graveyards).
- Hard to start (schlep blindness: Stripe's $100B opportunity was left because it needed a bank deal and card-network mastery).
- Existing competitors (Dropbox was ~20th).
- Off-trend / bad model / bad space ("every successful YC story: everyone thought the idea sucked").
- Sounds dumb at dinner (Airbnb, Coinbase).
- "Not venture scale" at idea stage.
- Founder lacks a decade of experience (depth is learnable fast).
- Because it differs from what influencers say. If your idea-filter equals everyone else's, you all screen out the same ideas.

---

## Fast scorecard (optional; rate each red / yellow / green)

`Pain` acute? · `Reach` can I find 10 buyers this month? · `Pay` is there a price and a payer? · `Fit` am I the right team (or do I have the immersion plan)? · `Now` why this moment? · `Ceiling` does the vehicle match the goal? · `Spec` can it be said in one sentence?
Two or more reds on Pain / Reach / Pay → don't build yet; test first. (This scoring rule is infounder's own synthesis, not a source claim.)

## Roast skeleton

```
**Your idea, in one sentence:** …
**Verdict:** SHARPEN — <one line>
**Kill-shot:** <the single most likely reason it fails>
**Lenses that matter here:**
- <lens>: <finding with a concrete example/number>
- …
**What's actually good:** …
**The fix:** <sharper version — who/what/instead of what/price>
**Test it:** <experiment · time-box · pass if X, kill if Y>
**Next 48 hours:** 1) … 2) …
**Two questions:** …
```

## Roasting a pitch deck / landing page / plan

- **Pitch/landing page:** can a stranger say what it does in 5 seconds? One compelling point, or four balls thrown? Proof (not claims)? Specific pain? A named mechanism? Price visible? One clear CTA?
- **Investor deck:** Does it lead with TAM and an exit slide while traction is zero? Delete the exit slide. Does it have customers, retention, a believable next milestone? For stage-appropriate proof: pre-seed = who you are and what you'll build; seed = working product + early users; Series A = revenue, growth, spend plan; Series B = the number on the dashboard.
- **Plan/roadmap:** run `plan-check.md`.
