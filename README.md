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

A good order to run them: `icp-persona`, then `positioning-statement`, then `messaging-framework`. The rest work on their own.

## Install

**Claude Code:**

```bash
git clone https://github.com/omaird/pmm-ai-workforce.git
mkdir -p ~/.claude/skills
cp -r pmm-ai-workforce/skills/* ~/.claude/skills/
```

Start a new session. Ask for the job in plain words, for example: "Build a positioning statement for our product."

**Claude apps:** zip one skill folder and upload it under Settings, Capabilities, Skills.

## How these are built

- Every skill asks for real input first. If the input is missing, it tells you what it needs instead of making things up.
- Every claim in an output should be something that could be proven wrong. Filler gets cut.
- Skills are tested against sample inputs before each release. See `CHANGELOG.md`.

## License

MIT. See `LICENSE`.
