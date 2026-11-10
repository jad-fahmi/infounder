# audit — review the product as actually built

Codebase-aware product and UX review. Your job is to experience the product the way a stranger would — from the code, the copy and the flows — and tell the founder where the first five minutes break, what to delete, and what single metric matters.

**Rule:** review what is *built*, not what the README or pitch claims. Always separate **built / claimed / planned**, and cite `path:line`.

---

## 1. Scan protocol (read before opining)

Time-box the orientation to ~10–15 tool calls; go deeper only on the paths the audit needs.

1. **Identity:** README, docs, package.json / pyproject / Cargo / go.mod, app name & description, landing page copy.
2. **Surface area:** routes / pages / screens / CLI commands / API endpoints (`Glob` for `pages/`, `app/`, `routes/`, `src/screens`, `cmd/`). Count the top-level destinations a new user sees.
3. **First-run path:** signup/auth, onboarding, empty states, default data, first action. Grep for `onboarding`, `welcome`, `getting-started`, `signup`, `tour`, `empty`.
4. **Money path:** grep `stripe`, `paddle`, `lemonsqueezy`, `checkout`, `pricing`, `plan`, `subscription`, `paywall`, `trial`, `upgrade`, `limit`, `quota`.
5. **Growth path:** grep `invite`, `referral`, `share`, `link`, `copy link`, `leaderboard`, `affiliate`, `utm`.
6. **Instrumentation:** grep `analytics`, `posthog`, `mixpanel`, `amplitude`, `segment`, `track(`, `event`, `gtag`, `plausible`, `sentry`.
7. **Customer contact:** support / feedback / chat widgets, `mailto:`, intercom/crisp, "reply to this email", changelog.
8. **Velocity & focus:** `git log --oneline | head -30`, recent churn, TODO/FIXME clusters, size of dirs (what got the effort?).
9. **Over-engineering tells:** microservices/queues/k8s/IaC for a product with no users; elaborate auth/roles/admin panels; i18n before PMF; plugin architectures; abstractions with one implementation; custom everything.

Open the audit with: *"What this actually is: …"* (2–3 lines). Let the user correct you.

---

## 2. The audit checklist

### A. The core job & first impression (5-second test)
- Can a stranger say what it does and for whom from the landing page / first screen? (One compelling point, or a four-ball list?)
- Is the **main result** obvious — the single outcome the customer came for?
- Does every visible feature help the customer reach that result? Mark the ones that don't → **delete list**. ("Does every added feature help the customer reach the main result?")

### B. Time-to-aha (activation)
- Count the steps and form fields between landing and first real value. Each one is a leak.
- What is the **aha moment**, and is there a defined **activation metric**? (Facebook is often cited for "N friends in M days" — a specific number, a specific window, a design that pushes people to it.) Propose one.
- Can the user get a win **before** signing up / paying? One easy win up front.
- Is the first-run empty? Pre-populate with realistic example data; show the product working.
- Are you **introducing things only when needed** for the next step of value? Perfect the step most people find valuable first, *then* reveal the next. (Skool cut weekly calls, moved content drops from monthly to quarterly, and turned off app features at entry after finding the #1 cancel reason was overwhelm, not lack of value.)

### C. Overwhelm & focus
- Number of nav items, settings, toggles, modes, and CTAs at entry. People leave when there are too many things to do.
- "How much can I take away and still have it be good — probably better?"
- Is there one primary action per screen?

### D. Retention
- What brings people back? (New value arriving, accumulating data/progress, reminders tied to their goal, accountability, community.)
- Visible **input → output** link (problems solved → score; workouts → results) so users see progress.
- Does it still work for the user **when they've grown** (the churn-by-scaling check)?
- What's the real #1 reason people leave? (Look for cancellation flows, surveys; if none exist, *that's the finding*.) The fix is usually "way smaller and more nuanced" than "this doesn't work" — break the funnel into components instead of binary pass/fail: click-through, traffic quality, page conversion, step-2-of-4 drop, hook, offer clarity, ad-to-page congruence, core-problem fit.

### E. Referral & sharing (the happy-customer loop)
- Is there any path for a happy customer to tell a friend? How many taps? Is the message pre-written? Is there an incentive (ideally one that *benefits the friend*)?
- Are share prompts at the **moment of delight**, not buried in settings?
- Four Rs, in order: **Retain → Review → Refer → Resell.** Which is missing?

### F. Money
- Is there a price? Where is it shown? Can the customer pay in ≤3 clicks? Is money handled properly, or punted (awkwardness avoided by "making it free")? *Solve the money problem; don't dodge it.*
- Is there a real **upgrade constraint** (something people want to lift: seats, volume, storage, features) — and is free→paid conversion tracked?
- Free pilots with no commitment? Everything free forever?
- Pricing as a config value you can A/B, or hard-coded in ten places?

### G. Instrumentation & learning loop
- Are the **four numbers** tracked: activation rate, week-1 retention, paid conversion, referral rate? If not, instrumenting these is the first fix.
- Is there a way to run experiments on pricing, landing page, onboarding, features (flags, variants), or to ship daily?

### H. Founder ↔ customer channel
- Can a customer reach a human fast? Does the founder talk to users (reply-to address, in-app message, calls)? Early users stay because they trust the founder.
- Do the emails the product sends pass: *"If I received this, would I reply?"*
- Speed-to-lead: when a lead arrives, how long until a human responds? (Calling a new lead within 60 seconds converts ~4–5× better.)

### I. Honesty & hostility
- Dark patterns, confirmshaming, hidden cancel flows, fake scarcity, hostile support (design that assumes customers are bad). Big companies drift into this; startups should exploit being human instead.
- Does the product's **brand feel** match the intent? A brand is a gut feeling formed by product, UX, copy, behavior and support — audit the *felt* result, not the logo.

### J. Premature scaling & over-engineering (the "turn the water on" check)
- Infrastructure built for a scale that does not exist (queues, sharding, microservices, multi-region, a global users table).
- Features built for hypothetical segments; platforms supported before demand (Android/iOS/web all at once).
- Time spent on what the customer can't see.
- Ask for each: *what's the dirtiest version that gets 90% of the benefit for 10% of the work?* And: *has a real user hit this problem yet?* Scalable things are a privilege earned by making something people want first. (Facebook ran per-school stacks and delayed a global users table for years; Twitch's first fix for a traffic spike was a static cached page.)
- **Conversely:** protect the core path if the product is reliability-critical (email, payments, health data).

### K. Quality of the unglamorous basics
- Loading speed, error states, empty states, mobile, accessibility, copy typos. (Apply the `apple-design` / `unslop` skills if available and visual polish is the issue — infounder owns *product strategy*, not pixels.)

---

## 3. Output format

```
## What this actually is
<2–3 lines. Built vs claimed.>

## The first 5 minutes (where it breaks)
1. <finding> — `path:line` — why it costs users/revenue
2. …

## Top 5 fixes (ranked by leverage ÷ effort)
| # | Fix | Why it matters | 90/10 build | Effort | Metric |
|---|-----|----------------|-------------|--------|--------|

## Delete list
- <feature/screen/setting> — doesn't serve <main result>

## Instrument first
Activation = <definition>. Track: activation, week-1 retention, paid conversion, referral.

## The one metric to watch
<metric, target, how to read it>

## Do this week
1) … 2) …
```

## Severity rubric
- **Blocker:** a stranger can't get to value or can't pay.
- **Leak:** a step many drop at; unclear value; no return reason.
- **Missed lever:** no referral path, no upgrade constraint, no instrumentation, no founder contact.
- **Debt/risk:** over-engineering, hostile patterns, reliability gaps in the core path.
- **Polish:** do last. "Your goal right now isn't to get it perfect. Your goal is to just make it exist."

## Anti-patterns for the auditor
Recommending a rewrite when a deletion would do · listing 30 issues instead of ranking 5 · judging polish before activation · proposing features without an activation/retention/referral/revenue reason · treating every missing best-practice as equally important · opining on code you haven't read.
