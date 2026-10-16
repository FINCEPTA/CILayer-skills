---
name: "quarterly-credit-letter"
description: "Write a head of credit's quarterly portfolio letter: what moved, attribution, alpha vs. score-cutoff beta, outlook with triggers & asks. Use for credit portfolio reviews, debt partner updates or QBR credit narratives."
---

# Quarterly Credit Letter

Help a head of credit / CRO / credit lead at a lender write a quarterly portfolio letter, the lending equivalent of a fund manager's LP letter. The letter explains what moved in the portfolio last quarter, why it moved, how the external environment maps to the book, which levers were pulled, where the portfolio is heading (with explicit triggers), what the team needs from partners & what it got wrong.

Use this skill whenever someone wants to write or prepare a quarterly credit/portfolio review, a debt partner or warehouse lender update, a board credit memo, a QBR credit narrative, a "portfolio thesis" or an explanation of why delinquency/default/loss rates changed, even if they never say "letter".

## The core idea (keep it in mind throughout)

A score cutoff is **beta**: anyone using the same bureau score at the same threshold inherits the same risk/return, & the book moves with the credit cycle. **Alpha** is the risk-adjusted yield earned above what a peer using the same score at the same cutoff would earn. It comes from segment selection, data that shifts the risk frontier, pricing vs. cost of funds, channel quality, servicing & anticipating macro/policy shifts in specific sub-segments.

The letter's job is to show the reader (and the author) which of the two the team is managing. A letter that only reports metrics is a dashboard. A letter that attributes, takes a view & commits to triggers is a thesis. Push gently but consistently toward the second.

## Workflow

### Step 1: Set the frame (ask briefly, 1 round)

Find out, from the conversation or by asking:

- **Audience:** internal team, board, debt partners (warehouse, forward-flow buyer, ABS investors), bank partner, or several. Audience decides what's disclosed & how candid the misses section is. If several, plan an internal master version plus an external cut.
- **Period:** which quarter, & whether a prior quarter's letter exists (if so, ask for it: last quarter's outlook & triggers get scored in this one).
- **Book basics:** product(s), segment(s), approximate size, funding structure, states/charter setup. Skip whatever the data already shows.
- **Length & voice:** default one to two pages, plain professional voice. Match the author's voice if they share prior writing.

Use a multiple-choice question tool if available. Otherwise ask in plain text, max ~4 questions per round.

### Step 2: Ingest metrics & attribution

The user may provide pasted tables, CSV/XLSX exports, a BI screenshot, a credit committee deck or a CILayer (or similar) attribution export. Read everything first, then build a **metrics sheet** for yourself:

| Metric | Prior Q | This Q | Change | Source | Driver (if known) |

Core metrics to look for (use what exists, don't demand all):
- Originations (count & $), approval rate, average loan size / APR / term
- Outstanding balance, active accounts
- 30+/60+/90+ DPD rates, first payment default (FPD), early roll rates
- Net charge-off rate, gross losses, recoveries
- Cure / rollback rates
- Vintage curves (cumulative loss or DPD by months on book)
- Mix by segment, channel, state, score band, product
- Yield, cost of funds, excess spread, covenant/trigger headroom
- CAC by channel, repeat-borrower share

If the user supplied raw data rather than computed attribution, compute it (see **Attribution methods** below). Show the math in a short appendix table so it can be checked. If attribution was supplied (e.g. from CILayer), use it as-is & note the source; don't recompute it differently without flagging the difference.

**Never invent numbers.** Where data is missing, write `[DATA NEEDED: ...]` in the draft & list it at the end. Clearly separate facts from the author's views & from your suggestions.

### Step 3: Interview, section by section

This step is where the letter's quality comes from. The data says *what*. Only the author knows *why* & *what next*. Ask questions from the **Question bank** below, but:

- Ask only what the data & conversation haven't answered. Lead with what you found: "30+ DPD rose 40 bps, & 25 bps of that is the 2026-Q1 vintage in the gig-income segment. What changed in how you underwrote that segment in Q1?"
- Go one section at a time, 3 to 5 questions per round, so it doesn't feel like a form.
- Accept "don't know" & "skip". Note the gap rather than forcing it.
- Use the **challenge prompts** when an answer is a headline rather than a driver, when an outlook has no trigger, or when there are no misses. Be direct & kind, like a sharp risk committee member, not an auditor.
- If the user is in a hurry, offer a fast path: draft from data plus your best inferences, each marked `[CONFIRM]`, then iterate.

### Step 4: Draft the letter

Use the **Letter template** below. Keep the same section order every quarter so readers learn where to look. Write tight: short paragraphs, numbers in the text where they make the point, a table only when it carries more than three numbers.

Output format: if a document/doc tool is available, write it there so it can be edited & shared. Otherwise produce a .md or .docx per the user's preference. For multiple audiences, draft the internal master first, then the external cut (see **Audience adjustments**).

### Step 5: Quality check before handing over

Run through the **Checklist** below, fix what you can & list the open items (data needed, confirmations, judgment calls) in a short note after the draft.

---

## Attribution methods

Use whichever fits the data available. Explain the method in one line in the appendix.

**1. Mix vs. rate decomposition (segments).** Portfolio rate R = Σ wᵢ·rᵢ, where wᵢ is segment i's share of balance (or accounts) & rᵢ its rate.
- Mix effect = Σ (wᵢ,₁ − wᵢ,₀) · rᵢ,₀ (change from shifting toward riskier/safer segments)
- Rate effect = Σ wᵢ,₀ · (rᵢ,₁ − rᵢ,₀) (change from segments themselves getting better/worse)
- Interaction = Σ (wᵢ,₁ − wᵢ,₀) · (rᵢ,₁ − rᵢ,₀)

The three sum to R₁ − R₀. Run it on whichever cut matters most (segment, channel, state, score band, vintage).

**2. Flow attribution (delinquency/default rate).** Change in DQ rate splits into:
- Origination dilution (denominator growth from new loans that can't be delinquent yet): DQ₀/B₁ − DQ₀/B₀
- Roll-forwards: new accounts entering delinquency ÷ B₁
- Cures: accounts rolling back to current ÷ B₁ (negative)
- Charge-offs & paydowns leaving the delinquent pool ÷ B₁ (negative)

Growth masking risk is the most common misread. Always call out dilution explicitly when originations grew fast.

**3. Vintage view.** Compare each vintage's curve at the same months-on-book against prior vintages, & line up the policy/data/channel changes made at each origination date. This is how you tell whether an underwriting change did what was expected.

**4. Fraud vs. credit.** If fraud flags exist, split losses into first-party fraud / synthetic / bust-out vs. true credit loss before attributing. Unseparated fraud distorts every other driver.

### Measuring alpha (differentiation)

Alpha needs a benchmark. Use the best one available & say which:
- **Score-implied benchmark:** expected loss by bureau score band (from the score's validation/odds chart or the lender's own earlier vintages) vs. actual. Outperformance at the same score bands = alpha from something other than the cutoff.
- **Frontier shift:** approval rate at constant loss, or loss at constant approval rate, before vs. after a data/model change. A frontier move is alpha. A movement along the frontier (cutoff change) is beta.
- **Peer/industry benchmark:** bureau industry reports, NY Fed Consumer Credit Panel, public ABS performance in similar collateral, or anonymized peer data if the user has it.
- **Risk-adjusted yield by segment:** yield − credit losses − cost of funds − servicing − CAC (amortized). Puts growth & risk in the same currency.

If no benchmark exists, say so plainly & suggest which one to build for next quarter rather than implying alpha.

---

## Question bank

Pick from these. Don't ask all of them.

**A. What moved & why**
- Which 3 to 5 metrics does your most important reader care about? Did any move outside the range you'd expect?
- How much of the change is mix (where you lent) vs. rate (how those segments performed)?
- Did originations grow fast enough to dilute delinquency? What does the matured-cohort rate say?
- Which vintage is steepening or flattening, & what changed in policy, data, channel or pricing when it was originated?
- Are any losses actually fraud (first-party, synthetic, bust-out)?
- Where is concentration drifting (state, employer/industry, channel, merchant, score band)?
- *Challenge:* "That's what moved. What's the driver behind it? If you had to bet, which single factor explains most of it?"

**B. Environment, mapped to your segments**
- Which macro indicators actually track your borrowers (unemployment in your top states/industries, card or auto DQ in adjacent segments, foreclosures, rent burden)? What did they do?
- Which consumer stress signals show up in your data (student loan repayment & collections, BNPL stacking, overdraft/NSF trends, essentials inflation)?
- Which policy changes touch your book: fair lending posture, immigration (ITIN/thin-file borrowers or workforce-heavy industries), housing affordability, state rate caps & licensing, true-lender rules?
- Does your edge depend on data whose access or cost could change (open banking / Section 1033, aggregator fees, bureau or score changes)? How are you hedging?
- What are competitors doing: tightening, loosening, exiting, entering? What does that do to your applicant pool (adverse selection)?
- *Challenge:* "The national number isn't your borrower's number. What's the version for your top segment?"

**C. Levers you control**
- Funding & pricing: if cost of funds moves 50 to 100 bps, what happens to APR, term, loan size & which segments stop being profitable? How close are you to rate caps, excess spread floors & covenant triggers?
- Charter & licensing: is the current setup (state licenses, bank partner, charter) limiting growth in product, geography or pricing? What's the plan?
- Distribution: which channels are working & why? Compare CAC, loss rate & repeat LTV by channel. Any channel cheap to acquire but expensive in losses?
- Underwriting: which data, attributes, scores or model changes moved the frontier (more approvals at the same risk or less risk at the same approvals)? Which didn't help?
- Servicing & collections: what changed in cure rates, recoveries, settlement or debt sale pricing?
- *Challenge:* "Was that a cutoff move or a frontier move? If a competitor copied your cutoff tomorrow, what would they still not have?"

**D. Outlook & triggers**
- What's your base case for next quarter, & what would make it upside or downside?
- For each scenario: which indicator, crossing which level, triggers which action? ("If X crosses Y, we do Z.")
- Where are you leaning in & pulling back, by segment & channel, & why?
- What do you need from debt partners, bank partners or the board (capacity, pricing, concentration limits, data, approvals)?
- *Challenge:* "Monitoring isn't a trigger. What level, & what exactly would you do?"

**E. What we got wrong**
- What did last quarter's letter (or plan) predict that didn't happen?
- Which decision would you make differently, & what did you change because of it?
- *Challenge:* "Every honest quarter has at least one miss. Debt partners trust a letter more when it names one."

---

## Letter template

```
[Company] Quarterly Credit Letter: [Quarter Year]
[Author, title] · [Date] · [Audience / confidentiality line]

Summary (3 to 5 sentences)
The one-paragraph version: what moved, the main driver, the view for next
quarter & the key ask.

1. What moved
   3 to 5 key metrics, prior vs. current, with attribution
   (mix / rate / dilution / cures / vintage). Small table if useful.

2. Why: internal vs. external drivers
   What came from our decisions vs. the environment.

3. The environment, mapped to our book
   Macro, consumer stress, policy & data shifts, each tied to a segment.

4. Levers we pulled (& results)
   Pricing & funding · policy & underwriting · channels · servicing.
   Where we earned alpha vs. where we rode beta, with the benchmark used.

5. Outlook & triggers
   Base / upside / downside, each with "if X crosses Y, we do Z".
   Where we're leaning in & pulling back.

6. Asks
   What we need from debt partners, bank partners, board.

7. What we got wrong
   Last quarter's misses & what changed because of them.

Appendix: metric definitions, attribution method & data sources.
```

If a previous letter exists, open section 7 (or a short box under the Summary) by scoring last quarter's triggers & outlook against what happened.

## Audience adjustments

- **Internal / board:** full candour, segment-level detail, named misses, open debates.
- **Debt partners:** lead with what they underwrite (collateral performance, concentration, covenant/trigger headroom, excess spread) & the asks. Keep the attribution & triggers, as they're what builds trust. Remove competitively sensitive detail (exact data vendors, model features, channel economics) unless the user wants it in. Keep the misses section, framed as "what we saw & what we changed".
- **Bank partner:** add compliance posture (fair lending monitoring, complaint trends, licensing) & how growth stays within the program's risk appetite.

## Guardrails

- No fabricated data, benchmarks or peer figures. Use `[DATA NEEDED]` & `[CONFIRM]` markers.
- Keep views & facts separate. Write the author's views as theirs; mark your suggestions as suggestions until accepted.
- Fair lending: never suggest using or proxying protected characteristics in underwriting, pricing or marketing. When discussing policy topics like immigration, frame them as portfolio exposure & data/eligibility questions, not borrower characterizations. Flag any segment or attribute that could raise disparate impact questions for the author's compliance review.
- For external versions, remind the author to have legal/compliance review statements about performance or forward-looking views before sending.
- External macro or policy facts should come from a source the reader can check (FRED, NY Fed, CFPB, bureau reports). If you can search the web, verify current figures. Otherwise mark them `[VERIFY]`.

## Checklist

Before handing over the draft, confirm:
- [ ] The Summary states the main driver, not just the metric change.
- [ ] Every headline metric change has an attribution (or an explicit "unknown, investigating").
- [ ] Growth dilution is called out if originations grew materially.
- [ ] Each external factor is tied to a specific segment in the book.
- [ ] At least one alpha claim is backed by a named benchmark, or the letter says none exists yet.
- [ ] Each outlook scenario has at least one explicit trigger & action.
- [ ] Asks are specific (who, what, how much).
- [ ] The misses section has at least one real entry.
- [ ] No invented numbers. Open `[DATA NEEDED]`/`[CONFIRM]`/`[VERIFY]` items are listed after the draft.
- [ ] Length fits the audience (aim for 1 to 2 pages plus appendix).