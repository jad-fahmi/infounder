# boost — high-leverage features & mechanics

Goal: recommend the **few** features and mechanics that move activation, retention, referral or revenue — each with its cheapest possible build — and the list of things to cut. Fewer, better, faster.

---

## The ranking rule

Score every candidate on **leverage ÷ effort** where leverage = how strongly it moves one of: *activation → retention → referral → revenue*. Then force the **90/10 pass**: "How can we get 90% of the benefit for 10% of the work?" (Paul Buchheit's question — founders hate hearing it; it's usually right.) And the **main-result pass**: "Does this help the customer reach the main result?" If not, it goes on the cut list.

Prefer **one sure bet on the highest-leverage thing** over many small bets ("death by 1,000 paper cuts"). Pick it, let it run, and resist launching a second fix at day 30 out of impatience. Aim for **orders of magnitude, not increments** (not "+2% close rate").

Let early adopters steer: a Tesla Roadster buyer wanted acceleration and tech over comfort, and that tilt shaped the whole lineage. Your first users choose which features matter; don't design the final form in a vacuum.

---

## Mechanic families (pick by the metric you need)

### 1. Activation — shorten the path to the aha
- Define **one activation metric** (specific number + window). Design the first-run to hit it. (e.g. "N friends in M days" — widely cited for Facebook; exact figures vary by source.)
- One easy win **before** the ask (sign-up/pay): show the product working.
- Pre-populated example data; opinionated defaults; no empty states.
- Progressive disclosure: introduce a feature only when the next step of value requires it.
- Remove steps and fields. Defer account creation.
- **Demo-first / fake door:** a mock or video that sells before the product exists (Dropbox's three-minute demo). Test demand with a landing page + price + "buy" button.

### 2. Retention — reasons to come back
- Make **input → output** visible: "every thousand problems solved ≈ +20 points" turns a vague effort into a measurable path.
- **Accountability with skin in the game:** "If you don't do your homework, I'll bill you." Prepay > transactional.
- Accumulating value (data, history, progress, community) that would be lost by leaving.
- Re-engagement tied to the user's goal, not your metrics. Reduce, don't add: if the #1 churn reason is overwhelm, *cut* cadence and features (fewer calls, quarterly rather than monthly content dumps).
- Reliability as retention for critical products — "people think email is important and it's got to always work."
- Founder-care: fast personal replies; a bug apology that makes the customer like you more than before (Stripe DMing about an overcharge).

### 3. Referral & virality — turn happy customers into the channel
Telling people → people telling people. Build the whole chain (Hormozi's partner machine):
1. **The offer** (why should they bother?) — rewards that are *worth it*, preferably non-cash; **two tiers**: scarce/unscalable for the "killers", an accessible long-tail reward for everyone; "approximations" of the scarce prize (recording, raffle entries) so lower tiers feel in the game; the reward should **benefit the referrer's audience** so they don't burn goodwill hard-closing.
2. **The place:** a page that sells people on *why to refer*, states the prizes, the exact steps, how you'll help.
3. **Promotion:** email your list twice only; re-activate last cycle's referrers first; a button on the thank-you page ("send anyone else? get more free prizes").
4. **Instant personal link** — the fast reward; they must *believe attribution works*.
5. **Real-time leaderboard** — proof of attribution + competition; send it often (people check it daily).
6. **Collateral:** plug-and-play posts, emails, ads, scripts; plus a feed of **winners** (what's converting) so partners double down.
7. **Regular comms** (behind-the-scenes data doubles as free marketing education) and **human follow-up** for the top 50–100.
8. **Compliance:** don't lie or exaggerate; write the collateral yourself.
- **Friction rule:** "As soon as there's friction, they'll stop." Set the minimum activation threshold *inversely* to friction (an in-person intro ≈ 2; a text ≈ 4–5; a bare opt-in ≈ 10+).
- Honest caveat: Gmail's invite system came from running out of server space, not growth genius. Constraint-born mechanics can still work — just don't mistake them for strategy.

### 4. Scarcity, identity & community
- **Limited editions / drops / colorways** put demand on display (queues, fights, resale = proof).
- **Community badge value:** people don't buy the object, they buy "the community of everyone holding one." Give them something to brag about and a reason to post.
- **Shareable proof moments:** a user-generated "it survived a car fire" moment became the campaign. Watch for such moments in your own users; amplify the real ones.
- **Peer engine, not a megaphone:** invite people to co-author the narrative; partner with creators who reinterpret the product in their own cultural frame. Brands are *stewarded*, not owned.
- **Launch segment by segment:** Facebook launched school by school (separate stacks), creating dense local networks.
- Patience compounds: brand affinity built slowly is hard to copy.

### 5. Hooks — the entry point into attention
(Copy-level mechanics; also see `spark.md`.)
- **Proof–Promise–Plan** (+ picture + pain) in the first ~30 seconds.
- **Specific pain call-out** ("stop thighs chafing in the sun").
- **A named unique mechanism** (checklist or sequence).
- **One compelling point** instead of four.
- **Story tests:** A/B test names, covers, subheads on a small audience before committing ($100M "Leads" beat "Promotions" and "Advertising" every time).
- **Entertainers hold attention; educators change behavior.** Pick which job the content has.
- Polarize on purpose: to reach your 20%, be willing to annoy the 80%. Never dilute yourself.

### 6. Give-first artifacts (sales mechanics)
Do ~20 minutes of work before asking for 30 minutes: a security scan of their public site, a walkthrough of their app with specific suggestions, a short compliance audit note, free whiteboarding on their architecture. A free session as "half assessment, half pitch": show one easy win, then "this is how I teach — do you like that?"

### 7. Pricing-as-feature
- A real **upgrade constraint** people want to lift.
- Packages/tiers on the landing page from day one.
- Prepay; annual; usage limits that match value.
- Charging as a product signal: B2B buyers read "free" as "will they support us?"

### 8. Speed & care as features
- **Speed-to-lead:** respond to new leads in 60 seconds (one $60k hire whose only job was calling new leads immediately → 55% conversion for a restoration company).
- Founders answering support personally. "Would I reply to my own email?"
- Do things big companies can't: DM the customer; fix their problem personally; show up.

---

## The 90/10 library (dirty-but-works moves)

When a feature feels hard, look for the cheap substitute:

| Hard thing | Dirty 90/10 version |
|---|---|
| Real-time compute (e.g. 2nd-degree connections) | A label ("in your friends list" vs "extended network") |
| Spike handling you can't test | A button that serves any page as a static cached version; pre-warm capacity based on how many are waiting |
| Global database / scale | Per-segment instances (one stack per school/region); build the global one years later |
| Translation into 40 languages | Serve English strings to non-English visitors with "volunteer to translate this?"; accept when three submissions match |
| Music-specific tooling | Hack existing video tooling: every track is a video with an empty video track |
| Partner won't cooperate | Block-page explaining why you can't serve their users, with a phone number to complain |
| Build all of email | Start by reading *your own* email in the new UI; add each feature when you need it |
| Expensive vendor (lawyer, PR, designer) | Do it yourself first; get a spec and quote; payment plans |
| A feature everyone asks for | Test it as a fake door or a manual service first |

Design principle: **the best product decisions are made fast and under duress** — "8pm, the site's down" produces clarity. Give yourself that constraint on purpose (a 12-week deadline; "a plan and not enough time").

---

## The one-thing method (focus)

- *The catch exercise:* throw four balls and the person drops them; throw one and they catch it. Pick the single most compelling promise/feature, state it compellingly, and let it determine the marketing message, product strategy and delivery.
- *The "what must be true in 12 months" test:* name the one thing that, if true, makes objectives 2–5 shrink or vanish (own a lead channel; a supply of technicians; cash collection cut from 90 → 30 days).
- *Convexity:* returns concentrate at the 95th–99th percentile; you can't get there spread thin. "Perfect every detail and limit the number of details."
- *Subtract first:* ask "what can I delete and still be valuable?" before "what can I add?"

---

## Output format

```
## 3 bets
### 1. <Mechanic> — moves <activation|retention|referral|revenue>
**Why it works:** <principle + evidence>
**90/10 build:** <the cheapest version, concretely — screens/files/steps>
**Metric & target:** <what moves, by how much, in what window>
**Risk / what would make us wrong:** …
### 2. …
### 3. …

## Cut list
- <thing> — doesn't serve <main result>

## Do first
<one thing, why first, what to ship by when>
```

## Anti-patterns
Listing 20 features · adding without cutting · building for scale before pull · "viral" without friction analysis · features justified by "competitors have it" · polishing a screen nobody reaches · launching a second fix to the same problem before the first has had time · hiring/contracting to ship more features before knowing the product is wanted.
