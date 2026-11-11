# pmm-ai-workforce

Tried and tested product marketing skills for Claude.

Each skill is one job a product marketer does, written as a method Claude can follow. Give it real inputs and it gives you a working draft you can edit, not a blank page.

## The skills

| Skill | What it does |
|---|---|
| `icp-persona` | Builds an ICP and persona card from the evidence you have, and labels what is assumed. |
| `positioning-statement` | Writes a positioning statement: who it is for, the problem, the alternative, why you win. |
| `messaging-framework` | Turns positioning into a messaging house: core message, pillars, proof. |
| `teardown` | Reads a live homepage and tells you what it says, what it misses, and what to change. |
| `competitor-profile` | Profiles one competitor from public sources. |
| `battlecard` | Builds a one-page battlecard a sales rep can use on a call. |
| `gtm-plan` | Plans a launch: tier, audience, message, channels, assets, owners, one metric. |

Some skills use the output of another. Run them in this order:

- `icp-persona`, then `positioning-statement`, then `messaging-framework`, then `gtm-plan`.
- `competitor-profile`, then `battlecard`.
- `teardown` works on its own.

## Install

**Claude Code, as a plugin (easiest).** Type these two commands in Claude Code:

```
/plugin marketplace add omaird/pmm-ai-workforce
/plugin install pmm-ai-workforce@pmm-ai-workforce
```

To get updates later, run these in your terminal, then restart Claude Code:

```bash
claude plugin marketplace update pmm-ai-workforce
claude plugin update pmm-ai-workforce@pmm-ai-workforce
```

**Claude Code, by hand.** Copy the skill folders into your skills folder:

```bash
git clone https://github.com/omaird/pmm-ai-workforce.git
mkdir -p ~/.claude/skills
cp -r pmm-ai-workforce/skills/* ~/.claude/skills/
```

To use the skills in one project only, copy them into that project's `.claude/skills/` folder instead.

Then start a new session. Ask for the job in plain words, for example: "Build a positioning statement for our product."

**Claude apps:** zip one skill folder and upload it under Settings, Capabilities, Skills.

## How these are built

- Every skill asks for real input first. If the input is missing, it tells you what it needs instead of making things up.
- Every claim in an output should be something that could be proven wrong. Filler gets cut.
- Every skill ends with a quality bar: a pass-or-fail checklist for the output. Check the draft against it before you use it.

## Feedback

Found a problem, or have an idea for a skill? [Open an issue](https://github.com/omaird/pmm-ai-workforce/issues).

## License

MIT. See `LICENSE`.
