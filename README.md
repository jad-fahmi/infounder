# infounder

An AI co-founder and advisor for Claude Code. It brings a bet instead of a questionnaire, reasons the way great founders decide, shows you where they'd disagree, makes the call, and tells you the cheapest way to test it against real users and real money.

**Stance: idea first, research later.** No TAM slides. Lead with a concrete bet, then test it by selling, shipping and talking to people who have the problem.

What sets it apart:
- **A council, not a framework.** Ask it anything you're in doubt about and it seats three or four advisors (Altman, Graham, Seibel, Zuckerberg, Bezos, Jobs, Musk, Hormozi, and more), shows each one's instinct applied to *your* situation, names the real disagreement, then rules. Built for the founder you are now and the one you'll become.
- **Reads your repo.** A roast or audit is about the app you actually built, not the one in your pitch. It separates built, claimed and planned. It also checks cost-abuse exposure: are your expensive endpoints protected, or only your login?
- **Evidence ladder.** Opinions < compliments < usage < pre-orders < money < repeat/referral.
- **Always ends with a test.** Every answer includes a time-boxed experiment with a numeric pass/fail, plus the next 48 hours.
- **AI-era aware.** Moat thinking (community, data, distribution), the "will a lab ship my feature?" test, lifecycle engagement, findability (SEO + GEO), and abuse/cost safety.

## Modes

```
/infounder [mode] <anything>
```

| Mode | Use it for |
|---|---|
| `ask` | Any doubt or decision. "Should I raise?", "what would Zuckerberg do?", "I can't choose" |
| `spark` | Ideas: a step-one idea, a sharp wedge, and a swing; plus 17 ways to enter a "taken" space |
| `roast` | Verdict + kill-shot + fix + cheapest test for an idea or plan |
| `audit` | Product/UX/onboarding/abuse-safety review from your code, ranked fixes, delete list |
| `boost` | Which features and mechanics to build next (including community and lifecycle) |
| `money` | Offer, pricing, unit economics, funding path |
| `launch` | First 10 customers, scripts, findability checklist, a 14-day pass/fail |
| `plan` | Roadmap, hiring and spend check |
| `coach` | Commit / pivot / focus calls |
| `brief` | No arguments inside a repo: a co-founder check-in |

No mode word and a question that sounds like a doubt? It runs `ask`.

## Install

Copy the files into your Claude Code folders:

```bash
git clone https://github.com/jad-fahmi/infounder.git
mkdir -p ~/.claude/skills/infounder ~/.claude/commands
cp -r infounder/SKILL.md infounder/references ~/.claude/skills/infounder/
cp infounder/commands/infounder.md ~/.claude/commands/
```

On Windows PowerShell, use `$HOME\.claude\skills\infounder` and `$HOME\.claude\commands` with `Copy-Item -Recurse`.

Then run `/infounder` in any project.

## Examples

```
/infounder ask a bigger AI lab just shipped a feature like mine. Do I pivot?
```

Expected shape (illustrative, not a recorded run):

```
My call: Don't pivot. Move the moat. Your value today is a prompt on top of a model; a lab can ship that in an update.
The table:
- Altman lens: ride the wave, don't race it. Build what gets better when models get better.
- Buffett/Munger lens: a feature isn't a moat; what does a customer lose by leaving?
- Seibel lens (dissent): if people pay you today, keep selling while you build the moat.
Where they disagree: speed of pivot vs. keep selling. Ruling: keep selling this month, build one moat in parallel.
Test it: the Lab Test. Pass = customers can name something they'd lose if you vanished.
Next 48 hours: ...
```

```
/infounder roast a Chrome extension that summarizes Slack threads for managers
```

## Layout

```
SKILL.md              the skill: laws, modes, output rules
commands/infounder.md the /infounder slash command
references/
  council.md          the seats: how great founders decide, plus the protocol
  dilemmas.md         30 "when in doubt" default calls with dissent and tests
  ai-era.md           moats, lifecycle engagement, findability, abuse/cost safety
  (one playbook per mode) + principles + question bank
```

## Coverage and roadmap

Stage coverage today: **strong** from idea to first revenue, **solid** from first revenue to product-market fit, **lighter** for scaling an established company (control and delegation, hiring A players, the $1-3M "swamp", funding mechanics are covered; executive-team design, board management, pricing power, international or product-line expansion, M&A and CEO evolution are not). The council's seats (Bezos, Chesky, Buffett/Munger, Collison, Hormozi) still give useful lens-based reasoning at later stages, labeled as general public-record reasoning rather than source-backed playbook.

## Credits and disclaimer

Inspired by public talks and writing from Y Combinator partners, Alex Hormozi, Ash Maurya (Lean Canvas) and Sam Altman, plus public record on founders and operators including Mark Zuckerberg, Jeff Bezos, Steve Jobs, Elon Musk, Paul Graham, Peter Thiel, Warren Buffett and Charlie Munger, Brian Chesky, Patrick and John Collison, and Terence Reilly, plus well-known startup case studies and a few creator field notes. **The council uses lenses on public decision patterns, never quotes, and none of these people has endorsed or is affiliated with this project.** The text is paraphrased and unofficial. Anecdotes and figures are illustrative and unverified; check anything before you rely on it. This is a thinking aid, not financial, legal, security or investment advice.

## License

MIT. See [LICENSE](LICENSE).
