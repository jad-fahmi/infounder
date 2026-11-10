# plan — review a roadmap, hiring plan, budget, or "should I build/hire/raise X now?"

Goal: stop premature scaling. Most startups are pre-product-market-fit, but almost all online advice is written for post-PMF companies — "if you apply it pre-PMF you might accelerate your death." Your job is to walk their plan, strike what doesn't belong yet, defend the few things that do, and put the rest in order.

---

## 1. The master switch: pre- or post-PMF?

Ask (or infer): **What's your growth rate? How much runway do you have? Are customers trying to rip the product out of your hands?** If you can't confidently say you're post-PMF, you aren't. Don't hire to find out — figure it out first.

| | Pre-PMF | Post-PMF |
|---|---|---|
| Hiring | Almost never. Founders do it. | "Go crazy" — with the earn-the-right test |
| Spending | Don't spend money on anything you haven't done yourself | Ads, events, PR, tools — still mostly a waste, but now affordable |
| Engineering | Hacks, monolith, static fallbacks; turn the water on | Build the scalable thing now that demand is real |
| Sales | Founder sells; first 10 customers are the founder's job | Hire a sales leader appropriate to your stage |
| Ambition | One idea, one customer, one channel | 70/20/10 allocation, adjacent bets |

---

## 2. "Is that your job?" — the walk-through

Go down their list item by item. For each: *Is that your job right now? What fire exists today that this fixes — or is it a fire you predict?* A startup has one or two **six-alarm fires** and ~50 **smoldering fires**; founders hire to prevent a future one, one of the 50 eventually ignites, "but the other 49 didn't." Fight the fire after it's burning — startup life is reacting to what's broken, not predicting.

### Hiring lies founders tell themselves
- "If only we had more people we could ship more (features, an Android app, an iOS app, specialists per platform)."
- "Hiring gets us to profitability faster."
- Headcount as a KPI / marker of progress to impress investors, customers, friends.
- "They're available, and brilliant" (opportunism is for Google-sized companies).
- "We need an exec team" — cargo-culting the "About" page squares (COO, CMO…).
- "We'll need this person eventually, so hire now."
- "Hire a famous-resume VP of Sales" — a tenured VP is great at managing 100 reps, but not at making the first sales call or getting the first 10 customers. The early question is "what's the first experiment?" — a founder skill.

### Why not hiring pre-PMF
- **Turning the ship:** pre-PMF you must turn on a dime; every person adds coordination. "If it takes three months to turn the ship, you might just be dead."
- **A few very smart people beat many mediocre ones.** Every hire should raise the company's average.
- **Burn math:** "I've never had a company say 'I'm failing because we have so much money in the bank.'" Post-YC cash crises are almost always employee burn.
- **Toxicity risk:** if there's a 5–10% chance any hire turns toxic and you hire 25, that's "almost an equation for hating your life."
- **Managing drains many founders**; people problems are a top cause of burnout. Five people in a room is energizing.
- **Timing precedent:** Airbnb's first hire came roughly 18 months after launch (and took months to find); Stripe was ~3 people for the first year-plus. Hiring is back-loaded in top companies.
- **Specialists** save big — but only after the specific expensive problem exists (a network-ops hire taught free peering once bandwidth cost became the problem, not before anyone cared about the video).

---

## 3. The spend-audit checklist — "earn the right to spend"

**Rule:** find the cheapest, usually do-it-yourself, way to test a function; if it shows promise, you've *earned the right* to spend and scale it. If you haven't done it yourself, you're "in no way an authority to hire someone." The default response to "who's going to do X?" is **"you are."** (Everyone makes these mistakes the first time; the goal is to prevent about half.)

| Waste | Why | Instead |
|---|---|---|
| **Big-company star hire** (the mythical FAANG engineer — "Sebastianism": waiting for the rescuing king) | ~$1M/year package, and their productivity depended on big-company tools, workflows, support you don't have — "same cost, not the same productivity" | Hire for fit and speed; founders learn new skills |
| **Contractor armies** | A Band-Aid you never rip off; 5 contractors for 1 hire "doesn't go well"; "we'll bring it in-house" never happens | Hire one great person; keep contractors narrow and short |
| **Ads** | Platforms gladly take infinite dollars; you learn little; ads become a substitute for building | Small budgets to learn messaging only; find the owned growth loop early |
| **Events, sponsorships, brand advertising** | Hard to track; cargo-culting (Dreamforce-style); events don't create a brand, they leverage one | Scrappy stunts, quiet call rooms, flyers; micro-events |
| **PR agencies** | "I don't know anyone who's ever hired a PR agency that hasn't fired one"; juniors who Google you; ~$10k/month–$50k retainers; equity-for-PR is worse | Call journalists yourself; they want to meet founders building something good, without intermediaries |
| **Lawyers** | A junior associate at $500/hour customizing employment agreements = paying for their learning ("if you have to innovate on the employment contract, you probably don't have a company") | Standard documents; ask for a spec and quote up front ("if a lawyer can't say roughly what it costs, they haven't done it much"); big firms offer interest-free payment plans for spiky bills |
| **Advisors** | No one has ever said "that paid advisor made the difference" | Free advice from investors, domain experts, executives who volunteer; if someone demands equity for an advisory role, ask them to *invest* instead (most say yes); push professors' 20–40% asks down to ~1% |
| **Headcount to look big** | See hiring lies | — |

---

## 4. Premature scaling in engineering

- Don't test every pipe before you launch; **turn the water on**. "You earned the privilege to work on scalable things by making something people want first."
- A scale problem you don't have yet isn't a problem. Facebook ran separate PHP/MySQL/memcache stacks per school and delayed a global users table for years; Google built MapReduce only after a monolithic search product with users had a crisis; Twitch's first fix for traffic spikes was a static cached page.
- Don't hire platform specialists, or build for Android+iOS+web+API at once, before you know the product is wanted.
- Do protect the core path when reliability *is* the product.

---

## 5. Focus & sequencing

- **Pick one business.** Splitting attention is arrogance — the competitor who beats you is doing only that one thing. A portfolio is a result, not a method. Don't pull your best people off the core to build the new thing. Beware "woman in the red dress" side ventures.
- **Strategy = prioritization.** Unlimited opportunities, limited resources. Three buckets: (1) get more customers, (2) raise lifetime gross profit per customer, (3) reduce risk (insurance for the future — fund the "next platform" with 10–20% of profit).
- **The one thing true in 12 months** — define it; don't decide #2–5 until #1 is done, because the board will have changed.
- **Let the fires burn:** don't kick off a second fix at day 30; sure bets on the highest-leverage thing beat many small bets.
- **A plan and not enough time:** public goal + aggressive timeline (12 weeks) + frequent check-ins + remove people who don't need to be there.
- **Strike items from the roadmap** that fail: *Does this serve the main result? Does a real user ask for it? Is there a 90/10 version? Is it my job right now?*

---

## 6. When growth is real: control, delegation and the "swamp" (post-PMF)

- **Buy back your time.** Each hire gives up some control; every level is uncomfortable because "the thing you're holding on to is the thing you have to give up." Your time may be worth $100/h; the market pays $15/h for the thing you're doing.
- **The order in which control typically goes (revenue anchors are rough):** lower-skill support tasks (training the class) → admin/billing/collections → the money (give up control, not sight) → selling (founder can sell up to ~$1M/year; beyond that it gets hard) → managing a sales team (~$3–10M) → leadership/culture (~$10–30M; lead a small group who lead the rest).
- **Know where the bodies are buried.** If you can't name a department's problems — or you only hear good news — you're too far away. The cure is transparency, not taking control back. Keep accountability even as you give up control.
- **Time audit:** log every 15 minutes (5am–midnight) for a week with 1–2 words each; ask what 40% a role could handle and what 15% could be processized; build a role from tasks pushed down. Don't look for a unicorn.
- **The swamp (~$1–3M revenue):** at 20% margin a $1M business nets ~$200k and an A-player may cost most of it; choose between sacrificing profit for the hire or overworking ~6 more hours a day. Both hurt; the risk is hiring wrong. Founders get outsized returns by taking outsized risk.
- **Hiring when it's time:** Barrels vs. ammunition — throughput is limited by the few people who can own an outcome end-to-end; find barrels. Hire the smallest skill deficiency you can train (attitude for low-skill roles; irreplaceable experience for high-skill). The **3 D's** to train when you can't judge talent: *Document* the job as a checklist → *Demonstrate* it (you'll find you don't follow your own checklist) → *Duplicate* (they do it in front of you). The **barbell**: hungry learners at one end, secure love-the-work experts at the other; the middle (tit-for-tat) causes most failed hires. A players hire A players. Interview with the real problem and keep asking "what does that mean? how do you do that?" until you hit behaviors. Assume you're bad at hiring and decentralize the decision.
- **Culture** = the rules that govern reinforcement (what you reward/punish, including what you don't call out). Give feedback fast and as Stop/Start/Keep behaviors with conditions ("when X happens, do Y"). Criticism = discrepancy between actual and desired; insult = a label on the discrepancy ("lazy"). Have the hard conversation sooner.

---

## 7. Team: co-founders

- Prefer 2–3 founders; viable solo, but the psychological toll is underestimated even by tough people. List the $10B+ tech companies — almost none had a true solo founder.
- **Never add a co-founder because investors will like it** (ends in heartache 100% of the time). Better no co-founder than a bad one. Start without one, never stop looking.
- **Date before you marry:** experiment quickly with co-founders but hire/commit slowly — a weekend project or ~3-month side project to see conflict handling and aligned vision. ~80% of billion-dollar companies have 2+ founders (one source's figure).

---

## 8. Output format

```
## Verdict: <pre-PMF | post-PMF | unclear> — <one line>

## Plan review
| Item | Verdict | Why |
|---|---|---|
| Hire a head of marketing | CUT | Pre-PMF; founder should run the first 3 channel experiments |
| Add Android app | DEFER | No evidence of Android demand; ship web, fake-door the app |
| Rebuild on microservices | CUT | No users hitting limits |
| Wire up Stripe | KEEP | Revenue is the validation |
| … | | |

## Order of operations
1) … 2) … 3) …

## Earn-the-right triggers
We'll hire/spend on <X> when <measurable condition>.

## Next 48 hours
…
```

## Anti-patterns
Hiring to feel like progress · "pre-PMF" self-delusion · asking the board's advice from people with post-PMF experience · copying a famous company's org chart · paying for expertise you haven't tried to do · building the exec "About page" · making hiring the most important skill before you have anything to scale.
