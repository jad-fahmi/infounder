# infounder

An AI co-founder for Claude Code. It brings a bet instead of a questionnaire, then tells you the cheapest way to test it against real users and real money.

**Stance: idea first, research later.** No TAM slides. Lead with a concrete bet, then test it by selling, shipping and talking to people who have the problem.

What sets it apart:
- **Reads your repo.** A roast or audit is about the app you actually built, not the one in your pitch. It separates built, claimed and planned.
- **Evidence ladder.** Opinions < compliments < usage < pre-orders < money < repeat/referral.
- **Always ends with a test.** Every answer includes a time-boxed experiment with a numeric pass/fail, plus the next 48 hours.

## Modes

```
/infounder [mode] <anything>
```

| Mode | Use it for |
|---|---|
| `spark` | Ideas: a step-one idea, a sharp wedge, and a swing |
| `roast` | Verdict + kill-shot + fix + cheapest test for an idea or plan |
| `audit` | Product/UX/onboarding review from your code, ranked fixes, delete list |
| `boost` | Which features and mechanics to build next |
| `money` | Offer, pricing, unit economics, funding path |
| `launch` | First 10 customers, scripts, a 14-day pass/fail |
| `plan` | Roadmap, hiring and spend check |
| `coach` | Commit / pivot / focus calls |
| `brief` | No arguments inside a repo: a co-founder check-in |

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

## Example

```
/infounder roast a Chrome extension that summarizes Slack threads for managers
```

Expected shape (illustrative, not a recorded run):

```
Verdict: SHARPEN. Kill-shot: managers don't feel this pain; the people drowning in threads are on-call engineers.
Fix: sell to support leads, one team, $49/mo.
Test it: DM 20 support leads; pass = 3 agree to a paid pilot in 7 days.
Next 48 hours: ...
```

## Layout

```
SKILL.md              the skill: laws, modes, output rules
commands/infounder.md the /infounder slash command
references/           one playbook per mode + principles + question bank
```

## Credits and disclaimer

Inspired by public talks and writing from Y Combinator partners, Alex Hormozi, Ash Maurya (Lean Canvas) and Sam Altman, plus well-known startup case studies. The text is paraphrased and unofficial. It is not affiliated with or endorsed by any of them. Anecdotes and figures are illustrative and unverified; check anything before you rely on it. This is a thinking aid, not financial, legal or investment advice.

## License

MIT. See [LICENSE](LICENSE).
