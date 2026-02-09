# Module 2: Problem Anatomy

**Status:** DRAFT v1.0
**Last updated:** February 9, 2026
**Feeds:** Marketing "Why Mysa" section, pitch deck slides 1-3

---

## 2.1 Workflow Audit: The Before State

### What an Adjuster Actually Does Today

A claims adjuster's day is a sequence of system switches, phone calls, and manual data entry — punctuated by the actual decision-making that determines what gets paid. Here is the step-by-step "Before" workflow for a typical motor claim at a mid-market European carrier:

| Step | Activity | Time | Systems Used | Pain |
|------|---------|------|-------------|------|
| 1 | **Receive claim notification** — email, portal submission, or phone call from broker/policyholder | 2-5 min | Email + CMS (Guidewire/Duck Creek) | Manual data entry from email into CMS. Copy-paste. |
| 2 | **Open case in CMS** — create file, assign claim number, link to policy | 5-10 min | CMS + policy system | Policy system is separate from CMS. Cross-reference manually. |
| 3 | **Verify coverage** — read policy document, check if claim is covered, check exclusions, check policy was active at time of loss | 15-30 min | Policy document (PDF) + CMS + calculator | Policy is often a 40+ page PDF. Adjuster ctrl-F's through it. No structured extraction. |
| 4 | **Review documents** — EAS form, police report, photos, repair estimates, medical records (if BI) | 15-25 min | Email attachments + CMS + estimation tool | Documents arrive as email attachments. Must be downloaded, renamed, uploaded to CMS. |
| 5 | **Triage** — score complexity, determine if desk or field, assign priority | 5-10 min | CMS + internal rules | Mental calculation based on experience. No standardized scoring in most mid-market carriers. |
| 6 | **Investigation** — make phone calls (policyholder, claimant, witnesses, repair shop, broker), collect statements, request missing documents | 30-60 min | Phone + CMS + email | 20+ calls/day. Each call requires note-taking, then manual entry into CMS. Context from prior calls not surfaced. |
| 7 | **Assessment** — review repair estimate against market rates, check for over-scoping, get independent estimate if needed | 15-25 min | Estimation tool (Xactimate/Audatex) + CMS | Estimation tool is a separate login. Results must be manually transferred to CMS. |
| 8 | **Convention matching** (EU only) — match EAS form data to convention rules (IDS/IRSA/CARD/CIDE) to determine fault percentage | 5-15 min | Convention platform + CMS | Form data must be manually entered into convention platform. Often re-keyed from paper. |
| 9 | **Reserve calculation** — estimate total claim cost for financial reporting | 10-15 min | Spreadsheet or CMS reserve module | Often done in Excel. Senior adjusters use gut feel. P&L impact not surfaced. |
| 10 | **Decision** — determine coverage, liability split, settlement amount | 10-20 min | All of the above + brain | The actual expert judgment. 60-70% of the work has been getting to this point. |
| 11 | **Document generation** — write coverage determination letter, reserve memo, settlement offer | 15-25 min | Word/template + CMS | Templates are generic. Each carrier has different requirements. Manual customization. |
| 12 | **Supervisor review** (if above authority limit) — wait for approval | 0-48 hours wait | CMS workflow | Bottleneck. Supervisor reviews 50+ decisions/day. Quality varies. |
| 13 | **Settlement** — issue payment, close case, document final decision | 10-20 min | CMS + payment system | Payment system is yet another separate login. |

**Total time per claim (simple motor):** 2-4 hours
**Total time per claim (complex motor/BI):** 8-20+ hours spread over weeks
**Total time per claim (property):** 4-12 hours (no convention system, more investigation)

[SOURCE: mysa_product_strategy.md, Parts 1-2; claims_journey_discovery.md — phases 6-11 activity lists; TRANSCRIPT: Feb 9, 2026 — "30-40% is data entry and admin... more than 20 phone calls... context switching between five to seven systems"; TRANSCRIPT: Feb 7, 2026 — "125 open claims, 300-480 closed/year"]

**Cost of this workflow:**

| Metric | Value | Source |
|--------|-------|--------|
| Fully loaded adjuster cost | ~$110K/year | [SOURCE: mysa_product_strategy.md, Part 2a — BLS + transcript] |
| Claims closed per year | 300-480 | [SOURCE: mysa_product_strategy.md, Part 2a] |
| Open claims at any time | ~125 | [SOURCE: mysa_product_strategy.md, Part 2a] |
| Cost per closed claim | $230-$370 | [SOURCE: mysa_product_strategy.md, Part 2a] |
| % time on admin/data entry | 30-40% | [TRANSCRIPT: Feb 7/9, 2026] |
| Systems per claim | 5-7 | [SOURCE: mysa_product_strategy.md, Part 2c] |
| Phone calls per day | 20+ | [TRANSCRIPT: Feb 7, 2026] |

---

## 2.2 The Villain

### The Enemy Is Not Any One System — It's the Gap Between All of Them

The claims adjuster's problem is not a bad CMS. It's not a bad estimation tool. It's not even bad data. **The problem is that the adjuster is the integration layer.**

Every claim requires an adjuster to:
1. Pull data from 5-7 disconnected systems
2. Hold context in their head across weeks of investigation
3. Apply carrier-specific rules they've memorized (or look up in a PDF manual)
4. Make judgment calls with incomplete information under time pressure
5. Document every decision in a format their carrier requires
6. Route decisions to supervisors who review without full context

The adjuster is a human API — receiving inputs from multiple systems, processing them through learned rules, and outputting decisions. **That's what makes the job exhausting, error-prone, and impossible to scale.**

The villain is not a competitor. The villain is **fragmented adjuster data and manual judgment bottlenecks** — the structural gap between where information lives and where decisions happen.

> "Everyone is trying to build a platform. And everyone is avoiding the hard part — the judgment, the decision stage."
> — Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

This gap exists because:
- **Systems were built in silos.** CMS vendors sell case tracking. Estimation vendors sell cost calculation. Fraud vendors sell risk scoring. Nobody built the layer that connects them into a decision.
- **Knowledge lives in heads, not systems.** A 15-year adjuster knows that "water damage claims in this zip code always involve this contractor" — but that knowledge walks out the door when they retire.
- **Every carrier is different.** SOPs, authority levels, reserve rules, documentation requirements — all carrier-specific. No generic tool works everywhere.

[SOURCE: mysa_product_strategy.md, Parts 1-2; AI_NATIVE_ARCHITECTURE_SPEC.md — "Their architecture assumes rules are CODE. Adding AI doesn't change that."]

---

## 2.3 The Workforce Crisis

### The People Who Make These Decisions Are Disappearing

The insurance claims adjuster profession is the 12th fastest-declining in the United States. This is not a future prediction — it is already happening.

| Metric | Data | Source |
|--------|------|--------|
| **BLS profession ranking** | 12th fastest-declining occupation by 2030 | [WEB: BLS Occupational Outlook Handbook — Claims Adjusters, Appraisers, Examiners, and Investigators] |
| **Near-term retirement** | 25% of all claims adjusters will retire within 5 years | [SOURCE: mysa_product_strategy.md, Part 2a + TRANSCRIPT: Feb 7, 2026] |
| **Long-term retirement** | 50% of insurance workforce retiring within 15 years | [SOURCE: mysa_product_strategy.md, Part 2a — industry survey] |
| **Annual attrition** | 20% at carriers, 33% at TPAs (Third-Party Administrators) | [SOURCE: mysa_product_strategy.md, Part 2a] |
| **Knowledge loss** | ~6 years of institutional knowledge lost per departure | [SOURCE: mysa_product_strategy.md, Part 2a] |
| **Replacement cost** | 12% higher operational costs from high turnover; 20% higher indemnity payouts from less experienced adjusters | [SOURCE: mysa_product_strategy.md, Part 2a] |
| **Fully loaded cost** | ~$110K/year per adjuster | [SOURCE: mysa_product_strategy.md, Part 2a] |
| **Training time** | 6 years to develop full adjuster expertise | [SOURCE: mysa_product_strategy.md, Part 2a] |

> "They're all boomers... their work output is super bad. Because they work like boomers. They are not digital native. So they cannot interact with very old tech properly, and they can surely not interact with new tech."
> — Jeremy Blehaut [TRANSCRIPT: Feb 7, 2026]

> "The worst part is... they're all going for retirement. This is a job that is requiring people. They have high turnover, high attrition. They are not able to lock new generations into this job."
> — Jeremy Blehaut [TRANSCRIPT: Feb 7, 2026]

### Why This Creates Urgency

The workforce crisis compounds across three dimensions:

**1. Volume is increasing, headcount is decreasing.**
Total claims volume is growing — driven by climate change (more weather events = more property claims), more vehicles on the road, and inflation increasing claim values. Meanwhile, the adjusters processing those claims are retiring faster than they can be replaced. [TRANSCRIPT: Feb 8, 2026 — "the total number of claims are increasing... climate change has increased the total number of claims"]

**2. Expertise cannot be replaced fast enough.**
It takes 6 years to develop full adjuster expertise. A carrier losing a 15-year veteran cannot produce a replacement in any reasonable timeframe. The knowledge — which policy clauses matter, how to negotiate with contractors, when to suspect fraud, what reserves are realistic — exists in the adjuster's head, not in any system.

**3. The remaining workforce struggles with existing tools.**
The current workforce skews older and is not "digital native." They struggle with the 5-7 systems they already use. Adding another tool that doesn't fundamentally change the workflow just adds burden. [TRANSCRIPT: Feb 7, 2026 — "boomers that must be working insurance and struggle to interact with non-AI, non-agentic products"]

**What carriers need:** Technology that (a) makes existing adjusters 2-3x more productive, (b) makes new adjusters effective in weeks instead of years, and (c) captures tribal knowledge into systems so expertise doesn't retire with the person.

[SOURCE: mysa_product_strategy.md, Part 2a; TRANSCRIPT: Feb 7, Feb 8, 2026]

---

## 2.4 The STP Reality Gap

### Convention Systems Promise 60-70%. They Deliver ~10%.

STP — straight-through processing — is the insurance industry's term for claims that can be resolved near-instantly with minimal human review. In European motor insurance, convention systems (IDS in Portugal, IRSA in France, CARD in Italy, CIDE in Spain) are designed to make multi-party claims STP-capable by applying deterministic fault rules.

**The promise:** A two-car accident where both parties fill out an EAS (European Accident Statement) form should resolve in seconds. The convention system matches the checkboxes on the form to a fault table, assigns a percentage, and both insurers pay their policyholders. No investigation, no negotiation, no delay.

**The reality:** ~10% of claims achieve STP. The other 50-60% that should be automatic are not — because the data is garbage.

> "Our north star is improving the STP... basically the amount of [claims] automatically [processed]... it takes seconds. It's like someone just reviewing it."
> — Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

### Why the Gap Exists

The convention lookup itself is trivial — it's a database query matching checkboxes to fault percentages. The bottleneck is getting clean, structured data FROM the EAS form INTO the convention system.

| Data Quality Problem | Impact | Frequency |
|---------------------|--------|-----------|
| ~50% of EAS forms are still paper | Must be manually digitized before convention lookup | Very common in Southern EU |
| Filled out by stressed people at accident scenes | Messy handwriting, unclear checkboxes, incomplete fields | Nearly universal |
| Diagrams are ambiguous | Convention case depends on which box is checked — ambiguous diagrams lead to wrong case selection | ~20-30% of forms |
| Missing fields | Convention system cannot process incomplete data | ~15-25% of submissions |
| Manual data entry | Re-keying from paper introduces transcription errors | ~10-15% error rate |
| Inconsistent field interpretation | Different adjusters interpret the same form differently | Systematic |

[SOURCE: mysa_product_strategy.md, Part 2b; claims_journey_discovery.md — Phase 3 STP analysis]

**The opportunity:** Whoever fixes data quality upstream unlocks a 50+ percentage point STP improvement. That's not marginal — it's transformational. A carrier going from 10% to 40-50% STP on motor claims saves hundreds of adjuster-hours per month.

Mysa's OCR + document understanding engine (currently at 81.5% accuracy on Portuguese EAS forms) is the key that unlocks the convention system. The product fixes the data quality problem as a means to enabling the decision engine — not as an end in itself.

[SOURCE: mysa_product_strategy.md, Part 2b; caravela-ocr.md (memory) — accuracy metrics]

### STP by Region

| Region | STP Mechanism | Promise | Reality | Gap |
|--------|-------------|---------|---------|-----|
| **EU Motor (convention)** | IDS/IRSA/CARD/CIDE — deterministic fault tables | 60-70% | ~10% | **50-60 pp** — data quality bottleneck |
| **EU Property** | None — no convention system for property | N/A | Near-zero STP | No mechanism exists. Every claim is manual. |
| **US Motor** | No convention system. State-by-state rules. | Variable | Very low for complex claims | US is more adjuster-intensive than EU. |
| **US Property** | No convention system. Estimation tools (Xactimate) provide cost data but not decisions | Variable | Low | Same problem — the decision is manual. |

[SOURCE: claims_journey_discovery.md — cross-phase STP analysis; mysa_product_strategy.md, Part 6b — convention systems by country]

---

## 2.5 The Productivity Drain

### 30-40% Admin. 5-7 Systems. 20+ Phone Calls Per Day.

> "The work of an adjuster, 30 to 40%, is data entry and admin. Manual reads papers. Types into the CMS, more than 20 phone calls, context switching between five to seven systems."
> — Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

An adjuster's time breaks down as follows:

| Activity | % of Time | Automate? | How Mysa Helps |
|----------|----------|-----------|----------------|
| **Data entry & admin** | 30-40% | YES | Document parsing auto-populates fields. OCR extracts from EAS forms, invoices, reports. |
| **Travel** (field inspections) | 25-30% | Partial | Better triage reduces unnecessary field visits. Desk adjusters handle more claims. |
| **Documentation** | 20-25% | YES | AI generates coverage letters, reserve memos, settlement offers per carrier SOP templates. |
| **Actual decision-making** | 10-20% | Augmented | The 6 decision sub-steps with AI recommendation + confidence score. Human reviews, not types. |
| **Phone calls / context switching** | 10-15% | YES | Call recording + transcription. Guided scripts per SOP. Context from prior calls surfaced automatically. |

[SOURCE: mysa_product_strategy.md, Part 2c; TRANSCRIPT: Feb 7, 2026]

**The systems an adjuster typically uses per claim:**

```
1. Xactimate or Audatex (estimation)
2. CMS — Guidewire ClaimCenter, Duck Creek, or proprietary
3. Policy administration system (separate from CMS at many carriers)
4. Convention platform (EU only — CIMPAS, CIDE portal, etc.)
5. Phone/call system + note-taking
6. Email (broker/claimant communication)
7. Carrier reporting portal (reserves, financials)
```

At mid-market carriers, these are often not integrated. The adjuster is the integration layer — logging into each system, extracting what they need, making sense of it, and entering conclusions back into the CMS.

[SOURCE: mysa_product_strategy.md, Part 2c — "5-6 separate systems per claim"]

### The Productivity Math

| Metric | Current | With Mysa (3x) | Impact |
|--------|---------|----------------|--------|
| Claims closed/year per adjuster | 300-480 | 900-1,440 | Same headcount, 3x throughput |
| Cost per claim | $230-$370 | $75-$125 | 60-66% cost reduction per claim |
| Savings per adjuster per year | — | $45-$120K | Pays for the product many times over |
| For a team of 20 adjusters | — | $900K-$2.4M/year saved | Clear ROI even at highest pricing tier |
| For a mid-tier TPA (200 adjusters) | — | $9-$24M/year saved | Transformational |

[SOURCE: mysa_product_strategy.md, Part 2c — "3x productivity math"]

> The productivity gain is not just "adjuster types faster." It's: (a) admin work is automated (30-40% of time freed), (b) decisions are pre-populated and reviewed rather than built from scratch (10-20% of time compressed to 2-3%), (c) documentation is generated (20-25% of time eliminated), (d) new claims can be taken on because backlog clears.

[TRANSCRIPT: Feb 8, 2026 — "there's probably that they can also take new claims... there is also the fact that they have more and more open claims that are long lasting"]

---

## 2.6 Reserve = P&L Impact

### The CFO's Problem — And Why It Opens a Second Buyer

Reserves are money set aside by an insurer for expected future claim payments. They are not optional — they're a regulatory and accounting requirement. And they hit the P&L immediately.

> "Do you know this concept? It's not what they are paying that matters. It's how much money they are reserving. Because reserves are already recognized in the P&L right away."
> — Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

> "And there are no rules... but they will hold you accountable if the reserve is too different from the value that you end up paying."
> — Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

### How Reserves Work (for non-insurance readers)

When a claim is filed, the insurer must immediately estimate how much it will eventually pay. This estimate — the reserve — is recorded as a liability on the balance sheet and an expense on the income statement. It affects:

| Impact | Over-Reserving (estimating too high) | Under-Reserving (estimating too low) |
|--------|--------------------------------------|--------------------------------------|
| **Financial statements** | Looks less profitable than it actually is | Looks more profitable — until reality catches up |
| **Stock price / investor confidence** | Depressed earnings, lower valuation | Surprise loss when reserves are corrected upward |
| **Regulatory** | Ties up more capital than necessary (reduces capital efficiency) | Regulatory intervention. Potential solvency warnings. |
| **Reinsurance** | Higher ceded premiums | Reinsurance disputes at renewal |
| **Year-end adjustment** | Positive "reserve release" — but suggests inefficiency | "Reserve strengthening" — triggers board questions |

**The math for a Caravela-sized carrier:**
- 57,000 claims/year, average reserve ~€2,000-€5,000 per motor claim
- Total reserves in force: €100M-€285M at any time
- A 5% improvement in reserve accuracy = €5M-€14M in freed capital or avoided losses
- For the carrier that lost €18M "because it rained a lot in December" [TRANSCRIPT: Feb 7, 2026], better reserve models would have smoothed this shock

[SOURCE: mysa_product_strategy.md, Part 2d; TRANSCRIPT: Feb 7, 2026; mysa_product_strategy.md, Part 9b — ROI calculation]

### Why This Matters for Mysa's Sales Motion

Most claims AI companies pitch to the VP Claims: "Your adjusters will be more productive." This sells to the operations budget.

Mysa should ALSO pitch to the CFO: "Your reserves will be more accurate." This sells to the finance budget — a completely separate buying center within the same carrier.

> Nobody else is framing their claims AI product in terms of reserve accuracy and P&L impact. [SOURCE: mysa_product_strategy.md, Part 2d — CLAUDE ANALYSIS]

The dual-buyer approach — VP Claims (productivity) + CFO (reserves) — strengthens the business case and creates multiple champions inside the carrier.

---

## 2.7 Garbage In, Garbage Out

### Fixing Intake Is a Prerequisite, Not the Product

> "I think what is wrong with companies, and I think our value is here, but you cannot start here. Because it's garbage in garbage out. So if you already have a lot of garbage in, you need to start by fixing that."
> — Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

> "Can you do the next steps without the step before being properly done? Garbage in, garbage out."
> — Jeremy Blehaut [TRANSCRIPT: Feb 7, 2026]

This is an architecturally important distinction: **Mysa's intake work (OCR, document parsing, data structuring) is a means, not an end.**

| Layer | What it is | Value alone | Value as pipeline |
|-------|-----------|-------------|-------------------|
| **Intake/Parsing** | Read documents, extract fields, structure data | Moderate — $1B+ of funded competitors do this already (Assured, FurtherAI, Avallon) | **Essential** — without clean data, the decision engine gets garbage |
| **Decision Engine** | Coverage, liability, reserves, fraud — the 6 judgment steps | **Very high** — nobody else does this. This is Mysa's value. | Requires clean data from the intake layer |

The competitive dynamic:
- If Mysa only does intake, we compete with $1B+ of funded companies
- If Mysa only does decisions on dirty data, the output is unreliable
- If Mysa does intake + decisions, we fix the data AND use it — the intake is the wedge, the decision is the moat

This is also a legal argument: decisions in claims are always subject to dispute, in both the EU and the US. Structured, well-documented decision-making (with traced data lineage from document to decision) creates stronger legal defensibility for the carrier.

> "This creates more of a legal power that is not legally binding Mysa, but allows them to have better structure for it."
> — Jeremy Blehaut [TRANSCRIPT: Feb 8, 2026]

[SOURCE: mysa_product_strategy.md, Part 2e; TRANSCRIPT: Feb 7, Feb 8, 2026]

---

## 2.8 Why Nobody Built the Decision Layer

### It Requires Both Deep Domain AND Modern AI — And That Combination Barely Exists

> "Because everyone is not focusing on solving problems. They are focusing on fundraising."
> — Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

> "I think this is just easier." (About why everyone builds intake instead of decisions)
> — Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

### The Five Structural Barriers

**1. Legacy system integration is brutal.**
74% of insurers still run some legacy technology. Guidewire, Duck Creek, Sapiens, mainframe systems — each integration is a 6-12 month project. CCC's own integration with Guidewire took years. Every insurer is different. Building a decision layer that works across carriers means integrating with all of them. [SOURCE: competitive_landscape_reality_check.md — "74% of insurers still run some legacy tech"]

**2. Regulatory fragmentation makes it hard to scale.**
In the US: 50 states, each with different claims handling rules, settlement timing requirements, and consumer protection laws. In the EU: country-by-country convention systems (IRSA, CARD, CIDE, IDS) plus GDPR plus per-country insurance regulators (ASF in Portugal, DGSFP in Spain, ACPR in France, IVASS in Italy). No one has built a universal decision layer because the rules differ everywhere. [SOURCE: competitive_landscape_reality_check.md; REGULATORY_COMPLIANCE.md]

**3. Incumbents defend their turf — aggressively.**
CCC sued Tractable for 5 years over anti-competitive behavior. Guidewire partners selectively. These are walled gardens, not open ecosystems. Building on top of incumbent platforms requires partnership agreements that can take 12-18 months to negotiate. [SOURCE: competitive_landscape_reality_check.md — "CCC sued Tractable for 5 years"]

**4. Adjusters resist change — badly deployed tools make things worse.**
"Enterprise-wide adoption is not plug-and-play — it requires thoughtful process redesign, adjuster upskilling, and robust change management." Tools that adjusters don't adopt are worthless. The current workforce skews older and is already overwhelmed by 5-7 systems. Adding a seventh or eighth system that doesn't reduce their workload increases resistance. [SOURCE: competitive_landscape_reality_check.md; TRANSCRIPT: Feb 7, 2026]

**5. The domain + AI combination barely exists.**
Building the decision layer requires understanding what adjusters actually decide and why (deep insurance domain expertise) AND building models that can reason about policies, evidence, and causation (modern AI engineering). Most startups have one or the other:

| Company Profile | Domain | AI | Result |
|----------------|--------|-----|--------|
| Insurance veterans starting a company | Deep | Shallow | Build what they know (CMS, workflow) — afraid to touch the judgment because they know how complex it is |
| AI engineers entering insurance | Shallow | Deep | Build what's easy (OCR, chatbots, intake) — don't understand the decision layer well enough to automate it |
| Large incumbents (Verisk, CCC) | Deep | Growing | Moving from data (estimation) toward judgment — but slowly, and US-only |
| **Mysa** | **Tiago's practitioner-level domain knowledge** | **Jeremy's working OCR + LLM system** | **Decision engine with carrier-specific SOP workflows** |

[SOURCE: mysa_product_strategy.md, Part 2f; competitive_landscape_reality_check.md; TRANSCRIPT: Feb 7, 2026]

### Why It's Possible NOW

Three things changed:

1. **LLMs can reason about policies.** For the first time, AI can read a 40-page insurance policy, understand coverage clauses and exclusions, and recommend whether a specific claim is covered. This was science fiction 3 years ago. It costs ~$6.50/month per 100 claims. [SOURCE: LLM_ARCHITECTURE.md — cost estimates]

2. **The workforce crisis creates urgency.** Carriers cannot wait for 12-month enterprise procurement cycles. Mid-market carriers (€100-200M GWP) have 1-2 decision-makers and need solutions now. The buying cycle is 3-6 months, not 18-24. [SOURCE: mysa_product_strategy.md, Part 3a]

3. **Agent-native architecture is viable.** Building a decision engine on top of hardcoded rules (the traditional approach) doesn't scale — every carrier has different SOPs, different rules, different templates. An agent-native architecture where "features are prompts, not code" and "rules live as knowledge, not code" means: new carrier = knowledge ingestion (hours), not code deployment (weeks). [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md — "Features are prompts, not code"]

> "We are just starting to be able to do this. But it's so many specks... items in the spectrum." — Tiago, on the complexity of encoding claims decisions [TRANSCRIPT: Feb 9, 2026]

---

## Sources

| Source | Type | Sections Used |
|--------|------|--------------|
| `mysa_product_strategy.md` Part 2 (2a-2f) | Primary — all problem data | 2.1-2.8 |
| `competitive_landscape_reality_check.md` | Primary — barriers to entry, competitive dynamics | 2.2, 2.8 |
| Feb 7 Granola call — Mid-market strategy | Transcript (summary) | 2.1, 2.3, 2.5, 2.6, 2.8 |
| Feb 8 Granola call — Strategy review | Transcript | 2.3, 2.5, 2.7 |
| Feb 9 Granola call — Claims workflow | Transcript | 2.1, 2.8 |
| Feb 5 Granola call — Workflow analysis | Summary | 2.4 (EU vs US) |
| `claims_journey_discovery.md` | Secondary — STP analysis, phase activities | 2.1, 2.4 |
| `AI_NATIVE_ARCHITECTURE_SPEC.md` | Secondary — architecture philosophy | 2.2, 2.8 |
| `LLM_ARCHITECTURE.md` | Secondary — cost estimates | 2.8 |
| `REGULATORY_COMPLIANCE.md` | Secondary — regulatory barriers | 2.8 |
| `caravela-ocr.md` (memory) | Internal — accuracy metrics | 2.4 |
