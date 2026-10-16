---
name: positioning-statement
description: Produce a positioning statement and the reasoning that produced it, using the publicly published April Dunford method that walks competitive alternatives, unique attributes, the value those attributes enable, who cares a lot about that value, and the market category. Use when a new product or engagement needs its positioning decided, when an existing positioning is due for a refresh, when research contradicts the current positioning, or when downstream assets have started disagreeing about who the buyer is. Do not use it to build the messaging house or to settle a strategic point-of-view question.
---

# Positioning statement

This skill decides what the story is, in one place, so that a dozen assets stop quietly disagreeing about it.

## When to use

Fire this skill when:

- A new product, company, or engagement starts and nothing written down names the buyer or the alternative the story has to beat.
- An existing positioning is due for its periodic refresh (quarterly works well).
- Research contradicts the current positioning. Raise the contradiction with the user first, then run this to draft the replacement. Never rewrite positioning silently to match a new finding.
- Two downstream assets say different things about the target buyer, and nobody can point at the document that settles it.

Do not use it when:

- The positioning is already settled and what you need is pillars, proof, and boilerplate. Use `messaging-framework`.
- You need the buyer described in operational detail: committee, triggers, disqualifiers. Use `icp-persona`. This skill produces the "who cares a lot" input that `icp-persona` expands.
- You need site or landing copy. That work sits on top of a finished positioning.

## Required inputs

**This skill refuses to run on an imagined competitor set.** Competitive alternatives must come from what buyers actually do today, evidenced. A positioning built against a competitor chosen because it was convenient to beat is a document that wins an argument nobody is having. If you cannot evidence a single alternative, stop and say so.

Checklist:

1. **Product truth**: what the product does today, in the hands of a user, not on the roadmap. Source it: the live site, the product itself, a brief, or material the user provides. Without it: refuse.
2. **Evidence of what buyers do today**: sales notes, win-loss material, review-site language, a real conversation, the buyer's own words anywhere they exist. At least two alternatives must trace to something observed. Without it: refuse, and name what would close the gap.
3. **The current positioning**, if one exists, with its date. You are proposing a revision to a known thing, not writing over it.
4. **A human ingredient** when the subject is the user's own company or brand: an anecdote, a real number, or an opinion from the user. Brand-defining positioning does not get drafted from nothing. Ask for it if it is missing.
5. **Any open questions** the user has already logged about the positioning. These are the user's to answer. This skill does not settle them by writing past them.

**Second refusal.** This skill does not decide strategic point-of-view questions. Changing who the audience is, claiming a market category the brand has not claimed before, or adding or dropping an offer are all decisions for a human. Draft the options, state the tradeoff, and escalate to the user. A strategic change that ships quietly inside a positioning doc is the failure mode this refusal exists to prevent.

## Method

The five-part sequence in steps 2 through 6 follows the positioning method **April Dunford** publishes in her book *Obviously Awesome* and in her public talks. Credit her by name in the deliverable and cite a specific public source, a talk or the book, with a link where you have one. Use her method. Do not reproduce her text. Every word of the output is your own.

1. **Load the context in a fixed order.** Any existing brand point of view, then the current positioning, then any voice guidelines. For a client or product, add the brief and any input material the user supplied. Use web search and fetch to read the live site and the alternatives' public claims. Record every source with its date. Name the specific buyer seat (for example, in security: a detection engineer, an identity architect, a cloud security lead, a CISO). "Security buyer" is a category, not a reader.

2. **List the competitive alternatives: what the customer actually does today.** Not the vendor list from a category report. Include the two alternatives teams forget: doing nothing, and a person plus a spreadsheet. For each alternative write what the buyer gets from it, what it costs them, and where your evidence for it came from. Rank them. The top-ranked alternative is the one the positioning has to beat, and it gets named in the statement. An alternative with no evidence line is labeled ASSUMED and cannot be ranked first.

3. **Isolate the unique attributes.** What is true of this product that is not true of the top alternatives. Capabilities, facts, structural properties. The test is external verifiability: could someone outside the company confirm this by looking, trying, or reading. "Better UX" fails that test. "Deploys agentless in under an hour, documented step by step in public docs" passes it. Drop everything that fails.

4. **Translate each attribute into the value it enables.** One line per attribute, phrased as what the buyer gets, not what the product has. If an attribute produces no value a buyer would pay attention to, delete the attribute. It is trivia. If two attributes produce the same value, merge them, because the value is the unit that matters downstream.

5. **Identify who cares a lot about that value.** Not everyone who could use the product. The characteristics that make a buyer care disproportionately: their situation, their constraint, the thing that is currently on fire. Write these as characteristics, not as demographics, so `icp-persona` can turn them into a card. If the best-fit buyer turns out to differ from the current target, that is a strategic change, so flag it for the user rather than absorbing it.

6. **Name the market category the product should be understood in.** Category is the frame that tells a buyer what to compare this to and what to expect. Test the candidate: put the product in the category, then list what a buyer would then assume about price, buying process, and who signs. If those assumptions are wrong, the category is wrong, however flattering it sounds. Claiming a new category is a strategic decision and escalates.

7. **Run the proof status pass.** Split every claim in the draft into three buckets: proven now with a source anyone can check, not yet proven, and required before this can be claimed at all. A positioning document that overstates evidence is how a brand ships a lie, so this section is not optional and it is written honestly even when the honest version is short. Name the specific artifact that would move each unproven claim, and who owns it.

8. **Assemble the statement and write the reasoning trail.** The statement is the compressed output. The reasoning trail is what makes it defensible six months later: for each of the five choices, one line on what the runner-up was and why it lost. Add a short "what we deliberately do not claim" list, because the claims you refuse are part of the position.

9. **Escalate and hand off.** List the strategic questions for the user, unanswered, as questions. Package the ICP characteristics, the ranked alternatives, the pillars-in-waiting, and the evidence so `messaging-framework` can run next.

## Output format

```markdown
# Positioning: <subject>

**Date:** YYYY-MM-DD
**Status:** DRAFT / PROPOSED / ADOPTED
**Method:** April Dunford's positioning approach, applied. Public source: <title and link>.
**Inputs read:** <path or URL, dated> ; <path or URL, dated>
**Your description:** <what the person running the skill wrote about the product, in their words>
**Validated against real buyer conversations:** yes / no, and how many

## Positioning statement

**For** <the target customer>
**who** <the situation or pressure they are in>
**<Product>** is a <market category>
**that** <the value it delivers>
**Unlike** <the top competitive alternative, named>
**<Product>** <the differentiated thing, traceable to a unique attribute below>

## 1. Competitive alternatives

What the customer actually does today. Ranked.

| # | Alternative | What the buyer gets from it | What it costs them | Evidence | ASSUMED? |
|---|---|---|---|---|---|
| 1 | <the one to beat> | | | <source> | no |
| 2 | doing nothing | | | | |
| 3 | a person plus a spreadsheet | | | | |

## 2. Unique attributes

| Attribute | Not true of which alternative | How an outsider could verify it |
|---|---|---|

## 3. The value each attribute enables

| Attribute | Value to the buyer, in their terms |
|---|---|

## 4. Who cares a lot

**Characteristics of the buyer who cares disproportionately:**
- <situation>
- <constraint>
- <what is currently on fire>

**For your ICP work:** <one line>

## 5. Market category

**Category:** <the frame of reference>
**What a buyer then assumes:** <price, buying process, who signs>
**Assumptions that are wrong, and how the statement corrects them:** <...>
**Strategic decision?** yes / no. If yes, it is in section 8.

## 6. Proof status

**Proven now:** <claim, and the source anyone can check>
**Not yet proven:** <claim, and the artifact that would prove it, and its owner>
**Required before this can be claimed at all:** <...>

## 7. What we deliberately do not claim

- <claim refused, and why>

## 8. Strategic questions for the user

1. <question, with the two options and the tradeoff, left unanswered>

## Reasoning trail

| Choice | What we picked | Runner-up | Why the runner-up lost |
|---|---|---|---|
| Top alternative | | | |
| Lead attribute | | | |
| Lead value | | | |
| Who cares a lot | | | |
| Category | | | |

## Handoff to messaging

**ICP:** <path or inline> | **Alternative to beat:** <...> | **Evidence file:** <path>
```

## Quality bar

- The statement names a specific competitive alternative. The word "competitors" in the plural, unnamed, does not appear.
- Every alternative ranked above position 3 carries an evidence source, or is labeled ASSUMED and is not ranked first.
- Every unique attribute has a written verification route an outsider could follow.
- Every attribute maps to exactly one value line. No orphan attributes.
- The proof status section separates proven from unproven, and every unproven claim has a named closing artifact and an owner.
- April Dunford is credited by name with a specific public source cited. No passage of her writing is reproduced.
- Strategic choices appear in section 8 as open questions addressed to the user, not as decisions made in the body.
- The "validated against real buyer conversations" line states a number, including when that number is zero.
- No em-dashes in your own prose. Em-dashes inside quoted source material are preserved exactly.
- Every factual claim about product marketing practice in general carries a public source.
- Sources are public or supplied by the user. No confidential material from anywhere else.

## Where it lands

Save the output as a markdown file named `YYYY-MM-DD-positioning-<subject>.md` wherever the user keeps working drafts. If the user maintains a canonical positioning document, propose changes against it; let the user edit that file rather than overwriting it. Have a reviewer check the draft before it is treated as final.
