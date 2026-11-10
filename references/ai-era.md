# ai-era — defensibility, engagement, findability and safety when building is cheap

Load this when: the user fears a model/lab will ship their feature; asks about moats, "AI wrapper" risk, community or data strategy; wants retention/engagement automation; is launching a website; or has a (vibe-coded) app with endpoints that cost money per request. Also load from `audit` when reviewing a repo with AI/LLM calls, email/SMS sending, uploads, or public APIs.

Provenance: section 1-4 distill field notes from creator content (Instagram reels) plus the Y Combinator / Hormozi / Altman material. They are **directional claims, not laws**; examples (Strava, Apollo, Duolingo) are illustrative and unverified here. Where the claim is strong, the underlying logic is old: features are copyable, moats aren't (Buffett/Munger), and distribution beats product (Hormozi).

---

## 1. The shift: features commoditize, moats don't

- General AI products ship new capabilities fast. Any product whose only value is "a feature on top of a model/API" can be absorbed by the next release, and "a vertical SaaS app" that is mostly UI around a prompt can become redundant in months.
- Software is cheaper to build than ever, so *building* is not the scarce thing. The scarce things are **distribution, trust, data, community, and being embedded in a customer's workflow**.
- The one-line version to give a founder: **"Build the product, but make community and data your moat."**
- Not "SaaS is dead": SaaS with a real moat (system of record, network effects, regulation, deep integration, proprietary data) is fine. It's *thin* SaaS that's exposed.

### The Lab Test (use in `roast` and `ask`)
1. If a lab shipped an equivalent feature tomorrow, what would customers lose by switching away from you? (If "nothing", you have a feature, not a company.)
2. Does your product get **better when models get better** (you're riding the wave), or does it exist only to patch today's model weaknesses (you're racing it, and will lose)?
3. What do you own that a lab can't copy by updating a model: relationships, data, a community, a regulatory permission, an installed workflow?
4. Can you survive on distribution alone if the product were copied tomorrow?
Any two "no"s → say so plainly and move the plan toward one of the moats below.

## 2. The moat menu (pick one to build on purpose)

| Moat | What it is | Illustration | Cheap first move | Test |
|---|---|---|---|---|
| **CaaS: community as a service** | People stay for *each other*, not the features | Strava (plenty of fitness apps; people use the one their friends and clubs are on); also brand communities (Stanley) | Seed a small group (20 users) with a shared goal and a reason to talk; host the thread, not just the tool | Do customers talk to each other unprompted? Would they stay if a rival copied every feature? |
| **DaaS: data as a service** | Proprietary data that compounds or that nobody else has; the software is the delivery vehicle | Apollo-style contact/company/insight databases: the value is the data, not the UI | Decide what data each customer interaction *adds* and make sure you keep rights to it (aggregated, consented) | Does each customer make the product better for the next? Can a lab scrape or buy this data? |
| **Distribution** | An audience, list, SEO footprint or partner channel you own | Creator-led businesses; affiliate/partner machines (`features-mechanics.md` §3) | Start an owned list and one content/partner channel from day 1 | Can you reach 1,000 buyers without paying a platform? |
| **Workflow / system of record** | You're where the work lives; switching is painful | Accounting, CRM, ops tooling | Integrate deeply with one tool your buyer already uses; store their history | What would a migration cost the customer? |
| **Trust, brand, regulation, capital** | Hard-to-fake permission or reputation | Licensed/regulated industries; outcome ownership ("be the insurer, not software for insurers") | Pick a niche where trust is the buying criterion | Would they pay you more than an equal product from a stranger? |
| **Speed + taste + founder proximity** | You ship faster and care more than a big team can | Founder-led support and iteration (`launch.md`) | Reply to every customer personally and ship weekly | Do customers name you, not the product, when recommending it? |

Rule: choose **one** moat to compound; name the cheapest 48-hour move toward it. Don't claim a moat you can't test.

## 3. The lifecycle engagement engine (the "ethical Duolingo")

**Idea (from the reels):** great consumer products feel obsessive because they work out *which message to send which person, when*. You can approximate this with behavioral analytics plus a language model: instrument everything → tag each person's activity by topic to build a per-user **interest map** → trigger the right nudge when someone is stuck or a community moment is missed.

**Concrete workflows**
- **Stuck-user rescue:** a user signs up, clicks around, never reaches the activation event → a workflow fires → an email or in-app message tailored to the topics they've shown interest in, aimed at getting them to the aha.
- **Community match:** a newcomer posts in your Discord/forum and gets no reply in X hours → a workflow finds the member whose interests best match the post → sends *that member* a short DM: "Could you answer this one?" Newcomers get replies; helpers feel useful.
- **Reactivation / progress:** quiet user + a topic they cared about → a relevant, single-purpose nudge, not a generic blast.

**How to build it, in the right order (don't skip steps)**
1. **Define the activation event** (the first moment of real value). Without it, nothing downstream means anything.
2. **Instrument** a small set of events first: signup, key page/feature views, activation, the few actions that predict return. A product-analytics tool (e.g. PostHog) can capture clicks, pageviews and custom events and trigger workflows.
3. **Detect "stuck"**: signed up N hours ago, no activation, or no reply to a post.
4. **Send one nudge, by hand first.** For the first ~50 users the founder writes the email or DM personally; that *is* the research (by-hand-first law). Automate only what already works.
5. **Measure against a holdout.** Compare nudged vs. not-nudged on activation and week-1 retention. If there's no lift, kill it.
6. **Then** add the AI layer: tag activity by topic, build interest maps, personalize. This is a multiplier on a loop that already works, not a substitute for one.

**Guardrails (non-negotiable, say these out loud)**
- **Ethical engagement:** the nudge must *help the person reach something they want*. No manufactured guilt, fake urgency, or notification spam. Add frequency caps and an easy unsubscribe. If you'd be embarrassed to explain the nudge to the user, don't send it. (See `product-audit.md` §I on dark patterns.)
- **Privacy:** collect only what you need; disclose it in your privacy policy; get consent where required (GDPR/ePrivacy, CCPA); don't pipe private message *content* into third-party tools or models without disclosure and a legal basis; prefer pseudonymous IDs and a retention limit. This is not legal advice; check the rules for your users' regions.
- **Anti-creep:** don't expose one user's data to another (the community match shares *a post*, not a profile).
- **Pre-PMF rule:** don't build this before you have users. With fewer than ~100 users, a founder with a spreadsheet and Gmail beats any workflow.

**Output when the user asks "how do I make people addicted/stick?"** → one activation event, one stuck-state, one nudge written out in full, one metric (activation within 24h), and the by-hand plan for the first 50.

## 4. Findability checklist (a website launch's plumbing)

This is one or two hours of setup, not a growth strategy. Do it once the site is live; don't make SEO your only channel pre-PMF (it's slow).

1. **Google Search Console:** verify the domain; check coverage/indexing; fix errors.
2. **XML sitemap:** generate (most frameworks/CMSs can) and **submit it** in Search Console; reference it in `robots.txt`.
3. **SEO basics:** a unique `<title>` and meta description for every page (title concise, roughly ≤60 characters; description a clear 1-2 sentences, roughly ≤155); one H1 per page; descriptive URLs; canonical tags; fast mobile load; internal links; real alt text; a page per thing people actually search for.
4. **GEO (generative-engine optimization):** make the site *citable* by AI answer engines. Clear, factual, self-contained answers near the top of key pages; an FAQ that mirrors real customer questions; structured data (schema.org: Organization, Product, FAQ, LocalBusiness as relevant); consistent brand name and facts everywhere; original data, quotes or numbers worth citing; mentions on credible third-party sites. Treat this as early and evolving: don't promise rankings in AI answers.
5. **Google Business Profile** (any business with a local or service-area presence): claim it; accurate name/address/phone/hours; correct categories; photos; ask happy customers for reviews; respond to reviews.
6. **Measure:** Search Console queries and clicks, plus one analytics tool; look monthly, not hourly.

## 5. Abuse & cost safety ("denial of wallet"): protect everything, not just login

**Why it matters (defensive framing).** Many fast-built apps secure the login page and then leave the rest wide open. Anything that costs you money or compute *per request* can be hit thousands of times by a script: an LLM chat, search, file upload/processing, image generation, email/SMS sending, signup and password-reset, contact forms, public/partner APIs, webhooks. A single unprotected expensive endpoint can run up a large provider bill, take the app down for real users and damage trust, all within hours. This is not "premature scaling": it's cheap insurance and the most common serious gap in vibe-coded products.

**The baseline (do all of these before you invite the public)**
1. **Rate limit everything**, not just auth: per user *and* per IP, with stricter limits on expensive routes and anonymous traffic.
2. **Usage quotas** tied to plan (daily/monthly caps on AI calls, uploads, emails). Free tier gets a small, hard cap.
3. **Request throttling / concurrency limits** and a queue for expensive jobs, so a burst can't fan out into unlimited provider calls.
4. **CAPTCHA or bot checks** (e.g. a privacy-friendly challenge) on anonymous forms and signup.
5. **Cost controls at the provider**: hard spending limits and budget alerts on every metered service (model APIs, cloud, email/SMS, storage). A dashboard alert is not a cap; set a real cap and an alert.
6. **Bound each request:** max input size, file type and size limits, timeouts, max output tokens on model calls, bounded retries.
7. **Require auth for expensive endpoints**; never put provider API keys in client code; keep secrets in environment variables.
8. **Database access rules:** enable and test access policies (e.g. row-level security) so users can only read/write their own data.
9. **Monitor and alert** on request spikes, error rates and spend; have a **kill switch** (feature flag) for the costliest feature.
10. **Idempotency / dedupe** for sends and payments so retries and floods don't double-charge or double-send.

**How to audit a repo (use in `audit`)**
- Grep for endpoints/handlers that call a model provider, email/SMS, storage, or payment API (`openai`, `anthropic`, `generate`, `sendgrid`, `twilio`, `resend`, `stripe`, `fetch(`/`axios` to third parties, `upload`) and check whether each is wrapped by a limiter/guard (`rateLimit`, `ratelimit`, `throttle`, `limiter`, `quota`, `captcha`, `turnstile`, `budget`).
- Check middleware order: is the limiter applied *before* the expensive call and to unauthenticated routes?
- Look for client-side secrets, `NEXT_PUBLIC_`-style leakage of private keys, and wildcard CORS.
- Report as a **Debt/risk, possibly Blocker** finding with `file:line`, and the smallest fix (a shared limiter middleware + a provider spend cap) rather than a rewrite.

**Test it:** from one IP, call the costliest endpoint ~1,000 times in a minute. Pass = throttled within seconds, alert fires, provider cap holds, normal users unaffected.

## 6. How the AI era changes the other modes (quick map)
- `spark`: prefer ideas where you own a community, data or distribution; sit at the edge of what models barely do today; sell the outcome, own the stack.
- `roast`: add the Lab Test and the moat check to the verdict; "AI wrapper with no moat" is a legitimate kill-shot.
- `audit`: instrumentation → lifecycle engine (§3); abuse/cost safety (§5); findability (§4).
- `boost`: community mechanics and lifecycle nudges are first-class bets.
- `launch`: findability plumbing (§4) plus the by-hand playbook; solo founders can now reach revenue with tiny teams, so don't assume you need to raise.
- `money`: model costs are COGS; price so heavy users can't make a plan unprofitable (quotas = pricing).
- `plan`: abuse/cost safety is *not* premature scaling; scalable infra still is.
