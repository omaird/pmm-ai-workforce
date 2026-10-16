---
name: teardown
description: Run a before/diagnosis/after teardown of a public company homepage, positioning page, or pricing page, using the Eight Reads lens (reader, category, claim, ask, clock, vocabulary, proof, swap). Use when a content slot calls for a teardown, when the user supplies a page URL plus their opinion on why it fails, or when a candidate page has been picked for a teardown. Do not use to hunt for candidates, and do not use on pages behind a login.
---

# Teardown

The structure is always before, diagnosis, after. The diagnosis is the value: a teardown that lists what is wrong is a review, and a teardown that names precisely which positioning or messaging failure is happening, and what it costs the company, is a method a reader can point at their own page. The Eight Reads lens below is what makes the format recognisable from issue to issue.

The examples here come from security vendors, where the lens was built, but it works on any B2B homepage.

## When to use

Fire this when you are publishing a before/diagnosis/after rebuild of somebody else's public page. Concrete triggers:

- A content plan has a teardown slot open.
- The user supplies a page URL with a line about what they think is wrong with it.
- A candidate from an idea list has been picked and the user has given their opinion on it.
- A page that was torn down before has since changed in a way worth revisiting. Re-run it as a new dated file. Never edit the old one, because the old one is the record of what the page said then.

Do not use this skill when:

- You are hunting for and ranking candidates rather than tearing one down.
- The page belongs to the user or their client and the job is to produce replacement copy as a deliverable. A teardown is public commentary on a page you do not own; commissioned copy is a different job.
- The output is a competitive assessment for sales use. Use `competitor-profile` or `battlecard`.
- The page sits behind a login, a paywall, a trial, or any agreement. Public sources only. Drop the candidate and say why.

## Required inputs

**Refuse to run without the human ingredient.** The human ingredient for a teardown is the user's opinion on why the original fails, in their own words. The diagnosis is a person's judgment and this skill does not invent it. If no opinion has been given, write nothing, stop, and return exactly this: "Teardown blocked. Need your opinion on why <URL> fails. One or two sentences is enough." The judgment is the only part of a teardown a competitor cannot fake, so this refusal is the format.

With that in hand, collect all of the following before writing:

- [ ] **The user's opinion**, quoted verbatim, with the date they gave it.
- [ ] **The live public URL**, the exact page, not a roundup or a screenshot of it.
- [ ] **The date fetched**, recorded in the file. Pages change. A teardown of a page that has since been rewritten is a correction waiting to happen, and the fetch date is what turns that from an error into a timestamp.
- [ ] **The copy as written**, captured verbatim: hero headline, subhead, every CTA label in order, section headers in order, and any proof on the page (logos, numbers, named customers, quotes).
- [ ] **The company's own category words**, taken from the page and the browser title, not from your impression of the product.
- [ ] **Two named competitors** with their public page URLs and fetch dates, for the swap test.

## Method

Nine steps. Run them in order. Steps 4 through 6 are the ones that produce the value.

1. **Load the constraints.** Read any voice guidelines the user has. Two rules bind every line you are about to write, including the rewritten copy: no em-dashes in your own prose, and every claim must be falsifiable.

2. **Confirm the human ingredient and quote it.** Pull the user's opinion verbatim into the draft before anything else, and keep it visible while you work. Everything downstream either supports that opinion or contradicts it, and if the evidence contradicts it, say so in the draft and raise it with the user rather than quietly writing around them. If the opinion is not there, stop per Required inputs.

3. **Capture the before, then verify you captured the right thing.** Fetch the page. Record the URL and the fetch date at the top of the file. Transcribe the copy word for word into the Before section. Do not paraphrase, do not tidy the punctuation, do not fix their typos. The Before section is evidence, and a paraphrased Before makes the diagnosis unarguable in the wrong direction. Em-dashes inside a quoted Before are preserved exactly; the no-em-dash rule covers your prose, not the evidence you are quoting.

   **Verify against the raw markup before you trust a single quote.** A summarising fetch returns what it judged important, not what the page leads with, and it will confidently hand you an announcement banner as the hero. Pull the raw HTML as well and confirm three things: the hero headline, the browser title, and that anything you are about to quote appears verbatim in the source. If the two passes disagree, the markup wins.

   **Do the factual verification here, not at step 8.** Check what the page actually attributes before concluding it attributes nothing: statistics carried in image `alt` text, logos linking to named case studies, claims sourced in a footnote. This is fact-checking and it belongs before the diagnosis is written. Step 8 is the separate, later question of whether the diagnosis is fair.

4. **Run Reads 1 through 7.** Each Read gets a mark of Holds, Soft, or Fails, plus at least one verbatim quote from the page as evidence, recorded in the Eight Reads table.

   **Read 8 waits for step 5.** The swap test compares against competitor pages that have not been fetched yet, and asserting it from memory is the one failure this format cannot survive. Score Reads 1 to 7 here, then score Read 8 immediately after the competitor fetch.

   **These marks are evidence, not the verdict.** Each one is arguable straight from the quote sitting under it. What is NOT decided here is step 6: choosing which failing Read is primary, and saying what it costs. Score every Read here; leave the ruling to the user's opinion.

   - **Read 1, The Reader.** From the words on the page alone, who does this copy assume is reading it? Name the person: their role, and what they came to the page to find out. In security this has to land on a specific seat, because a detection engineer, an identity architect, a cloud security lead, and a CISO read the same page for different things and fear different outcomes. Record the phrases that name or imply them. Fails when the page names nobody ("teams", "businesses", "security leaders"), or names two seats that want different things and gives neither a path.
   - **Read 2, The Category.** What category does the product claim, in the page's own words? Find the noun the company applies to itself in the hero and in the browser title. Fails when there is no category noun and the reader has to guess what kind of thing this is, when the page invents a category nobody has a budget line for, or when the hero claims one category and the pricing page claims another.
   - **Read 3, The Claim.** What is the differentiated claim, and is it falsifiable? Pull the single sentence that is meant to be the reason to choose them over the alternative. Then write its negation. If no company on earth would ever say the negation ("our platform is slow and hard to use", "we do not care about security"), the sentence is decoration, not a claim. Fails when the strongest sentence on the page cannot be proven wrong.
   - **Read 4, The Ask.** What does the copy ask the reader to do next, and has the page earned it? List every CTA label in the order a scrolling reader meets it, and note the proof offered before each one. Fails when several asks compete at equal weight, when the ask costs more than the page has justified (a sales call before the page has said what the product is), or when the verb hides the commitment.
   - **Read 5, The Clock.** Is there a deadline, a regulation, a funding event, or a shift in attacker behaviour that makes this matter this quarter rather than next year, and does the page say so? Security buyers defer easily, because nothing on the page is ever as urgent as the incident in front of them. Fails when the page gives a reader no reason to act now, or when it manufactures urgency it cannot support.
   - **Read 6, The Vocabulary.** Are the company's own product names and internal terms outranking the plain words a buyer uses for the job? Count the named layers, tiers, and modules in the nav and the hero. Fails when a first-time visitor cannot map a named thing to a job they need done. Named layers are internal architecture, and a buyer has to translate them before they can care.
   - **Read 7, The Proof.** Whose words carry the proof? Separate investor and advisor quotes praising the concept from customer quotes describing an outcome. Note whether any number on the page has a unit and a source. Fails when the strongest proof is an investor endorsing the idea, which tells a buyer the round closed rather than that the product works.
   - **Read 8, The Swap.** Put a competitor's logo on this page and see what breaks. Take the two named competitors, go line by line, and mark every line either of them could publish unchanged. Quote the surviving lines and name which competitor could run them. If a competitor's logo could sit on this page unchanged, the positioning is not doing work. The hero surviving the swap is one of the most common failures in security homepage copy and it is often the primary. Security has an aggravating factor: whole categories share a vocabulary, so a hero built from category words survives the swap against every vendor in the category at once.

5. **Fetch the competitors, then score Read 8.** Fetch both competitor pages, record their URLs and fetch dates, and quote the lines you are comparing against. A swap test asserted from memory is a guess, and a guess is what a correction is made of.

   **Check the target's own page for merger or acquisition news first.** The obvious comparison is wrong if the two companies just combined, and the target's site is usually where that is announced. If the target is mid-acquisition, stop and ask the user whether to proceed, because tearing down a company in the middle of being acquired is an editorial call about the brand, not a copy call. Until they rule, keep the work as evidence only (see "When a gate fires after work exists").

6. **Write the diagnosis, from the user's opinion rather than from your own.** Name exactly one primary failure.

   **The user's opinion decides it, not the severity of the marks.** If their opinion points at Read 2 while Read 5 failed harder on the evidence, the primary failure is Read 2. Severity ranks the evidence; the human judgment ranks what it costs the company, and the second is the thing a competitor cannot copy. Note the harder-failing Read as a secondary.

   **How to pick when several Reads fail, which is the normal case.** Map the user's opinion to the failing Reads and name the one it points at. If they wrote that the page never says what the product is, that is Read 2. If they wrote that any competitor could run the same headline, that is Read 8. You are not choosing on your own judgment; you are reading theirs onto the evidence.

   Escalate only when their opinion does not map to any Read that actually failed. That is a real signal and not a formality: it means either the mechanical pass missed something they can see, or they are reacting to something outside the page. Say which Reads failed, quote their opinion next to them, and ask which one they meant. Do not pick for them, and do not quietly widen a Read to make it fit.

   State the primary failure in one precise sentence, show the quoted copy that proves it, then say what it costs the company. The cost sentence is where teardowns go wrong. "This hurts their conversion rate" cannot be argued with and is therefore worthless. Good judgment here looks like naming a specific visitor, where they arrived from, the moment they give up, and what they do instead: "a platform engineer who arrived from a comparison query cannot tell within one screen whether this replaces their existing scheduler, so they go back to the comparison page and read the competitor's version." Add at most two secondary failures, one line each. If any general claim about marketing practice appears (a benchmark, a named method, a percentage), it carries a public source URL in the Sources list. Unsourced specifics get cut.

7. **Write the after as literal copy.** Replacement lines, not advice. "They should lead with the outcome" is not an after. Rewrite the hero headline, the subhead, the primary CTA label, and the one section that fixes the primary failure, and set each replacement directly beside the line it replaces. Rewrite only what the diagnosis condemned, so a reader can see the diagnosis and the fix are one argument. Every replacement claim must be falsifiable and must be supportable from evidence already public on the company's own site. Inventing a capability or a number to make the rewrite land is fiction and fails the quality bar.

8. **Run the fairness pass, which is purely about tone.** Factual verification happened at step 3, deliberately, because a factual correction discovered here would already be baked into the diagnosis. Before assembling, write one paragraph steelmanning the original: the best reason a competent team, under real constraints, shipped this page. Then check the diagnosis still stands against it, and cut any sentence that mocks the company or its team. A teardown that strawmans its target damages the author's credibility more than the target's. The people who wrote that page read these, and the format only has authority if it would survive being read by them.

9. **Assemble and save.** Fill the template, include the `Your opinion` line, save it per "Where it lands", and have a reviewer check it before it is published.

## Output format

````markdown
# Teardown: <Company>, <page type>

**Source:** <full public URL>
**Fetched:** YYYY-MM-DD
**Your opinion, given YYYY-MM-DD:**

> <The user's opinion, quoted verbatim. One to three sentences.>

## Before

The page as it read on <fetch date>. Quoted, not paraphrased.

- **Hero headline:** "<verbatim>"
- **Subhead:** "<verbatim>"
- **Primary CTA:** "<verbatim label>"
- **Secondary CTA:** "<verbatim label, or none>"
- **Section headers, in order:** <verbatim list>
- **Proof on the page:** <logos, numbers, named customers, quotes, or "none">

## The Eight Reads

| Read | What the page does | Evidence, quoted verbatim | Mark |
|---|---|---|---|
| 1. The Reader | <who the copy assumes is reading, in one line> | "<the line that names or implies them>" | Holds / Soft / Fails |
| 2. The Category | <the category noun the page claims> | "<the hero or title line carrying it>" | Holds / Soft / Fails |
| 3. The Claim | <the differentiated claim, and its negation> | "<the claim as written>" | Holds / Soft / Fails |
| 4. The Ask | <what the reader is asked to do next> | "<the CTA label, verbatim>" | Holds / Soft / Fails |
| 5. The Clock | <the reason to act now, or none> | "<the line carrying urgency, or none>" | Holds / Soft / Fails |
| 6. The Vocabulary | <named internal terms outranking plain words> | "<the nav or hero term>" | Holds / Soft / Fails |
| 7. The Proof | <whose words carry the proof> | "<the strongest proof line>" | Holds / Soft / Fails |
| 8. The Swap | <what survives a logo swap> | see the full swap test below | Holds / Soft / Fails |

Every Read carries its quote in the table; do not add per-Read prose sections beneath it. Read 8 is the exception, because a swap test needs several lines and two competitors, so it expands below.

**Read 8 in full, the swap test.** Lines that survive a logo swap, and who could run them:

- "<verbatim line>" could run unchanged on <Competitor A>.
- "<verbatim line>" could run unchanged on <Competitor B>.
- Lines that could not: "<verbatim line>", because <reason>.

## Diagnosis

**Primary failure: Read <N>, <one precise sentence naming the failure>.**

<The quoted copy that proves it.>

**What it costs them.** <Which visitor, arriving from where, gives up at which point, and what they do instead.>

**Secondary.**
1. <one line>
2. <one line>

**The fair reading.** <One paragraph: the best reason a competent team shipped this page. Then why the diagnosis survives it.>

## After

Replacement copy, not advice.

**Hero headline**
Before: "<verbatim>"
After: "<replacement>"
Why: <one line, tied to the failing Read>

**Subhead**
Before: "<verbatim>"
After: "<replacement>"
Why: <one line>

**Primary CTA**
Before: "<verbatim label>"
After: "<replacement label>"
Why: <one line>

**<The one section that fixes the primary failure>**
Before: "<verbatim>"
After: "<replacement, written out in full>"
Why: <one line>

## Does the rewrite pass the swap test?

<One paragraph. Run Read 8 on the new copy. Name the competitor that could not publish these lines, and say what stops them.>

## What a reader can steal from this

<Two to four bullets. The method, not the conclusion. A reader should be able to run the same lens on their own page tonight.>

## Sources

- <page URL>, fetched YYYY-MM-DD
- <Competitor A URL>, fetched YYYY-MM-DD
- <Competitor B URL>, fetched YYYY-MM-DD
- <public source URL for any general marketing claim made above>
````

## Quality bar

Every line below is checkable. Fail one and the file is not ready for review.

- The file carries a `Your opinion` line, and the user's opinion appears quoted verbatim. No opinion given means no teardown was written.
- The source URL and the fetch date are recorded for the torn-down page and for every competitor page cited.
- All eight Reads carry a mark of Holds, Soft or Fails, and at least one verbatim quote from the page. No Read is blank and no Read is skipped. The word "verdict" is deliberately not used for these: a mark is evidence, and the verdict is the diagnosis, which follows the user's opinion.
- The swap test names at least two real competitors and quotes the specific lines that survive the swap. "A competitor could say this too" without the competitor named and the line quoted does not count.
- The diagnosis names exactly one primary failure. The cost sentence identifies a specific visitor and the specific moment they leave. "Hurts conversion" fails.
- The After contains literal replacement copy for the hero headline, the subhead, and the primary CTA. Any recommendation phrased as advice fails.
- Every replacement claim can be proven wrong, and every replacement claim is supportable from something already public on the company's own site. No invented capabilities, no invented numbers.
- The fair reading paragraph exists, and no sentence anywhere mocks the company or its team. Read the file as if the target's product marketer will read it, because they will.
- Any general claim about marketing practice carries a public source URL in the Sources list. Everything cited is public. No confidential material.
- No em-dashes in your own prose. Em-dashes inside quoted source material are preserved exactly.
- Delete the company name and the "What a reader can steal from this" section still stands on its own. If it does not, the piece is an opinion about one company, not a teardown.

## Where it lands

Save the teardown as a markdown file named `YYYY-MM-DD-teardown-<company>.md`, where `<company>` is the company name lowercased with hyphens for spaces.

### When a gate fires after work exists

Steps 5 and 6 can both stop a run once the page has been fetched and the Eight Reads scored. Real evidence about a live page exists by then, and that page will change, so keep the work rather than throwing it away.

**The file.** Save it as `YYYY-MM-DD-teardown-<company>-blocked.md`, so it is never mistaken for a finished teardown.

**The format is this skill's own Output format with four sections omitted.** Write the header block, `## Before`, and `## The Eight Reads` exactly as the template defines them. Omit `## Diagnosis`, `## After`, `## Does the rewrite pass the swap test?`, and `## What a reader can steal from this` entirely, rather than including them empty. An omitted section is unambiguous; an empty one invites someone to fill it.

- **Open it with a blocking header** naming which gate fired, the one question the user has to answer, and that it is not ready for publication.
- **Keep `## Sources`**, including every fetch date. That is the part that goes stale and the reason this file exists.
- If the user's opinion was already given and the gate fired for another reason, quote it under the blocking header so the next run does not have to ask again.

| Gate | Fires when | The question for the user |
|---|---|---|
| Step 5, acquisition | The target's own page announces a merger or acquisition | Do we tear down a company mid-acquisition at all? An editorial call about the brand, not a copy call. |
| Step 6, unmappable opinion | The user's opinion matches no Read that actually failed | Which failing Read did you mean? Either the mechanical pass missed something you can see, or you are reacting to something off the page. |
