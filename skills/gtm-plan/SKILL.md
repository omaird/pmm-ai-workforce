---
name: gtm-plan
description: Build the go-to-market plan for a launch, covering the tier ruling (T1, T2, or T3), audience, core message, channel sequence, asset list with owners, risks, a readiness gate, and ONE primary metric committed before launch day. Use when a launch date exists and someone needs the plan everything else hangs off, and after launch to run the retrospective against that metric.
---

# GTM plan

Produce the single document a launch runs from. It rules the launch tier, names the audience and the message, sequences the channels, lists the assets and who builds each one, and commits to ONE primary metric. One metric, not a dashboard, because a launch with five equally important numbers has no way to be called a success or a failure. Choosing the metric afterward is how launches get graded on whatever they happened to be good at, and that is the failure this plan exists to prevent.

## When to use

- A real launch exists, with a date, a scope, and a named owner.
- A launch needs its tier decided and its effort sized to match.
- A launch has shipped and needs a retrospective against the metric it committed to.

Do NOT use this skill with no launch in front of you. A GTM plan written without a real launch turns into a generic checklist.

## Required inputs

Refuse to run without the first three. Say which one is missing, who can supply it, and stop. Do not write a plan with placeholders where the inputs go.

1. **A real launch:** what is launching, the date, the scope, and the named owner.
2. **The current messaging** for the product being launched (a messaging framework, or at least a positioning statement). The plan does not invent a message.
3. **The ICP or persona** for the audience being launched to (see `icp-persona`).
4. **Competitive context** for anything the launch positions against (see `competitor-profile`), where relevant.
5. **Channel reality:** which channels actually exist and who can staff them. Ask the user. A plan that assumes a channel nobody runs is a wish.
6. **Pricing and packaging inputs**, where relevant. The plan can recommend how an offer is packaged at launch. Price itself is a business decision for the user; present options, do not set it.

## Method

1. **Rule the tier, and write down why.**
   - **T1:** a company-defining moment. New product, new category claim, major repositioning. Earns the full plan, a full launch brief, a full day-0 comms pack, and a hard readiness gate.
   - **T2:** a significant feature or expansion that changes what a buyer can do. Earns a shorter plan and a lighter comms pack.
   - **T3:** an incremental update. Earns a changelog entry and a note to sales, and nothing more.
   Write the reason for the ruling so it can be argued with later. Watch for tier inflation: if everything becomes T1, tiering stops carrying information. Applying T1 effort to a T3 launch is the most common way a small team burns itself out. If a stakeholder wants a different tier, state the reasoning and hand the decision to the user rather than negotiating it.
   The whole plan, from the title to the last line, fits the tier: T3 250 to 400 words, T2 600 to 1,000, T1 1,000 to 1,800. Table cells count. Rule the tier first, then size every section to it: one short line per row, one line per risk, and no sentence that repeats the inputs back. Keep every section; a T3 section is a line or two. Count before you finish. Over the top of the band is too long: cut it again. Under the floor is fine when every section is present; never pad to reach it. The retrospective file is not counted.

2. **Commit to ONE primary metric, before day 0.** One number the launch either hits or misses, with a target and a measurement window. Timestamp it in the plan. Secondary numbers may be tracked, but they are not the grade. Ask "what is the one number" first, then write the Primary metric line in one of three ways:
   - **Committed,** when someone commits to the number before day 0: `<metric, target, window>. Committed YYYY-MM-DD.`
   - **Committed on day 0,** when it is committed on day 0 itself: `<metric, target, window>. Committed YYYY-MM-DD, on day 0, not before it.` The Readiness gate gets an unchecked box: `- [ ] Primary metric committed before day 0`.
   - **Proposed,** when nobody can commit to one number in this session: propose one metric with a target and a window, and write `<metric, target, window>. PROPOSED by Claude on YYYY-MM-DD, not committed. Commit it before day 0.` The Readiness gate gets an unchecked box: `- [ ] Primary metric committed`. Never write "Committed" for a metric you picked.
   When the plan is done, write `**The call:**` under the header: one sentence, at most 20 words, naming the tier, the one metric and its target, and what must be true before day 0. If the metric is PROPOSED, The call says so. Count the words before you write it. Over 20 is too long: cut it again.

3. **Name the audience.** One primary audience, taken from the ICP or persona card. If the buyer and the signer are different people (common in technical and security sales, where practitioners choose and executives approve), name both and say which one the launch is written for.

4. **State the core message.** Lifted from the messaging framework, not rewritten. One sentence, plus the two or three proof points the launch will lean on. Mark any proof point that is not yet proven.

5. **Sequence the channels with dates.** Only channels that exist and have an owner. Pre-launch, day 0, and the follow-through window, each with dates.

6. **List the assets.** Each asset gets an owner and a due date. Size the list to the tier. A T3 asset list is two lines. Wherever you fill an owner the user did not give, label it "(proposed)" where it appears. Never present a pick as the user's choice.

7. **Name dependencies and risks.** What has to be true for the launch to go (product readiness, pricing decided, legal review, sales trained), and what could move the date.

8. **Set the readiness gate.** The checklist that has to be clear before anyone declares day 0. If items are open on the date, the choice is to clear them or move the date. Launching with items open is the user's call, made explicitly, not a default.

9. **Save the plan** as `YYYY-MM-DD-gtm-plan-<launch-slug>.md`. Have someone other than the author review it before the team works from it.

10. **After launch, run the retrospective** against the same primary metric, in a file saved next to the plan. Did it hit the number? Then convert each insight into a named action with a named owner and a date. A retro that produces observations and no owners has not done its job.

## Output format

```markdown
# GTM plan: <Launch>

**Launch date:** YYYY-MM-DD   **Owner:** <name>
**Tier:** T1 / T2 / T3
**Primary metric:** <metric, target, window>. <one of: "Committed YYYY-MM-DD." / "Committed YYYY-MM-DD, on day 0, not before it." / "PROPOSED by Claude on YYYY-MM-DD, not committed. Commit it before day 0.">

**The call:** <one sentence, at most 20 words: the tier, the one metric and its target, and what must be true before day 0>

## Tier ruling
<the tier and the reason>

## Audience
<primary audience; buyer vs signer if different>

## Core message
<one sentence, from the messaging framework>
**Proof points:** <each marked PROVEN with source, or UNPROVEN>

## Channel sequence
| Date | Channel | What goes out | Owner |
|---|---|---|---|

## Assets
| Asset | Owner | Due |
|---|---|---|

## Dependencies
## Risks
## Readiness gate
- [ ] <item that must be clear before day 0>

## What this plan did not settle
<open questions, with who decides>
```

Retrospective, saved as `YYYY-MM-DD-gtm-retro-<launch-slug>.md`:

```markdown
# Launch retrospective: <Launch>

**Primary metric:** <metric, target>. **Result:** <actual>. Hit / missed.

## What we learned
| Insight | Action | Owner | Due |
|---|---|---|---|
```

## Quality bar

- [ ] Exactly one primary metric, with a target and a window, written as one of the three lines in step 2: Committed, Committed on day 0, or PROPOSED. Never "Committed" for a metric Claude picked. A day-0 or PROPOSED metric has its unchecked box in the Readiness gate.
- [ ] `**The call:**` sits directly under the header block. It is one sentence of at most 20 words, in plain words, naming the tier, the one metric and its target, and what must be true before day 0. If the metric is PROPOSED, The call says so. Good: "T2 launch: 40 teams turn on rotas in 30 days; sales trained before day 0." Good: "If legal clears the claims before day 0, this T1 launch targets 500 paid accounts in 60 days." Do not copy the shape of these examples.
- [ ] Tier ruling stated with its reasoning. The whole plan, from the title to the last line, stays under the top of its tier's band: T3 400 words, T2 1,000, T1 1,800. Table cells count. The retrospective file is not counted.
- [ ] One primary audience named.
- [ ] Core message taken from existing messaging, not invented; unproven proof points marked.
- [ ] Every channel has an owner and dates. No channel nobody runs.
- [ ] Every asset has an owner and a due date. An owner the user did not name is marked "(proposed)".
- [ ] A readiness gate exists and is checkable.
- [ ] No price set in the plan; pricing is presented as options for the user to decide.
- [ ] "What this plan did not settle" is not empty.
- [ ] No em-dashes in your own prose. Em-dashes inside quoted material, such as the core message lifted from the messaging framework, are preserved exactly.
