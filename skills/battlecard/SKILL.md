---
name: battlecard
description: Build or refresh a one-competitor sales battlecard with blunt, evidence-backed strengths and weaknesses on both sides, the traps a seller falls into, the real objections with honest answers, and discovery questions. Use when a named competitor shows up in a deal, when sales asks how to sell against a specific rival, or when a monthly refresh finds a card older than 30 days.
---

# Battlecard

Turn a verified competitor profile into a one-screen card a seller can use live on a call: where we win, where they win, the traps, and the language to use. The card is blunt in both directions. It states our own honest weaknesses next to theirs, because a card that only flatters our side gets ignored the first time a buyer contradicts it. It tells the seller where they are about to get hit, not what they already believe.

## When to use

- A named competitor appears in a real deal, so a card would be opened rather than filed.
- Sales asks how to sell against a specific rival.
- An existing card is more than 30 days old, or its competitor has launched or changed pricing since the last review.
- Win-loss findings contradict what a live card says.

Do NOT use this skill for a first research pass on a competitor. Build the profile first (see `competitor-profile`). The battlecard is a rendering of verified intel, not a fresh research pass.

## Required inputs

Refuse to run without the first three. Say which one is missing, who can supply it, and stop. Do not write a stub card.

1. **A current competitor profile** for the named competitor, no older than 30 days, with every claim sourced and dated. If none exists, produce one with `competitor-profile` first.
2. **Your current messaging** (a messaging framework or at least a positioning statement), so the counter-language matches your positioning instead of inventing new claims. The card does not write the pitch; it reports what is true and points at language that already exists.
3. **Real objections**, from calls that have actually happened, in the buyer's words. Ask the user or sales for them. Invented objections train sellers for a conversation nobody has.
4. **Optional, preferred:** field signal from won and lost deals against this competitor.
5. **Optional:** the buyer seat the card is for (for example, in security: detection engineer, identity architect, cloud security lead, application security lead, or CISO). One seat per card. If the product is chosen by practitioners and signed by an executive, note both, and say which one the card is written for.

## Method

1. **Check freshness first.** Read the profile's review-by date and the competitor's recent moves. If they launched, changed pricing, or repositioned since the profile was written, refresh the profile before building the card. A stale card is worse than no card because it is confidently wrong.

2. **Write the one-line read.** One sentence on who this competitor is and when they show up in deals. If you cannot write it in one sentence, the profile has not answered its question yet.

3. **List where they genuinely win.** Pull from the profile's "where they genuinely beat us" section. Each item is something a buyer would actually choose them for, with a dated public source. No throwaways like "bigger brand".

4. **List where we genuinely win.** Same standard. Each item carries evidence and maps to a claim in your messaging. A win you cannot prove does not go on the card; it goes in "claims cut for lack of proof".

5. **Name our honest weaknesses against them.** At least one, in the same plain type as theirs. This is the point of the card. The seller already knows where you are strong.

6. **Write the three traps.** The three places a seller falls in against this competitor: the feature comparison you lose, the question that makes you look evasive, the claim of theirs that sounds unanswerable. For each, what the seller should do instead.

7. **Write the objection answers honestly.** For each real objection: the objection in the buyer's words, the honest response, and the point at which the honest response is "we are not the right fit." A card without that line teaches reps to bluff, and technical buyers detect bluffing fast. Never discredit a product the buyer already owns.

8. **Write the discovery questions.** Three to five questions that surface the difference between you and this competitor early, before the buyer has framed the deal on the competitor's terms.

9. **Enforce the sourcing rule.** Every claim about the competitor carries a public source and the date it was checked. Anything unverifiable is labelled `UNVERIFIED` or cut. Conflicting sources go to the user for a ruling and are marked `CONFLICT, ESCALATED YYYY-MM-DD`, never smoothed over with "reportedly" or "some users say".

10. **Keep it to one page.** A two-page battlecard is a document nobody opens mid-call. Cut until it fits.

11. **Save the file** as `YYYY-MM-DD-battlecard-<competitor-slug>.md`, with a refresh log line at the bottom. Have someone other than the author review it before sellers get it.

## Output format

```markdown
# Battlecard: <Competitor>

**Last reviewed:** YYYY-MM-DD   **Review by:** YYYY-MM-DD (30 days)
**Buyer seat:** <one seat>
**Built from:** <competitor profile filename and date>

## One-line read
<who they are and when they show up>

## Where they win
- <strength>. Source: <url>, checked YYYY-MM-DD

## Where we win
- <strength>. Proof: <source>, checked YYYY-MM-DD

## Our honest weaknesses against them
- <weakness, stated plainly>

## Three traps
1. <trap>. Instead: <what to do>
2. <trap>. Instead: <what to do>
3. <trap>. Instead: <what to do>

## The real objections
| Objection, in the buyer's words | The honest answer | When to walk |
|---|---|---|

## Discovery questions
1. <question>

## Claims cut for lack of proof
<each claim removed, and what evidence would restore it>

## Sources
| Claim | Source | Checked |
|---|---|---|

## Refresh log
- YYYY-MM-DD: <created / refreshed, and what changed>
```

## Quality bar

- [ ] Built from a competitor profile no older than 30 days.
- [ ] Fits on one page.
- [ ] At least one honest weakness on our own side.
- [ ] Every competitor claim carries a public source and a check date. Zero unsourced claims.
- [ ] No hedging words standing in for a conflict. Conflicts are escalated and marked.
- [ ] Objections are real, in the buyer's words, and every one has a "when to walk" line.
- [ ] Nothing discredits a product the buyer already owns.
- [ ] Counter-language matches your existing messaging; no new positioning claims invented on the card.
- [ ] Refresh log line present, with a review-by date 30 days out.
- [ ] No em-dashes in your own prose. Quoted source material is preserved exactly.

## Freshness

No live card sits more than 30 days unreviewed. Run a monthly sweep across all live cards; any card past its review-by date, or whose competitor has moved since, gets flagged as stale rather than quietly served.
