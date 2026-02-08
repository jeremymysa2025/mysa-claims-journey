# Mysa — Product Strategy Working Document

### Fundraising Preparation | Product Roadmap | Demo Specification

*Last updated: February 7, 2026*

**Sourcing convention:**
- `[TRANSCRIPT]` = verbatim quote from co-founder strategy call (Feb 2026)
- `[RESEARCH: filename]` = finding from discovery/competitive research documents
- `[AGENT RESEARCH]` = finding from competitive deep-dive research agents
- `[CLAUDE ANALYSIS]` = synthesis, inference, or strategic suggestion — clearly labeled
- `[WEB SOURCE]` = data from web search with URL

---

## Part 1: What Mysa Is

### One-Liner

**AI decision engine for insurance claims adjusters — the expert judgment layer between FNOL intake and estimation that nobody has built.**

### The Positioning Problem: CRM vs Decision Engine

The co-founder call surfaced this tension directly. Jeremy asked: *"So it's a CRM for adjusters?"*

The co-founder's response reframed it:

> [TRANSCRIPT — Co-founder]: "everyone is trying something... everyone is trying to build a platform... And everyone is avoiding the judgment, the decision stage."

> [TRANSCRIPT — Co-founder]: "I'm here to support the adjuster. To spend less amount of time on everything that doesn't require work. And when they get to the decision, I will help them with all the data that we have been collecting, and I will learn with him."

**Why "decision engine" wins over "CRM for adjusters":**

| Framing | What it implies | Who does this already | Problem |
|---------|----------------|----------------------|---------|
| CRM for adjusters | Data entry, case tracking, workflow | Five Sigma, Guidewire, VCA Software, ClaimPilot | Crowded, commoditized |
| Claims copilot | Surface-level AI suggestions on any task | Majesco Copilot, Microsoft Copilot for Insurance, Sedgwick Sidekick | Broad but shallow |
| **Decision engine** | The 6 expert judgment steps that consume 60-70% of adjuster time | **Nobody** | **Mysa's gap** |

[CLAUDE ANALYSIS]: The positioning should be "decision engine" — but the fundraising pitch needs to explain WHY this is different from a copilot. The distinction: a copilot helps you DO tasks faster. A decision engine helps you THINK through the judgment. It's the difference between autocomplete and a reasoning partner. Copilots speed up the keyboard. Decision engines speed up the brain.

---

### The 6 Decision Sub-Steps

This is the core product scope. The co-founder defined the framework:

> [TRANSCRIPT — Co-founder]: "the decision is breaking basically breaking down in six different categories. You have coverage. You have checking the policy reports. You need to check the repairs. You need to check how much it costs. You need to check... how much money you are reserving... does it have fraud? There are, like, six steps. That's the judgment."

| # | Decision Step | What the adjuster does today | What Mysa does | Time saved |
|---|--------------|------------------------------|----------------|------------|
| 1 | **Coverage verification** | Manually reads policy document, cross-references claim facts against coverage clauses and exclusions | AI reads policy, matches claim facts, highlights applicable coverage and exclusions with confidence score | 15-30 min → 2 min review |
| 2 | **Policy report checking** | Checks if documentation is complete, facts are consistent, nothing is missing or contradictory | AI validates completeness, flags gaps, identifies contradictions, drafts follow-up requests | 10-20 min → 1 min review |
| 3 | **Repair assessment** | Reviews proposed repair scope, checks if it's reasonable, looks for missing or over-scoped items | AI compares scope against comparable claims, flags anomalies, checks against carrier guidelines | 15-25 min → 3 min review |
| 4 | **Cost analysis** | Compares repair cost estimate against market rates, historical claims, and carrier pricing databases | AI pulls comparable data, identifies outliers, calculates expected range | 10-20 min → 2 min review |
| 5 | **Reserve calculation** | Estimates total claim cost for financial reporting — this hits P&L immediately | AI calculates reserve with confidence interval based on historical data, comparable claims, and claim trajectory | 10-15 min → 1 min review |
| 6 | **Fraud detection** | Looks for red flags — inconsistencies, patterns, known fraud indicators | AI pattern-matches against fraud signals, scores risk, recommends SIU referral if flagged | 5-10 min → automated flagging |

**Total adjuster time on decisions today:** 65-120 min per claim
**With Mysa:** 10-15 min review per claim
**Productivity gain:** 4-8x on the decision step alone

[CLAUDE ANALYSIS]: These time estimates are my inference based on the transcript discussion ("60-70% of time on decisions") and the per-adjuster economics from our research (300-480 claims closed/year, ~125 open). They need validation with actual adjusters at Caravela.

---

### SOP-Driven Workflow Generation

This is the core differentiator vs. Five Sigma and every other claims AI tool.

> [TRANSCRIPT — Co-founder]: "everything that we build, needs to be really around SOP, like, what is the SOP that your insurance company or your TPA follows for that."

> [TRANSCRIPT — Co-founder]: "when we onboard an insurance company, we upload the SOPs, and we also translate those SOPs into workflows. And you can also go there and manually create more workflows."

> [TRANSCRIPT — Co-founder]: "Ideally, you upload the SOPs, or you tell to AI what's the SOP, and their workflow is automatically built."

**How it works:**

```
ONBOARDING:
Carrier uploads SOPs (PDF, Word, scanned docs)
  → Mysa OCR extracts rules, thresholds, escalation paths
  → AI generates structured decision workflows
  → Carrier reviews and adjusts
  → Workflows go live

PER CLAIM:
Claim data arrives
  → Mysa matches claim type to relevant SOP workflows
  → AI walks adjuster through each decision step per carrier's own rules
  → Documents generated per carrier's templates and requirements
  → Decisions checked against SOP compliance
```

[CLAUDE ANALYSIS]: This is a genuine differentiator. Five Sigma's Clive uses general insurance knowledge — their "playbooks" are pre-defined templates per claim type. Mysa would use the SPECIFIC carrier's SOPs to generate decision workflows. This means:
1. Recommendations are tailored per-carrier, not generic
2. New hires can follow carrier-specific processes from Day 1 (addresses workforce crisis)
3. Creates switching costs — once SOPs are encoded, the carrier is locked in
4. Compliance is built-in — every decision is checked against the carrier's own rules

**Playbooks** — the co-founder acknowledged Five Sigma got this right:

> [TRANSCRIPT — Co-founder]: "the adjuster should be something similar to they call it, playbooks. That's a smart one. Damn it. That's very smart. Let's replicate that."

[AGENT RESEARCH — Five Sigma]: Five Sigma's playbooks are pre-defined investigation workflows per claim type. Mysa's version must go deeper: SOP-driven playbooks that adapt per carrier, per claim type, per complexity score — not generic templates.

---

### What Mysa Does vs. What Mysa Does NOT Do

| Layer | Mysa's role | Who already does this | Our relationship |
|-------|-------------|----------------------|-----------------|
| FNOL / Intake | Does NOT replace — works on top of existing intake | Assured ($1B), Avallon ($4.6M), FurtherAI ($30M) | Integrate with, not compete |
| Document parsing | **YES** — parses emails, claims docs, policies, EAS forms | Caravela OCR engine (existing asset, ~80% accuracy) | Core capability |
| Triage | **YES** — complexity scoring, desk vs field, priority, SOP-driven routing | Some overlap with ClaimSorted, Five Sigma | Better because SOP-driven |
| Investigation support | **YES** — scopes investigation, guides calls, records, generates docs | **Nobody does this well** | Core product |
| Assessment/Estimation | Does NOT estimate — integrates with estimation tools | Verisk/Xactimate (US), Solera/Audatex (EU) | Must integrate |
| Decision support | **YES — PRIMARY VALUE** — the 6 sub-steps | **NOBODY** | **Our gap** |
| Document generation | **YES** — generates all decision documents per SOP | Core product | Core capability |
| Payment processing | No | Carrier's own systems | Not our layer |

> [TRANSCRIPT — Co-founder]: "I don't care about [intake]. Just do intake very well, and I don't change how they are doing intake. I just help them doing the intake that they are already doing."

> [TRANSCRIPT — Co-founder]: "I am basically using an extractor... I'm basically if missing data, I'll go back to the user."

---

### The Historical Data Engine (Long-Term Moat)

> [TRANSCRIPT — Co-founder]: "If you have the historical data, then you can start... give you already an overview of everything that happened so far. And what we think will happen based on historical data, the SOPs, and the documents uploaded so far. So you don't need to review again everything. We already start from a clean point."

> [TRANSCRIPT — Jeremy]: "the real product is... based on historical data."

> [TRANSCRIPT — Co-founder]: "When we come in and we use the historical data, and the out-of-the-box thing, we get 60%. As soon as we start getting better data and training the models, we go to 70 or 80%."

**The flywheel:**

```
Day 1: SOP workflows + document parsing → basic recommendations
  ↓
Month 3: Historical claims data ingested → better comparable matching
  ↓
Month 6: Decision ground truth captured (adjuster accepts/modifies/rejects) → model learns
  ↓
Month 12: Enough data to predict outcomes → proactive recommendations
  ↓
Month 18+: Models can handle routine decisions with minimal review → near-STP
```

[CLAUDE ANALYSIS]: The moat is decision ground truth data. Every competitor has claim OUTCOMES (what was paid). Nobody has decision REASONING (why the adjuster decided what they decided). As the co-founder articulated: "you see the end result... but you don't know exactly how they got to that end result." Mysa captures the HOW — and that's the training data nobody else has.

> [TRANSCRIPT — Co-founder]: "Claude gave me this example. When you go to a restaurant, you see the end result. You see what you order and the end result. That's a claim. That's what they get. They don't know exactly how they got to that end result."

---

## Part 2: The Problem — Why This Exists

### 2a. The Workforce Crisis

The insurance claims adjuster profession is dying. This isn't hyperbole — it's the primary market driver.

> [TRANSCRIPT — Jeremy]: "They're all boomers... their work output is super bad. Because they work like boomers. They are not digital native. So they cannot interact with very old tech properly, and they can surely not interact with new tech."

> [TRANSCRIPT — Jeremy]: "the turnover of those people is so high... the newcomers, they are fighting to get them in The US. Meaning it's like the champions league. They're trying to get the Cristiano Ronaldo."

> [TRANSCRIPT — Co-founder]: "25% of all claims adjusters predicted to retire within five years."

**Hard data:**

| Metric | Data | Source |
|--------|------|--------|
| Profession ranking | 12th fastest-declining by 2030 | [RESEARCH: competitive_landscape_reality_check.md] — BLS data |
| Retirement wave | 50% of insurance workforce retiring in 15 years | [RESEARCH: Section 6] |
| Near-term retirement | 25% of adjusters within 5 years | [RESEARCH: Section 6] + [TRANSCRIPT] |
| Annual attrition | 20% at carriers, 33% at TPAs | [RESEARCH: Section 6] |
| Knowledge loss per departure | ~6 years institutional knowledge | [RESEARCH: Section 6] |
| Impact of high turnover | 12% higher operational costs, 20% higher indemnity payouts | [RESEARCH: Section 6] |
| Fully loaded cost per adjuster | ~$110K/year | [RESEARCH: Section 6] + [TRANSCRIPT: "$110k for the ones that spend six years"] |
| Caseload | ~125 open claims, 300-480 closed/year | [RESEARCH: Section 6] |
| Cost per closed claim | $230-$370 | [RESEARCH: Section 6] |

> [TRANSCRIPT — Jeremy]: "the worst part is... they're all going for retirement. This is a job that is requiring people. They have high turnover, high attrition. They are not able to lock new generations into this job."

**Why this matters for Mysa:** Carriers can't hire enough adjusters. They can't train new ones fast enough (6 years to develop expertise). They need technology that makes existing adjusters handle more claims AND makes new adjusters effective faster. That's exactly what SOP-driven decision support does.

---

### 2b. The STP Reality Gap (EU Motor)

[RESEARCH: claims_journey_discovery.md, Phase 3]: EU convention systems promise 60-70% STP for motor claims. Actual STP is ~10%. The gap is 50+ percentage points.

> [TRANSCRIPT — Co-founder]: "Our north star is improving the STP... basically the amount of [claims] automatically [processed]... it takes seconds. It's like someone just reviewing it."

> [TRANSCRIPT — Jeremy]: "But that's impossible in Europe. You're not allowed to automatically approve a claim."

> [TRANSCRIPT — Co-founder]: "No. It is. They just get automatically approved in the sense it's not automated, but it takes seconds."

**Why the gap exists:**
[RESEARCH: claims_journey_discovery.md]: The convention lookup itself is trivial — it's a database query matching checkboxes to fault percentages. The bottleneck is DATA QUALITY:
- ~50% of EAS forms are still paper
- Filled out by stressed people with shaking hands at accident scenes
- Messy diagrams, unclear checkboxes, missing fields
- Manual data entry introduces errors

**The opportunity:** Whoever fixes data quality upstream unlocks the 50+ point STP gap. Mysa's EAS digitization (OCR + document understanding) is the key that unlocks the convention system.

---

### 2c. Adjuster Productivity Drain

> [TRANSCRIPT — Co-founder]: "the work of an adjuster, 30 to 40%, is data entry and admin. Manual reads papers. Types into the CMS, more than 20 phone calls, context switching between five to seven systems."

[RESEARCH: Section 7]: Today, an adjuster uses 5-6 separate systems per claim:
```
Xactimate (estimation) + Hover/EagleView (measurements) +
CMS (VCA/Guidewire/JURIS) + n2uitive (recorded statements) +
Encircle/BuildArray (field docs) + carrier portal (reporting)
```

**The productivity math:**

| Activity | % of adjuster time | Automate? |
|----------|-------------------|-----------|
| Data entry & admin | 30-40% | YES — document parsing, auto-population |
| Travel (field inspections) | 25-30% | Partial — desk vs field triage |
| Documentation | 20-25% | YES — document generation per SOP |
| Actual decision-making | 10-20% | Augmented — the 6 sub-steps |
| Phone calls / context switching | 10-15% | YES — call recording, guided scripts |

[RESEARCH: Section 6] — The 3x productivity math:
- Current: ~300-480 claims closed/year per adjuster
- At 3x: 900-1,440 claims closed/year
- Cost per claim drops from $230-$370 to $75-$125
- **Savings: $45-120K/year per adjuster**

For a mid-tier TPA with 200 property adjusters: saves **$9-24M/year**.

---

### 2d. Reserve Accuracy = Direct P&L Impact

This is the selling point that should be front-and-center with CFOs.

> [TRANSCRIPT — Co-founder]: "Do you know this concept? It's not what they are paying that matters. It's how much money they are reserving. Because reserves are already recognized in the P&L right away."

> [TRANSCRIPT — Jeremy]: "So they're losses right away."

> [TRANSCRIPT — Co-founder]: "And there is no rules... but they will hold you accountable if the reserve is too different from the value that you end up paying."

**Why this matters:**
- Over-reserve → looks less profitable → lower stock price / investor confidence
- Under-reserve → regulatory action → potential solvency issues
- Accurate reserves → financial predictability → better reinsurance rates

> [TRANSCRIPT — Co-founder]: "Caravela... they lost 18 million last year or two years ago. Do you know why? Because it rained a lot in December. And they were very bad at selling their own policies."

[CLAUDE ANALYSIS]: This is a CRITICAL selling point. Most claims AI companies pitch "adjuster productivity" (saves the VP Claims budget). Mysa should ALSO pitch "reserve accuracy" (saves the CFO's P&L). This opens a second buyer within the same organization and creates a stronger business case. Nobody else is framing their product this way.

---

### 2e. The "Garbage In, Garbage Out" Problem

> [TRANSCRIPT — Jeremy]: "Can you do the next steps without the step before being properly done? Garbage in, garbage out."

> [TRANSCRIPT — Co-founder]: "No. You can't because you need to have a claim open and you need to have a reserve already."

> [TRANSCRIPT — Co-founder]: "I think what is wrong with companies, and I think our value is here, but you cannot start here. Because it's garbage in garbage out. So if you already have a lot of garbage in, you need to start by fixing that."

[CLAUDE ANALYSIS]: This is why Mysa needs to handle BOTH document parsing/structuring AND the decision layer. You can't build a decision engine on garbage data. The product does intake cleanup NOT as the value proposition but as the DATA PIPELINE that feeds the real value (decisions). This is architecturally important: Mysa's intake work is a means, not an end.

---

### 2f. Why Nobody Has Built the Decision Layer

> [TRANSCRIPT — Co-founder]: "Because everyone is not focusing on solving problems. They are focusing on fundraising."

> [TRANSCRIPT — Co-founder]: "I think this is just easier." (About why everyone builds intake instead of decisions)

[RESEARCH: competitive_landscape_reality_check.md]:
1. **Legacy system integration is brutal** — 74% of insurers still run some legacy tech. Each integration is 6-12 months.
2. **Regulatory fragmentation** — 50 US states with different rules. EU is country-by-country.
3. **Incumbents defend turf** — CCC sued Tractable for 5 years over anti-competitive behavior.
4. **Adjusters resist change** — "enterprise-wide adoption is not plug-and-play."
5. **TAM is fragmented** — buyers scattered across carriers, TPAs, MGAs of all sizes.

[CLAUDE ANALYSIS]: The real reason: building the decision layer requires BOTH deep insurance domain expertise (understanding what adjusters actually decide and why) AND technical AI capability (models that can reason about policies, evidence, and causation). Most startups have engineering talent or insurance talent, rarely both. Mysa's advantage: co-founder's insurance domain knowledge + existing Caravela OCR engine for document processing.

---

## Part 3: The Market — Sized for Mid-to-Small

### 3a. Why Mid-to-Small, Not Enterprise

> [TRANSCRIPT — Co-founder]: "I always think about insurance companies as companies that have a data science team. But I think you are right." (After Jeremy pointed out mid-to-small don't have dev teams)

> [TRANSCRIPT — Jeremy]: "for the mid-market ones like Caravela, they want us."

> [TRANSCRIPT — Jeremy]: "for big carriers, it will be 'don't touch this. It's my turf. It's my logic. Build our own.'"

[RESEARCH: competitive_landscape_reality_check.md]: "Allianz launched 'Insurance Copilot' in Austria in 2024... Key insight: Allianz built it in-house for themselves, not as a product for other insurers. That's the pattern with the big carriers."

**The segmentation — anchored to Caravela (€188M GWP, 149 employees, 57K claims/year, 7th in Portuguese non-life):**

[WEB SOURCE: Caravela 2024 Annual Report, ECO rankings, ASF data]

| Segment | Size (GWP) | EU Count (4 countries) | Tech approach | Mysa addressable? | Reference carriers |
|---------|-----------|----------------------|---------------|-------------------|-------------------|
| Enterprise | >€1B | ~16-18 groups | Build in-house | NO — Allianz, AXA, Generali, UnipolSai, Covéa all building own | Fidelidade (PT), Mapfre (ES), Covéa (FR), UnipolSai (IT) |
| Large | €200M-€1B | ~24-40 carriers | Buy best-of-breed or outsource to TPA | YES — but longer sales cycles | Zurich PT, Linea Directa (ES), Matmut (FR), Vittoria (IT) |
| **Caravela tier** | **€100M-€200M** | **~30-50 carriers** | **Need it, can't build it, ~100-200 employees** | **PRIMARY TARGET — sweet spot** | **Caravela (PT), Pelayo (ES), Thélem (FR), HDI Italy** |
| Small | €50M-€100M | ~40-60 carriers | Want tech help, tight budget, <100 employees | YES — entry-level pricing | UNA (PT), Patria Hispana (ES), small mutuelles (FR) |
| Micro | <€50M | ~170-255+ entities | Manual processes, minimal tech, <50 employees | LONG-TAIL — self-serve/per-claim | Regional mutuals, niche writers, many French mutuelles |

**Why "Caravela tier" (€100-200M) is the sweet spot:**
- Big enough to have real claims volume (~30K-60K/year) that justifies the investment
- Small enough to lack a data science team or in-house AI capability
- Growing fast (Caravela grew 10x in 10 years) — need tools to scale without proportional headcount
- Budget exists: €50K-200K/year is 0.03-0.2% of GWP — trivial if it improves STP or reserve accuracy
- Decision-making is fast: 1-2 decision-makers, not a 12-month procurement process

[CLAUDE ANALYSIS]: The previous segmentation used vague EU-wide estimates. Now validated with actual carrier data per country: the "Caravela tier" (€100-200M GWP) has ~30-50 carriers across just 4 Southern EU countries. Add smaller carriers (€50-100M) and you get ~70-110 carriers. Add Northern EU (Germany, Benelux, Nordics) and the total addressable universe of sub-€200M carriers is likely 200-400+ across Europe. This is more than enough for a focused startup.

> [TRANSCRIPT — Co-founder]: "My girlfriend [at BCP] also has a Copilot in-house... I also know how the Copilot for the BCP works. It's very bad."

[CLAUDE ANALYSIS]: Even the large carriers that build in-house are building BAD copilots. The co-founder's direct observation: internal tools are document retrieval, not decision support. Mysa could eventually sell to large carriers as "better than what you built internally" — but that's Phase 3, not Phase 1.

---

### 3b. Total Market Sizing

[RESEARCH: home_property_competitive_deep_dive.md, Section 18 + AGENT RESEARCH: full EU 16-country + US carrier distribution validated]

**US Market:**
| Segment | Count | Revenue/Premium | Concentration |
|---------|-------|----------------|--------------|
| P&C Carriers | ~4,116 entities | $1.06T DWP | Top 10 = 51.4%, Top 100 = ~90% |
| Caravela-comparable ($100-500M) | ~200-350 carriers | — | Buy-not-build segment |
| TPAs (P&C, material size) | ~500-800 | $115B market | Growing as carriers outsource |
| MGAs with claims authority | ~330-550 | $114B managed premium (16% CAGR) | Emerging claims buyer |
| Independent adjusting firms | ~53,000 businesses | $11.7B market | Workforce augmentation |
| **Total claims/year** | **~45-50M** | **$632B losses + LAE** | |

**EU Market (16 countries validated):**
| Segment | Count | Revenue/Premium | Key Data |
|---------|-------|----------------|----------|
| Total insurers | ~2,141+ undertakings | ~€400-450B GWP (all lines) | 16 countries mapped |
| Motor GWP | — | **~€128-136B** | Southern €57.9B + Northern €70-78B |
| Caravela tier (€100-200M) | **~96-165 carriers** | — | Primary target across 16 countries |
| Small tier (€50-100M) | ~204-260+ | — | Entry-level pricing |
| MGAs | 650+ | €18B GWP (23% CAGR) | Growing fast in EU |
| **Total claims/year** | **~55-70M** | **~€300-350B claims paid** | |

**Combined addressable:**
- ~1,530-2,400 potential buyer companies (EU carriers + US carriers + TPAs + MGAs)
- ~100-120M claims/year across both markets
- €200-650M TAM (initial sale), €400M-1.3B with land-and-expand
- **Market is 90-95% open** in EU mid-market, 75-85% open in US mid-market (only 4% of insurers have scaled claims AI)

---

### 3c. First Attack: EU Motor — Caravela-Sized and Below

**Anchor: Caravela Seguros** — €188M GWP (2024), 149 employees, 57K claims/year (42K motor), 7th in Portuguese non-life.

[WEB SOURCE: Caravela 2024 Annual Report; ASF; ECO Sapo rankings; MAPFRE Economics; France Assureurs; IVASS/ANIA. Full source list in agent research.]

#### Country-Level Market Overview

| Country | Convention | Motor GWP | Vehicles | Total Insurers | Motor Writers |
|---------|-----------|----------|----------|---------------|--------------|
| **Portugal** | IDS/CIMPAS | **~€1.8B** (2023) | ~5.8M light (7.3M total) | 47 active non-life (63 domestic) | ~25-30 |
| **Spain** | CIDE/ASCIDE/CICOS | **€13.2B** (2024, +8.9%) | **34M** | 176 operating (187 RAEA) | ~80-100 (31 groups in motor) |
| **France** | IRSA | **€28.1B** (2024, +7.3%) | **45.5M** | **660 ACPR-supervised** (246 FFA) | ~100-120 |
| **Italy** | CARD | **~€14.8B** (2023) | **~40M** | ~85 national (IVASS) | **38 write RC Auto** |

#### Carrier Distribution by Size Tier (validated, per country)

| Size Tier (total GWP) | Portugal | Spain | France | Italy | **4-Country Total** |
|-----------------------|----------|-------|--------|-------|-------------------|
| **>€1B** (enterprise — builds in-house) | 3 | 5-6 | 5-7 | 3 | **~16-19** |
| **€200M-€1B** (large — buys best-of-breed) | 4-5 | 8-10 | 10-20 | 8-12 | **~30-47** |
| **€100-200M** (Caravela tier — **PRIMARY TARGET**) | 6-8 | 8-10 | 30-60 | 10-15 | **~54-93** |
| **€50-100M** (small — entry-level) | ~8-12 | ~25-35 | ~100+ | ~8-12 | **~141-159+** |
| **<€50M** (micro — long-tail) | ~25-30 | ~110-130 | ~100-200+ | ~8-12 | **~243-372+** |

[WEB SOURCE: Portugal — ECO/ASF rankings, top 10 = 92% of market. Spain — DGSFP sector report, 176 operating entities. France — ACPR data, 660 organizations (324 mutuelles + 302 insurance code + 34 social security code), ACPR 1st quartile cutoff = €82M. Italy — IVASS, only 38 companies write RC Auto. EIOPA — ~300 of ~2,300 Solvency II entities qualify as SNCU (<€100M GWP, ~13%)]

#### Caravela-Tier Deep Dive: Named Carriers (€100-200M range)

| Country | Carrier | Est. GWP | Notes |
|---------|---------|----------|-------|
| **Portugal** | **Caravela** | €188M (2024) | Design partner. 7th non-life. 42K motor claims. |
| Portugal | CA Seguros | ~€200-210M | 8th, displaced by Caravela |
| Portugal | Mapfre PT | ~€190-210M | 9th, surge with Bankinter |
| Portugal | Aegon Santander | ~€170-190M | 10th, health +37.5% |
| Portugal | Victoria | ~€130-150M | 11th, strong in health |
| Portugal | UNA | ~€120-140M | 12th, health +53%, motor +26% |
| **Spain** | Pelayo | ~€375M (mutua) | 844K auto policies, 2.42% motor share |
| Spain | Admiral/Balumba | ~€100-150M motor | UK-owned direct writer, +13.4% |
| Spain | Patria Hispana | ~€100-130M | Centennial company, +12.9% |
| Spain | Mutua Tinerfeña | ~€80-120M | Regional Canary Islands mutual |
| **France** | Thélem Assurances | €453M total | ~€150-200M motor. 1.15M contracts. **Closest French analog to Caravela.** |
| France | L'Olivier Assurance | ~€220-260M | Online auto pure-play. Similar to Caravela. |
| France | Direct Assurance (AXA sub) | ~€300-400M | Slightly larger than Caravela |
| France | ~30-60 small mutuelles | €82-200M each | ACPR 2nd quartile. Many are autonomous, multi-line with motor books. |
| **Italy** | HDI Assicurazioni | €716M non-life, ~€160-200M motor | R.C. Auto = 22.8% of non-life. **Closest Italian analog to Caravela.** |
| Italy | ~10-12 smaller carriers | €50-200M motor | Regional companies, online insurers (Prima, Quixa, Verti, Linear) |

#### TAM Calculation — Caravela-Anchored

**Tier 1: Caravela tier (€100-200M GWP) — Primary target:**
- ~54-93 carriers across 4 Southern EU countries
- Average claims/year per carrier (Caravela reference): ~40-60K
- Average motor claims: ~30-45K
- ACV at €50K-200K/year: **€2.7M-€18.6M**
- Per-claim at €2-5/claim: **€3.2M-€20.9M**

**Tier 2: Small carriers (€50-100M GWP) — Entry-level:**
- ~141-159+ carriers across 4 countries
- Average claims/year (estimated): ~15-30K
- ACV at €30K-€100K/year: **€4.2M-€15.9M**
- Per-claim at €3-5/claim: **€6.3M-€23.9M**

**Tier 3: Large carriers (€200M-€1B GWP) — Expansion:**
- ~30-47 carriers across 4 countries
- ACV at €200K-€500K/year: **€6M-€23.5M**

**Tier 4: Micro (<€50M GWP) — Long-tail, self-serve:**
- ~243-372+ entities (many are French mutuelles)
- Not all write motor. Realistic motor writers: ~100-150
- ACV at €10K-€30K/year or per-claim only: **€1M-€4.5M**

**Combined TAM (4 Southern EU countries only):**

| Scenario | Carriers Reached | Revenue |
|----------|-----------------|---------|
| **Conservative** (Caravela tier only, low ACV) | ~54 carriers | **~€2.7M** |
| **Base case** (Caravela + small tiers, mid ACV) | ~195 carriers | **~€15-25M** |
| **Optimistic** (all tiers incl. large + micro, high ACV) | ~468+ carriers | **~€45-80M** |
| **Full EU** (add Germany, Benelux, Nordics, CEE) | ~700-1,000+ | **~€70-150M** |
| **EU + US expansion** (add US mid-market) | ~2,000+ | **~€200-650M** |

[CLAUDE ANALYSIS]: The honest answer: the Southern EU motor market alone is **NOT a venture-scale TAM**. At base case (~€15-25M), it's a healthy SaaS business but not a $1B+ outcome. The venture story requires: (1) expanding to all of EU including Northern markets, (2) expanding to US, (3) expanding from motor to property, and (4) moving up-market over time. EU motor is the **wedge**, not the company. This is consistent with the co-founder's own observation: "cars in Europe... you don't have a company."

**But as a wedge, it's perfect:**
- 54-93 carriers in the primary tier = reachable with 2-3 sales reps
- Caravela as design partner proves the product in a live environment
- Convention system expertise creates defensible moat
- Every carrier added builds the historical data flywheel
- Technology transfers directly to property and US markets

> [TRANSCRIPT — Jeremy]: "It's like 700 mid-market players in Europe. That makes less than 500 million of... insurance, like Caravela style."

**Why Portugal first:**
1. Co-founder network — Caravela is the design partner
2. IDS/CIMPAS system has 91% agreement rate — best-performing convention system
3. Smallest market = fastest to prove (fewer edge cases, tighter feedback loop)
4. Portuguese EAS forms are standardized and well-documented

> [TRANSCRIPT — Jeremy]: "I want an LOI [from Caravela], and we say we're doing it in free beta tester. For six months. This is the cost."

---

### 3d. Expansion Markets

**US mid-market property** (Phase 4, months 10-12):
[AGENT RESEARCH — NAIC, AM Best, Conning, IBIS World validated]:
- ~200-350 Caravela-comparable carriers ($100-500M DWP) — buy-not-build segment
- ~500-800 P&C-focused TPAs of material size — process claims for carriers, need efficiency tools
- ~330-550 MGAs with claims authority — fastest-growing buyer segment (16% CAGR)
- US homeowners ($173B) is less concentrated than auto ($359B, top 5 = 63.6%) — more mid-market opportunity
- US auto mid-market is tough: GEICO/Progressive/State Farm dominate. Target property first in US.
- [RESEARCH: Section 6]: "Mid-tier TPAs buy rather than build. They have budget pressure (adjuster shortage, leakage, turnover)."

**Northern/Central EU motor** (Phase 2 expansion, months 4-9):
[AGENT RESEARCH — BaFin, DNB, FSMA, FMA, FINMA, FI, FSA validated]:
- ~42-72 Caravela-tier carriers across 12 countries (Germany = 15-25, largest segment)
- ~63-101 small-tier carriers (€50-100M)
- Germany (~€30B motor) is the single largest EU motor market — but more concentrated than Southern EU
- Belgium (RDR convention), Netherlands (DSA — new 2024), Sweden (Trafikskadenämnden) have convention-like systems — partial wedge opportunity
- Austria, Switzerland, Ireland, Denmark, Norway, Czech Republic have no formal convention — less wedge, more general decision engine sell

**EU property** (Phase 3-4):
- ~250-400 mid-market carriers across EU
- No convention system advantage — same problem as US
- Sell to carriers directly (EU has minimal TPA market for property)

---

### 3e. Pricing Model

> [TRANSCRIPT — Jeremy]: "100% we can get from the tiniest 50k a year for this. And for the biggest 1,000,000."

[RESEARCH: Section 6]: Per-claim pricing ($50-200/claim) preferred by TPAs. Typical ACV $500K-$2M for mid-tier.

**Proposed pricing tiers (anchored to Caravela economics):**

Caravela reference: €188M GWP, ~57K claims/year. At €100K/year = 0.05% of GWP. At €3/claim = €171K/year = 0.09% of GWP. Both are trivial relative to the potential savings (€562K-€750K/year from STP improvement alone — see Part 6c).

| Tier | Target | # Carriers (4 countries) | Annual Contract | Per-Claim | Est. Claims/Year |
|------|--------|-------------------------|----------------|-----------|-----------------|
| Micro | <€50M GWP | ~100-150 motor writers | €10K-€30K/year | €5-8/claim | ~5-15K |
| Starter | €50-100M GWP | ~141-159 | €30K-€100K/year | €3-5/claim | ~15-30K |
| **Professional** | **€100-200M GWP (Caravela tier)** | **~54-93** | **€50K-€200K/year** | **€2-4/claim** | **~30-60K** |
| Growth | €200M-€500M GWP | ~20-30 | €200K-€500K/year | €2-3/claim | ~60-150K |
| Enterprise | €500M-€1B GWP | ~10-17 | €500K-€2M/year | Custom | ~150K+ |
| Design Partner | Caravela (beta) | 1 | Free 6 months → €50K-€100K/year | N/A | ~57K |

[CLAUDE ANALYSIS]: Per-claim pricing is better for landing new customers (low barrier, pay-as-you-go). Platform pricing is better for revenue predictability. Offer both and let the carrier choose. Most will start per-claim and migrate to platform as they scale.

---

## Part 4: Competitor Deep Dive — Head-to-Head

### 4a. Five Sigma / Clive — The Closest Competitor

> [TRANSCRIPT — Co-founder]: "I also care a lot about them [Five Sigma]. For me, they are still my main competitor, and I'm trying to find ways to win."

> [TRANSCRIPT — Jeremy]: "But I think they're everywhere and nowhere at the same time."

[AGENT RESEARCH — Five Sigma deep dive, 10-dimension analysis]:

**What they are:**
- **Revenue**: $10.1M (180% YoY growth) — growing fast but still small
- **Tech**: Gemini-based multi-agent system (same LLM backbone Mysa would use)
- **Integration**: REST API on any CMS — proven this approach works
- **Product**: Clive is 6 specialized AI agents:
  1. Communication agent — drafts emails, correspondence
  2. Investigation agent — guides investigation steps
  3. Evaluation agent — coverage matching, liability assessment
  4. Compliance agent — regulatory checks
  5. Knowledge agent — searches claim history, policy database
  6. Management agent — workflow orchestration

- **Traction**: Starr Insurance partnership (Jan 2026), "70% US, 30% EU"
- **Playbooks**: Pre-defined investigation workflows per claim type

**Five Sigma's confirmed GAPS:**

| Gap | Detail | Mysa's advantage |
|-----|--------|-----------------|
| No property-specific features | No Xactimate integration, no scope-of-loss, no contractor coordination | Mysa will integrate with Xactimate (US) |
| No EU convention systems | Cannot match EAS data against IRSA/CARD/CIDE/IDS | Mysa builds this as core wedge product |
| Generic playbooks | Pre-defined templates, not carrier-specific | Mysa uses carrier SOPs → tailored workflows |
| LLM coverage matching is fragile | Uses LLM to read policies — breaks on complex exclusions, nested clauses | Mysa supplements LLM with structured rules + SOP compliance |
| No causation analysis | Cannot determine "sudden vs gradual" for property | Mysa builds this for Thesis 3 |
| Limited EU presence | 30% of business, US-first | Mysa is EU-first |
| No P&L-aware reserve setting | Basic reserve suggestions | Mysa frames reserves as P&L impact — CFO-level selling point |
| No decision ground truth capture | Doesn't systematically capture WHY adjusters decide | Mysa's core moat is decision reasoning data |

---

### 4b. Verisk / XactAI — The Existential Long-Term Risk

> [TRANSCRIPT — Co-founder]: "How can we integrate with them? I want this integrated with them." (About Xactimate)

[AGENT RESEARCH — Verisk deep dive]:

**What they have:**
- 75-80% US property estimation market share via Xactimate
- Every Xactimate estimate ever written — massive data moat
- XactAnalysis (workflow), XactContents (contents valuation), Hover integration
- Revenue: Verisk is a $35B+ market cap public company

**XactAI (launched Sept 2025):**
- Photo labels and transcription — admin features ONLY
- Bundled FREE with Xactimate subscription — genius distribution
- NO decision support built yet: no coverage analysis, no reserve recommendation, no investigation scoping

**Why Mysa has time (for now):**

| Factor | Assessment |
|--------|-----------|
| Strategic DNA | Verisk is an estimation + data analytics company, NOT a decision support company |
| Buyer mismatch | XactAI buyer = CTO/IT (platform). Decision engine buyer = VP Claims. Different budgets, different champions. |
| Current XactAI scope | Admin automation (faster data entry), not expert judgment |
| Domain expertise gap | Building real decision AI requires insurance adjusting expertise they don't have |
| Timeline | 2-3 years before meaningful decision support — Mysa needs to establish by then |

**The risk — why this is existential:**
If Verisk decides to build coverage analysis on top of their estimation data, they have:
- Every property claim estimate ever written
- Regional pricing databases
- Carrier relationships (75-80% market share means every carrier already pays them)
- Free distribution (bundle with Xactimate like they did with XactAI)

[CLAUDE ANALYSIS]: Verisk is the biggest LONG-TERM risk but NOT an immediate competitor. The EU-first strategy buys time — Verisk has minimal EU presence. By the time Verisk builds decision AI (if they do), Mysa needs to have the decision ground truth data moat established. The co-founder's instinct to INTEGRATE with Xactimate is correct — in the US, you want to be the decision layer that feeds INTO Xactimate, not competes with it.

---

### 4c. Shift Technology — The EU Danger

[AGENT RESEARCH — Shift Technology deep dive]:

**What they have:**
- $320M raised — by far the best-funded EU claims AI company
- 25+ countries, 100+ customers
- Core DNA: Fraud detection (original product, 7+ years of data)
- Shift Claims (launched Sept 2025): Agentic AI for full claims workflow
- AXA Switzerland: 60% automation rate — impressive headline but details thin

**Shift Technology GAPS:**

| Gap | Detail |
|-----|--------|
| Starts downstream | Automates workflow AROUND decisions, not the decisions themselves |
| Fraud-first architecture | AI optimized for pattern matching, not judgment reasoning |
| No convention matching | Doesn't process EAS → convention system → fault determination |
| No SOP-driven workflows | Limited workflow customization |
| "60% automation" is misleading | Likely means 60% of TASKS automated, not 60% of DECISIONS |

[CLAUDE ANALYSIS]: The key distinction: **Shift automates the workflow. Mysa automates the judgment.** These are different layers. Shift makes the process flow faster. Mysa makes the decisions better. But Shift has the EU relationships and capital to build into the decision space. Speed matters — Mysa needs to establish the convention system / SOP workflow moat before Shift expands there.

---

### 4d. Secondary Competitors

| Company | Funding | What they do | Why not a direct threat | Transcript quote |
|---------|---------|-------------|------------------------|-----------------|
| **Assured** | $1B valuation | FNOL + messaging AI agent "Emma" | Intake-focused, US only, auto-focused | "they are focusing a lot on the initial stage" |
| **Avallon** | $4.6M | AI agents for calls, emails, doc triage | Intake automation only | "they are just calling the repair guy" |
| **ClaimSorted** | €11.4M | AI-first TPA | TPA model, not pure software | "their positioning is the worst" |
| **FurtherAI** | $30M (a16z) | AI workforce for insurance, 30x faster intake | All-lines horizontal tool | "they are trying to do everything" |
| **omni:us** | ~€45M | Berlin. End-to-end claims AI, 70% auto-settlement | Document-processing focused | — |
| **MarvelX** | €5.4M | Amsterdam. "ClaimOS MaX" EU-first agentic AI | Founded 2025, pre-traction | — |
| **Crawford/Turvi CoverAI** | Corporate | AI coverage review | Proprietary to Crawford TPA stack | — |
| **CCC/EvolutionIQ** | $730M acquisition | AI claims guidance for auto casualty | US only, auto casualty only, enterprise | — |

---

### 4e. Master Comparison Matrix

| Dimension | **Mysa** | **Five Sigma** | **Verisk XactAI** | **Shift Claims** | **Assured** |
|-----------|----------|---------------|-------------------|-------------------|-------------|
| **Core focus** | Decision engine (6 steps) | CMS + copilot | Estimation + admin AI | Fraud + workflow | FNOL + messaging |
| **Coverage analysis** | **Primary feature** | LLM matching (basic) | None | None | None |
| **Convention systems** | **EU-native** | None | None | None | None |
| **SOP-driven workflows** | **Yes — per carrier** | No (generic playbooks) | No | Limited | No (Flow Builder) |
| **Reserve setting** | **AI + P&L framing** | Basic | None | None | None |
| **Causation analysis** | Planned (property) | None | None | None | None |
| **Historical data engine** | **Core moat** | Limited | Data moat (estimates) | Fraud patterns | Interaction data |
| **Document generation** | **Per SOP, per decision** | Some | None | Limited | Standard |
| **EU presence** | **Primary market** | 30% | Minimal | 25+ countries | None |
| **US presence** | Expansion (Year 2) | 70% | Dominant (property) | Growing | Primary |
| **Integration** | Any CMS via API | Any CMS via API | Xactimate ecosystem | Own platform | On any CMS |
| **Funding** | Pre-seed | ~$20M | Public ($35B+) | $320M | $1B valuation |
| **Target buyer** | Mid-to-small carriers | Mid-market | All Xactimate users | Large carriers | Large carriers |

---

## Part 5: How It Works — Product Architecture & Technology

### 5a. The Product Flow

> [TRANSCRIPT — Co-founder]: "So think the product is quite similar to Avalon in the way that it is built. Like, you have the process. You can generate emails. You can parse emails that we are getting. We can draft the email... we parse that. We understand if something is missing. Then you can send automated emails. You can have AI calling."

```
CLAIM ARRIVES (email, portal, API, broker submission)
  │
  ▼
STEP 1: INTAKE PARSING
  │ Parse incoming documents, emails, photos, scanned forms
  │ "I am getting data from all those intake sources" [TRANSCRIPT]
  │ "If I'm missing data, I'll go back to the user" [TRANSCRIPT]
  │
  ▼
STEP 2: DATA STRUCTURING
  │ Extract fields, validate completeness, structure for processing
  │ Uses Caravela OCR engine for document extraction (~80% accuracy → targeting 90%+)
  │ "we need to structure the data" [TRANSCRIPT]
  │
  ▼
STEP 3: TRIAGE
  │ Complexity scoring, assignment, prioritization
  │ Apply SOP-driven workflows for routing
  │ "when we onboard, we upload SOPs, translate SOPs into workflows" [TRANSCRIPT]
  │ "auto triage: I have 20-30%. So you still have value here if you can create more" [TRANSCRIPT]
  │
  ▼
STEP 4: INVESTIGATION SUPPORT
  │ Guide adjuster through investigation per SOP
  │ Record calls, guide through questions, generate investigation docs
  │ "We are recording the calls that you need to make.
  │  We are guiding you through those calls." [TRANSCRIPT]
  │
  ▼
STEP 5: DECISION ENGINE — The 6 Judgment Sub-Steps
  │ For each: AI recommends with confidence score + explanation
  │ Human reviews, accepts/modifies/rejects
  │ "within decisions, there are six subsections, and for each
  │  one of them, we already help you" [TRANSCRIPT]
  │
  │  ┌──────────────────────────────────────────────────────────┐
  │  │ 1. Coverage verification    ← Policy parsing + SOP       │
  │  │ 2. Policy report checking   ← Document completeness      │
  │  │ 3. Repair assessment        ← Comparable analysis         │
  │  │ 4. Cost analysis            ← Market rates + historicals  │
  │  │ 5. Reserve calculation      ← Statistical model + P&L    │
  │  │ 6. Fraud detection          ← Pattern matching + signals  │
  │  └──────────────────────────────────────────────────────────┘
  │
  ▼
STEP 6: DOCUMENT GENERATION
  │ Generate all required documents per SOP template
  │ Coverage determination letters, reserve memos, investigation summaries
  │ "we are generating all the documents for you" [TRANSCRIPT]
  │
  ▼
STEP 7: FEEDBACK LOOP — Decision Ground Truth Capture
  │ Adjuster's actual decisions vs AI recommendations → training data
  │ "we are training our models to eventually start taking these steps" [TRANSCRIPT]
  │ Models improve with every claim processed
  └──────→ Flywheel: better data → better recommendations → more trust → more data
```

---

### 5b. Agent-Based Architecture

[CLAUDE ANALYSIS]: Based on the product flow and Five Sigma's multi-agent approach (proven viable with 6 agents on Gemini), Mysa should have 8 specialized agents:

| Agent | Function | Inputs | Outputs |
|-------|----------|--------|---------|
| **Intake Agent** | Parse emails, docs, photos. Identify missing info. Draft follow-up requests automatically. | Raw email, attachments, portal submissions, scanned docs | Structured claim data, missing data alerts, auto-drafted outreach |
| **Triage Agent** | Score complexity. Apply SOP workflows. Route to right desk/adjuster/priority. | Structured claim data, carrier SOPs, historical patterns | Assignment recommendation, priority score, SOP workflow activated |
| **Coverage Agent** | Read policy document. Match claim facts against coverage clauses and exclusions. Flag ambiguities. | Policy document, claim facts, carrier SOPs, coverage rules | Coverage determination recommendation + confidence score + cited clauses |
| **Investigation Agent** | Scope what needs to be investigated. Guide calls per SOP. Record and transcribe. Generate investigation docs. | Claim data, comparable claims, SOPs, call recordings | Investigation checklist, transcripts, investigation summary document |
| **Reserve Agent** | Calculate suggested reserve with confidence intervals. Compare to historical claims. Flag P&L impact. | Historical claims data, claim facts, market rates, carrier reserve rules | Reserve recommendation + variance analysis + P&L impact memo |
| **Fraud Signal Agent** | Pattern matching against known fraud indicators. Score risk. Recommend SIU referral. | Claim data, fraud pattern database, red flag rules | Fraud risk score + flagged indicators + SIU referral recommendation |
| **Document Agent** | Generate all required documents per SOP and per decision step. Apply carrier templates. | All decision outputs, SOPs, carrier templates | Coverage letters, reserve memos, denial letters, investigation summaries |
| **SOP Compliance Agent** | Check every decision against carrier-specific SOPs. Flag deviations. Ensure audit trail. | All decisions, SOP database, approval thresholds | Compliance status + deviation flags + audit trail |

---

### 5c. Technology Stack

> [TRANSCRIPT — Jeremy]: "right now, I went for Gemini because it's us. But if we wanted to build a really robust thing, we could go somewhere else."

> [TRANSCRIPT — Co-founder]: "And that's also why we are selling this to investors in the sense that we started with documentation because our product, a core part of the product is reading documents."

| Component | Technology | Rationale |
|-----------|-----------|-----------|
| **LLM backbone** | Gemini | Proven for insurance by Five Sigma. Existing Caravela expertise. Cost-effective for high-volume document processing. |
| **Document processing** | Caravela OCR engine | Existing asset, Gemini-based, ~80% accuracy (targeting 90%+). [TRANSCRIPT: "I was looking at OCR results... the top companies advertise 98-99% on historical data"] |
| **EAS processing** | OCR → structured data → convention matching | Deterministic rules engine for CIMPAS/IDS/IRSA/CARD/CIDE |
| **Policy parsing** | LLM + structured extraction | Read coverage clauses, exclusions, conditions — output structured coverage map |
| **Cloud hosting** | EU-region (AWS eu-west / GCP europe-west) | NOT on-prem. [AGENT RESEARCH]: 85% cloud adoption in P&C. GDPR doesn't require on-prem. Mid-market lacks IT resources. |
| **Integration** | REST API + webhooks | Same approach as Five Sigma — proven viable. Works on any CMS. |
| **Estimation integration** | Xactimate API (US), Audatex/Solera API (EU) | Must-have for assessment step. [TRANSCRIPT: "How can we integrate with them?"] |
| **Call recording** | Recording + transcription | For investigation support. Similar to Harvey.ai for legal. |
| **Data storage** | Encrypted, EU-resident, GDPR Article 22 compliant | Claims data is sensitive. AI Act high-risk conformity required. |

---

### 5d. The Human-in-the-Loop Requirement

> [TRANSCRIPT — Jeremy]: "it's mandatory to always have a human step."
> [TRANSCRIPT — Co-founder]: "Really? Even in The US?"
> [TRANSCRIPT — Jeremy]: "You cannot be 100%... there needs to be a human."

[RESEARCH: Section 9]: GDPR Article 22 prohibits fully automated decisions with legal effect. EU AI Act classifies claims AI as high-risk — requires human oversight, conformity assessment, transparency.

[CLAUDE ANALYSIS]: Human-in-the-loop is a FEATURE, not a limitation:
1. **Regulatory compliance** baked into the architecture
2. **Adoption** — adjusters feel augmented, not replaced (critical for sales)
3. **Training data** — every human decision creates ground truth for model improvement
4. **Error catching** — prevents wrongful denials (lawsuits) or overpayment (leakage)
5. **Trust building** — carriers need to trust AI before letting it decide autonomously

---

## Part 6: EU Motor — First Attack Area

### 6a. Why EU Motor First

> [TRANSCRIPT — Co-founder]: "cars in Europe, you don't need it [an adjuster]... But it's very, very small. If you build the product for that, you don't have a company."

[CLAUDE ANALYSIS]: The co-founder is RIGHT that EU motor alone isn't enough for a company. EU motor is the WEDGE:
1. **Proves the technology** — EAS digitization + convention matching is a clean, measurable problem
2. **Lands design partner** — Caravela is in Portugal, co-founder has the network
3. **Builds capabilities** — OCR, document AI, structured decision logic all transfer to property
4. **Creates defensible moat** — Convention system expertise takes years to build, nobody else has it
5. **Lower risk first product** — Simpler decisions (deterministic conventions), smaller blast radius

The COMPANY is built on property + US expansion. EU motor is the proof point.

---

### 6b. Convention Systems by Country

[RESEARCH: Section 11 — STP Reality Gap Deep Dive]:

| Country | Convention | How it works | Coverage | Speed | Key data | Market size (validated) |
|---------|-----------|-------------|----------|-------|----------|----------------------|
| **Portugal** | IDS/CIMPAS | Direct compensation protocol. Both insurers settle with their own policyholder. | ~100% market participation | **1.94 days** avg decision time | 91% inter-insurer agreement rate | ~€1.8B GWP, 5.8M vehicles, 63 domestic insurers, top 3 = 59.2% |
| **Spain** | CIDE/ASCIDE/CICOS | Tabla de Culpabilidad (fault table) + CICOS digital platform | 70-83% of all motor claims | Varies | 2.5M claims/year processed via CICOS | **€13.2B GWP** (2024), 34M vehicles, 187 companies, 15-25 mid-market |
| **France** | IRSA | 13 standardized cases. Outputs only 0%, 50%, or 100% fault. | ~80% of material motor claims | Deterministic (instant lookup) | Simplest fault model in EU. **7.4M claims/year** (confirmed) | **€28.1B GWP** (2024), 45.5M vehicles, 246 FFA, 20-30 mid-market |
| **Italy** | CARD | Mandatory for 2-vehicle claims, <9% permanent disability. Civil code + CAI form. | All qualifying 2-vehicle claims | Days | Most complex form. **2M claims paid** (confirmed), avg €2,105 | **~€14.8B GWP** (2023), ~40M vehicles, ~205 insurers, 10-15 mid-market |

**Convention lookup is trivial** — it's a database query. The bottleneck is getting clean, structured data FROM the EAS form INTO the convention system. That's where Mysa's OCR fits.

---

### 6c. The EAS → STP Pipeline

**Current process (manual):**
```
Paper EAS → Manual data entry (error-prone, 20-30 min) →
Convention lookup (trivial) → Settlement decision →
Human review → Payment
```
STP rate: ~10%

**Mysa process:**
```
Paper EAS → OCR extraction (2 min) → Structured data →
Convention matching (instant) → Fault determination →
Settlement recommendation + documents → Adjuster review (2-3 min) → Payment
```
Target STP rate: 40-50%

**Delta = 30-40 percentage point improvement.** For a carrier processing 50,000 motor claims/year, this means:
- 15,000-20,000 additional claims processed with minimal human intervention
- At ~45 min saved per claim = 11,250-15,000 hours saved/year
- At €50/hour loaded cost = €562K-€750K saved/year
- Mysa charges €100K-200K/year = 3-7x ROI

---

### 6d. Country-by-Country Rollout

**Phase 1: Portugal** (Months 1-3)
- Design partner: Caravela
- Convention: CIMPAS/IDS
- Why first: Co-founder network, smallest market (fastest to prove), best convention performance (91% agreement)
- Target: 5-10 Portuguese mid-market carriers

**Phase 2: Spain** (Months 4-6)
- Convention: CIDE/ASCIDE/CICOS
- Why second: Largest convention volume (2.5M/year), existing CICOS digital platform to integrate with. 187 companies operating (2024), €13.2B motor GWP, 34M insured vehicles. **15-25 mid-market carriers** in the €50-500M range (Linea Directa, Pelayo, Reale, Caser, Santalucia, etc.)
- Competition risk: Bdeo has 7/10 top Spanish auto insurers (but for visual AI, not decisions)
- Target: 10-15 Spanish mid-market carriers

**Phase 3: France and/or Italy** (Months 7-9)
- France (IRSA): Largest EU motor market (**€28.1B GWP** 2024, 45.5M vehicles, 246 in FFA, **7.4M claims/year confirmed**), simplest fault model (13 cases). **20-30 mid-market carriers** (Matmut, Direct Assurance, L'Olivier, etc.). Market leader Covéa (MAAF/MMA/GMF) ahead of AXA. Mutual-heavy structure = sometimes resistant to external tech but rising claims costs (+4.3%) create urgency.
- Italy (CARD): Complex but mandatory — high pain = high willingness to pay. ~40M vehicles, **2M claims paid** for €10B annually (avg €2,105/claim, +4.2%). UnipolSai dominant, then Generali (€3B), Allianz (€2.67B). **10-15 mid-market carriers** (Reale Mutua, Vittoria, Groupama Italy, Sara, HDI).
- Target: 10-20 carriers across both markets

**Phase 4: Northern EU** (Months 10-12+)
- Germany, Netherlands, Belgium — different convention systems
- Higher technical complexity but larger markets
- By this point, Mysa has convention matching expertise from 3+ countries

---

## Part 7: Product Roadmap — 18 Months

### Phase 1 (Months 1-3): MVP — Portuguese Motor

**Build:**
- EAS OCR pipeline (Portuguese forms) — leverage Caravela OCR engine
- CIMPAS/IDS convention matching engine (deterministic rules)
- Basic adjuster dashboard: claim data, convention match result, recommended fault
- Email/document parsing for incoming claims (email → structured claim)
- Missing data detection + auto-drafted follow-up requests

**Ship to:** Caravela (free beta, weekly syncs)

**Success metric:** Process 100 Portuguese motor claims. Measure STP rate improvement vs baseline.

> [TRANSCRIPT — Co-founder]: "I hope that we build this, and then I test this with caravela."
> [TRANSCRIPT — Jeremy]: "we need to meet weekly with Caravela."

---

### Phase 2 (Months 4-6): EU Motor V1 — Multi-Country

**Build:**
- Spain (CIDE) and France (IRSA) convention support
- SOP upload → workflow generation engine
- Triage automation (complexity scoring, desk vs field routing)
- Reserve recommendation engine (basic — historical comparables)
- STP rate tracking dashboard
- Broker-facing view (claim status, documents, timeline)

**Ship to:** 3-5 paying EU carriers (Portugal + Spain)

**Success metric:** Measurable STP improvement at 3+ carriers. First paying customer.

> [TRANSCRIPT — Co-founder]: "when we onboard an insurance company, we upload the SOPs, and we also translate those SOPs into workflows."

---

### Phase 3 (Months 7-9): Decision Engine Core

**Build:**
- Coverage verification engine (policy document parsing + coverage determination)
- Investigation support (call recording, guided investigation, document generation)
- The 6 decision sub-steps as distinct AI modules
- Fraud signal detection
- REST API for CMS integration (any CMS)
- Playbooks per claim type (SOP-driven, not generic)

**Ship to:** Existing EU motor customers (expanded capabilities) + first property pilots

**Success metric:** First property claim processed through full decision pipeline.

---

### Phase 4 (Months 10-12): US Market Entry

**Build:**
- Xactimate integration (non-negotiable for US property)
- US-specific coverage rules engine (50-state variation handling)
- Adjuster decision copilot packaged for US property mid-market
- Contents valuation support

**Ship to:** 3-5 US pilot customers (mid-market carriers or TPAs)

**Success metric:** First US revenue.

---

### Phase 5 (Months 13-18): Platform Expansion

**Build:**
- Coverage + causation AI for property (the "sudden vs gradual" problem)
- Historical claims analytics engine (the data flywheel kicks in)
- Multi-line support (commercial property, specialty lines)
- Enterprise features (SSO, audit trails, compliance reporting, multi-level approval workflows)
- Advanced reserve modeling with P&L impact dashboard

**Target:** $1M+ ARR, 10+ paying customers across EU and US

---

## Part 8: Demo Plan — What to Build

### Context

> [TRANSCRIPT — Co-founder]: "Let me see if my guy built the demo. Most likely it's shit."
> [TRANSCRIPT — Co-founder]: "I tried to build two demos today, and they basically... I think we need to build block by block."
> [TRANSCRIPT — Jeremy]: "Yeah. It has to be. Otherwise, it goes everywhere and nowhere at the same time."
> [TRANSCRIPT — Co-founder]: "Let's build the demo tomorrow. We have something to show."

**Principle: Block by block.** Don't try to show the full product. Show specific, impressive steps.

---

### Demo 1: EU Motor — EAS to Settlement (The "Easy Case")

> [TRANSCRIPT — Co-founder]: "On the demo, we already see that, oh, let me call the repair shop. But that's a demo like this. It's the most easy case possible."

**Scenario:** Portuguese motor claim. Two-car fender bender. No injuries. Paper EAS form filled out at scene.

**Step-by-step demo flow:**

| Step | What happens on screen | What to highlight | Technical requirement |
|------|----------------------|-------------------|---------------------|
| 1. Claim arrives | Email with attached scanned EAS form appears in inbox | "This is what arrives today — a messy paper form" | Email parsing, attachment extraction |
| 2. OCR extraction | Split screen: raw EAS image on left, extracted structured data on right | "In 30 seconds, Mysa extracts every field" — show accuracy on messy handwriting | Caravela OCR engine on EAS forms |
| 3. Missing data | Mysa flags: "Counterparty policy number is missing. Checkbox 7 is ambiguous." | "Mysa catches what humans miss" | Field validation, completeness checking |
| 4. Auto-outreach | Draft SMS/email to policyholder requesting missing info | "Automated follow-up — no adjuster time spent" | Template generation, SMS/email integration |
| 5. Convention match | With complete data: "CIMPAS Case 7 matched. 95% confidence." | "The convention system is a solved problem — the data quality was the bottleneck" | Convention matching engine (deterministic) |
| 6. Fault determination | "Based on checkboxes 2, 4, 7 and diagram analysis: 100% liability to Party A" | Show the reasoning chain, not just the answer | Explainable AI output |
| 7. Reserve recommendation | "Estimated repair: €2,400-€3,100. Recommended reserve: €3,100. Based on 847 similar claims." | "P&L impact: this reserve is immediately recognized as a loss" | Historical data matching |
| 8. Settlement recommendation | Full recommendation + auto-generated settlement documents | "Before: 3-5 days, 45 min adjuster time. After: 4 min review." | Document generation per SOP |
| 9. Adjuster review | Adjuster clicks approve/modify. Decision logged. | "Human always decides. AI recommends. Every decision trains the model." | Human-in-the-loop UI |

**What makes this demo impressive:**
- The SPEED: 30 seconds from paper EAS to structured data
- The ACCURACY: on messy handwriting
- The AUTOMATION: convention matching is instant once data is clean
- The DOCUMENTS: everything generated automatically
- The COMPARISON: before/after (3-5 days → 4 minutes)

---

### Demo 2: US Property — Water Damage (The "Hard Case")

> [TRANSCRIPT — Co-founder]: "imagine that you get the claim. It's a water leakage. You have, oh, let me look at the images on my desk. Let me check. Okay. Actually, this seems a bit — I'm not sure. So I need to send someone there."

**Scenario:** Homeowner reports water damage in basement. Standard HO-3 policy. The key question: is this covered? (sudden burst = covered, gradual seepage = excluded)

**Step-by-step demo flow:**

| Step | What happens | What to highlight |
|------|-------------|-------------------|
| 1. Claim arrives | Homeowner email: photos of wet basement, brief description | "This is what lands on a desk adjuster's screen" |
| 2. Photo analysis | Mysa categorizes: water damage, basement, ~200 sq ft affected | "AI reads photos, doesn't just store them" |
| 3. Policy parsing | HO-3 policy loaded. Coverage clauses highlighted in green. Exclusions in red. | "Mysa reads the WHOLE policy, not just the header" |
| 4. Coverage question identified | "Coverage determination requires: was this sudden or gradual?" | "This is the judgment call nobody automates" |
| 5. SOP-driven investigation | "Investigation checklist generated from YOUR company's SOP" — Request plumber's report, check maintenance records, assess damage pattern, schedule field if needed | "Every carrier has different SOPs. Mysa follows YOURS." |
| 6. Decision support (covered) | After plumber confirms sudden burst: "Coverage APPLIES under Section I, Coverage A. Deductible: $1,000." + Reserve: "Median similar claims: $8,400. Recommended: $9,200." | "The 6 sub-steps, with reasoning, not just an answer" |
| 7. Document generation | Coverage determination letter, reserve memo, investigation summary — all per SOP | "Every document your SOP requires, auto-generated" |
| 8. **The "what if"** | Switch scenario: evidence shows gradual seepage instead. Coverage Agent flips: "Exclusion 2.c applies. Recommend DENIAL." Denial letter auto-generated with policy citations. | "Same product, opposite outcome. The AI adapts to evidence." |

**What makes this demo impressive:**
- The COVERAGE DETERMINATION: nobody else automates "sudden vs gradual"
- The SOP COMPLIANCE: workflows from the carrier's own procedures
- The WHAT-IF: showing the AI can reason in both directions
- The DOCUMENTS: denial letter with correct policy language citations
- The HUMAN-IN-THE-LOOP: adjuster always decides

---

### Demo 3: The Historical Data Flywheel (If Time)

> [TRANSCRIPT — Co-founder]: "the second time that you have a second case, for that claim type, it will be always [faster] and it might already be slightly automated because our AI [learned from the first one]."

Show: After processing 100+ water damage claims, Mysa displays:
- "87% of similar claims in your region with this plumber's report pattern were covered"
- "Average settlement: $9,100"
- "Recommend expedited processing — confidence: HIGH"
- Time-series showing recommendation accuracy improving over time

---

### Demo Requirements Summary

**Must show (non-negotiable):**
1. OCR accuracy on real documents (EAS forms, policies, emails)
2. SOP → workflow generation (upload SOP, see structured workflow)
3. The 6 decision sub-steps with AI recommendations + confidence scores
4. Human-in-the-loop (adjuster reviews, adjusts, approves)
5. Document generation per decision
6. Before/after time comparison (manual vs Mysa)

**Should NOT try to show:**
- Full CMS replacement (we're not a CMS)
- Real-time call recording (complex, save for v2)
- Xactimate integration (US-only, complex — save for Phase 4)
- Multi-user workflow (single-adjuster view is enough for demo)
- Historical data flywheel (only if time permits)

**Technical build requirements for demo:**
1. EAS OCR pipeline (can use Caravela engine)
2. Convention matching rules engine (CIMPAS for Portugal, at minimum)
3. Policy document parser (can use Gemini for initial demo)
4. SOP upload → workflow UI
5. Adjuster dashboard with 6 decision sub-step cards
6. Document generation templates (coverage letter, denial letter, reserve memo)
7. Before/after comparison screen

[CLAUDE ANALYSIS]: The demo should be a real working product, not a mockup. Using Caravela's OCR engine + Gemini for policy parsing + a simple convention matching rules engine, a functional demo for Demo 1 (EU motor) could be built in 2-3 weeks. Demo 2 (US property) requires policy parsing which is harder — this could be a guided demo with pre-loaded data initially.

---

## Part 9: Fundraising Narrative

### 9a. The Market — Full EU Country-by-Country + US Comparison

[AGENT RESEARCH — validated via EIOPA, BaFin, ACPR, IVASS, ASF, DGSFP, DNB, FSMA, FMA, FINMA, Central Bank of Ireland, FI Sweden, FSA Denmark, FIN-FSA, Finanstilsynet Norway, KNF Poland, CNB Czech Republic, NAIC, AM Best, Conning]

#### EU Motor Insurance — 16 Countries

**Southern EU (convention systems — first attack):**

| Country | Motor GWP | Convention System | Total Insurers | Caravela Tier (€100-200M) | Small (€50-100M) | Convention Detail |
|---------|----------|-------------------|---------------|--------------------------|-------------------|-------------------|
| **Portugal** | **€1.8B** | IDS/CIMPAS | ~47 active | 6-8 | 8-12 | 1.94 day avg, 91% agreement |
| **Spain** | **€13.2B** | CIDE/ASCIDE/CICOS | ~176 | 8-10 | 25-35 | 2.5M claims/year processed |
| **France** | **€28.1B** | IRSA | ~660 | 30-60 | 100+ | 13 cases, deterministic |
| **Italy** | **€14.8B** | CARD | ~85 | 10-15 | 8-12 | Mandatory for 2-vehicle |
| **Southern EU Total** | **€57.9B** | **All have convention** | | **54-93** | **141-159+** | |

**Northern/Central EU (expansion markets — mixed convention):**

| Country | Motor GWP | Convention System | Total Insurers | Caravela Tier (€100-200M) | Small (€50-100M) |
|---------|----------|-------------------|---------------|--------------------------|-------------------|
| **Germany** | **~€30B** | Teilungsabkommen (bilateral only) | ~522 BaFin + 534 state | 15-25 | 20-35 |
| **Netherlands** | **~€5.9-6.2B** | DSA (new, launched 2024) | ~60-70 | 3-5 | 5-8 |
| **Belgium** | **~€4.3-4.5B** | RDR (Convention Règlement Direct) | ~82-90 | 5-8 | 8-12 |
| **Austria** | **~€4.3B** | None formal | ~30-35 | 2-4 | 3-5 |
| **Switzerland** | **~€7.2-8.2B** | None formal | ~117 | 3-5 | 5-8 |
| **Ireland** | **~€1.3B** | None | ~40-50 | 2-4 | 3-5 |
| **Sweden** | **~€2.6-2.9B** | Trafikskadenämnden | ~50-60 | 3-4 | 4-6 |
| **Denmark** | **~€2.0-2.4B** | None formal | ~40-50 | 2-3 | 3-5 |
| **Finland** | **~€1.2-1.4B** | Traffic Insurance Centre | ~40-49 | 2-3 | 2-3 |
| **Norway** | **~€2.7-2.8B** | None formal | ~30-40 | 2-3 | 3-4 |
| **Poland** | **~€6.5B** | UFG coordination | ~29 | 3-5 | 4-6 |
| **Czech Republic** | **~€2.1-2.3B** | None formal | ~24-30 | 2-3 | 3-4 |
| **Northern/Central EU Total** | **~€70-78B** | **Mixed** | | **~42-72** | **~63-101** |

**Full EU Totals:**

| Tier | Southern EU | Northern/Central EU | **All EU** |
|------|------------|--------------------|-----------|
| Enterprise (>€1B — builds in-house) | 16-19 | ~20-30 | **~36-49** |
| Large (€200M-€1B — buys best-of-breed) | 30-47 | ~30-50 | **~60-97** |
| **Caravela tier (€100-200M — PRIMARY)** | **54-93** | **42-72** | **~96-165** |
| Small (€50-100M — entry-level) | 141-159+ | 63-101 | **~204-260+** |
| Micro (<€50M — long-tail) | 243-372+ | 200-400+ | **~443-772+** |
| **Total motor GWP** | **€57.9B** | **~€70-78B** | **~€128-136B** |

[CLAUDE ANALYSIS]: Key insight: the Northern EU market is LARGER in premium terms than Southern EU (€70-78B vs €57.9B) but has FEWER mid-market carriers in the Caravela tier. Germany alone is €30B but concentrated in large players. Southern EU has more fragmented markets = more mid-market targets. Convention systems in Southern EU provide the wedge, but Germany/Benelux/Nordics are the expansion that makes this a real company.

#### US Market — For Comparison

[AGENT RESEARCH — validated via NAIC 2024 Market Share, AM Best, Conning, IBIS World]

| Segment | Count | Premium/Revenue | Concentration |
|---------|-------|----------------|--------------|
| Total P&C carriers | ~4,116 entities | $1.06T DWP | Top 10 = 51.4%, Top 100 = ~90% |
| **Auto insurance** | — | **$359B** | **Top 5 = 63.6%** (extremely concentrated) |
| **Homeowners** | — | **$173B** | Top 25 = 78% (less concentrated) |
| Commercial multi-peril | — | $87B | More fragmented |
| Workers' comp | — | $65B | Fragmented |

**US Carrier Distribution by Size:**

| Tier (DWP) | # Carriers | Profile |
|-----------|-----------|---------|
| >$5B (top 25-30 groups) | ~25-30 | Build in-house (State Farm, GEICO, Progressive, Allstate) |
| $1B-$5B | ~50-80 | Mix of build/buy — Cincinnati Financial, Hanover, Erie |
| **$100M-$500M (Caravela-comparable)** | **~200-350** | **Buy-not-build — can't afford data science teams** |
| $50M-$100M | ~150-250 | Lean operations, budget-conscious |
| <$50M | ~3,000+ | Micro carriers, regional, many inactive/run-off |

**US Adjacent Buyers:**

| Buyer Type | Count (material size) | Why They Buy |
|-----------|----------------------|-------------|
| TPAs (P&C-focused) | ~500-800 | Process claims for carriers, need efficiency tools |
| MGAs with claims authority | ~330-550 | Growing 16% CAGR, increasingly handle claims |
| Independent adjusting firms | ~53,000 businesses ($11.7B market) | Workforce is their product — augmentation = survival |

**Total US addressable buyers: ~1,030-1,700** (carriers + TPAs + MGAs with claims authority)

[CLAUDE ANALYSIS]: The US market is 3-4x larger than EU by carrier count and 8x by premium. But US auto is dangerously concentrated (top 5 = 63.6%) — the mid-market opportunity is in homeowners and commercial, not auto. For Mysa, US entry should target homeowners/property mid-market carriers + TPAs, not US auto.

#### Competitor Adoption — How Open Is the Market?

[AGENT RESEARCH — validated via company press releases, Crunchbase, analyst reports, customer case studies]

| Competitor | Est. Customers | Geographic Mix | Customer Profile | What They Sell |
|-----------|---------------|---------------|-----------------|---------------|
| **Five Sigma/Clive** | ~20-30 | 70% US, 30% EU | Starr, Qover, INSHUR, Pie Insurance | CMS + AI copilot |
| **Shift Technology** | ~135 | 25+ countries | AXA Switzerland, Tokio Marine, Generali — **large carriers** | Fraud → workflow automation |
| **Tractable** | ~20-35 | UK, EU, US | GEICO, Covéa, Aviva, PZU — **enterprise only** | Computer vision for damage |
| **Bdeo** | ~50+ | Spain-dominant | 8/10 top Spanish auto insurers | Visual intelligence photos/video |
| **Hi Marley** | ~40+ | US only | American Family, MetLife, Erie | Communication (text/messaging) only |
| **omni:us** | ~3-5 | DACH region | Allianz Austria, UNIQA, Württembergische | Document processing + auto-settlement |
| **ClaimSorted** | ~20+ | UK, EU, US | Mid-market | AI-first TPA (not pure software) |
| **Assured** | Unknown (est. 10-20) | US only | Large carriers | FNOL + messaging AI agent "Emma" |
| **FurtherAI** | ~3-5 | US only | Early stage | AI workforce for intake |
| **Avallon** | ~3-5 | US only | Early stage | AI agents for calls/emails |
| **Total "taken" globally** | **~400-600** | | | |

**Market openness by segment:**

| Segment | Total Entities | Using Claims AI | % Open | Mysa Opportunity |
|---------|---------------|----------------|--------|-----------------|
| All carriers globally (EU + US) | ~6,300+ | ~400-600 (~7%) | **~93% open** | Massive whitespace |
| EU mid-market (€50-200M) | ~300-425 | <30 (Shift customers are large, Bdeo = visual only) | **~90-95% open** | **Primary target — virtually untouched** |
| US mid-market ($100-500M) | ~200-350 | ~30-50 (Five Sigma + Hi Marley customers) | **~75-85% open** | Strong — but competitors more active |
| TPAs globally | ~500-800+ | ~50-80 (Shift, ClaimSorted) | **~85-90% open** | Good expansion target |
| MGAs with claims authority | ~330-550 | <20 | **~95% open** | Emerging segment, growing fast |

**Critical insight: Only 4% of insurers have SCALED AI in claims** [WEB SOURCE: McKinsey 2025 insurance survey]. Most "adoption" is pilots, POCs, or single-feature tools (Bdeo = photos only, Hi Marley = texting only). Nobody has deployed an AI decision engine at scale.

> [TRANSCRIPT — Co-founder]: "everyone is trying something... everyone is trying to build a platform... And everyone is avoiding the judgment, the decision stage."

[CLAUDE ANALYSIS]: The market is overwhelmingly open. The EU mid-market is 90-95% untouched by AI claims tools. Even the US mid-market is 75-85% open despite more competitor activity. The "competition" narrative is misleading — most funded competitors serve large carriers (Shift, Tractable) or focus on intake/communication (Assured, Hi Marley, Avallon). The decision layer is genuinely unoccupied.

---

### 9b. Revised TAM — All Data Combined

**Building the TAM bottom-up with validated carrier counts:**

| Scenario | EU Carriers | US Buyers | Total Buyers | ACV Range | **Revenue Range** |
|----------|------------|-----------|-------------|-----------|-------------------|
| **Conservative** — Southern EU Caravela tier only | 54-93 | — | 54-93 | €50-200K | **€2.7-€18.6M** |
| **Base** — All EU €50-200M carriers | 300-425 | — | 300-425 | €30-200K | **€25-55M** |
| **EU + large tier** — Add €200M-1B | 360-520 | — | 360-520 | €30-500K | **€50-100M** |
| **EU + US mid-market** — Add US $100-500M carriers | 360-520 | 200-350 | 560-870 | €30-500K | **€100-250M** |
| **Full addressable** — All EU + US (carriers + TPAs + MGAs) | 500-700 | 1,030-1,700 | 1,530-2,400 | €10K-2M | **€200-650M** |
| **With land-and-expand** — Upsell to property, commercial lines | — | — | Same | Higher ACV | **€400M-1.3B** |

[CLAUDE ANALYSIS]: The honest TAM story for fundraising:
- **Wedge TAM** (EU motor, Caravela tier) = €2.7-€18.6M — proves the product works, not venture-scale alone
- **Year 2-3 TAM** (all EU mid-market + large) = €50-100M — real SaaS business
- **Year 3-5 TAM** (EU + US mid-market) = €100-250M — venture-scale
- **Vision TAM** (full addressable + expansion) = €200-650M+ — IPO-scale

The narrative: "We're not raising on the wedge TAM. We're raising on the €100-250M EU+US mid-market TAM that the wedge unlocks. The technology we build for EU motor convention systems transfers directly to property coverage decisions — same AI architecture, bigger market."

---

### 9c. The Pitch

**Slide 1: The Problem**
100-120M insurance claims per year across the US and EU. The workforce that processes them is disappearing — 30% retiring in 5 years, 12th fastest-declining profession. And the decisions they make hit the company's P&L immediately through reserves.

**Slide 2: The Gap Everyone Missed**
$1B+ has been invested in automating claims INTAKE (Assured, Avallon, FurtherAI). Nobody has automated the DECISION — the 6 judgment steps that consume 60-70% of an adjuster's time: coverage, investigation, repair assessment, cost analysis, reserves, fraud.

> [TRANSCRIPT — Co-founder]: "everyone is avoiding the judgment, the decision stage."

**Slide 3: Mysa — AI Decision Engine for Claims**
SOP-driven workflows. 8 specialized AI agents. Human-in-the-loop always. Works on any CMS via API. Integrates with existing estimation tools (Xactimate US, Audatex EU).

**Slide 4: Why Now**
- LLMs finally accurate enough for recommendation (not automation)
- Workforce crisis creating urgent buyer need — carriers can't wait
- Document AI (OCR) reaching 90%+ accuracy on handwritten forms
- EU AI Act creates regulatory moat for compliance-first products

**Slide 5: Product**
Show the product flow: Intake → Structure → Triage → Investigate → Decide → Document → Learn

**Slide 6: Market**
- €200-650M TAM (€400M-1.3B with expansion) — 28.4% CAGR
- 16 EU countries + US = ~1,530-2,400 addressable buyers
- EU mid-market is **90-95% untouched** by AI claims tools
- Only **4% of insurers** have scaled claims AI
- 100-120M claims/year across both markets
- €50K-€2M ACV per customer

**Slide 7: Traction**
- Design partner: Caravela (Portuguese insurer, €188M GWP, 57K claims/year)
- Existing OCR engine: Caravela, Gemini-based, ~80% accuracy
- EU convention system expertise: CIMPAS/IDS built
- Co-founder insurance domain knowledge — 10+ years in claims

**Slide 8: Moat**
Three layers:
1. Convention system intelligence — country-by-country (4 systems built, 8+ planned), takes years to replicate
2. Decision ground truth data — captures WHY adjusters decide, not just outcomes
3. SOP-to-workflow generation — each carrier's rules encoded, creates switching costs

**Slide 9: Competition**
Everyone builds AROUND the decision, not the decision itself. Market is 90%+ open. [Show comparison matrix from Part 4e + competitor adoption table]

**Slide 10: Business Model**
- Per-claim SaaS: €2-10 per claim processed
- Platform license: €50K-€2M/year based on carrier size
- Land: EU motor (STP improvement, 54-93 carriers). Expand: all EU + property + US (~1,500+ buyers)

**Slide 11: Roadmap**
Phase 1-5 over 18 months (from Part 7). EU motor → multi-country → property → US → platform.

**Slide 12: Ask**
[TBD — depends on fundraising target]

> [TRANSCRIPT — Co-founder]: "I think we need to raise as much money as ClaimSorted [€11.4M]"
> [TRANSCRIPT — Jeremy]: "Further AI series A level [$30M]... on seed."

---

### 9d. Key Investor Objections + Honest Answers

| Objection | Answer | Evidence |
|-----------|--------|----------|
| "Isn't this what Five Sigma does?" | They're a CMS + copilot with ~20-30 customers. We're a decision engine. They have generic playbooks, we have carrier-specific SOP workflows. They don't do convention systems, causation analysis, or P&L-aware reserves. | [AGENT RESEARCH]: Five Sigma = $10.1M revenue, 6 generic agents, no SOP workflows, no EU conventions |
| "Won't Verisk just build this?" | They're an estimation company. XactAI is admin automation (photo labels, transcription), not expert judgment. Different product, different buyer. But they're the long-term risk — that's why we start in EU where they have no presence. | [AGENT RESEARCH]: XactAI = admin features only, no decision support, 2-3 year timeline at best |
| "Won't Shift eat this in EU?" | Shift automates workflow around decisions (135 customers, mostly large carriers). We automate the decision itself for mid-market. Fraud-first vs decision-first. Their 60% is task automation, not decision automation. EU mid-market is 90-95% open. | [AGENT RESEARCH]: Shift = no convention matching, no SOP workflows, fraud architecture, serves enterprise |
| "Why EU first when US is bigger?" | Convention systems are a unique wedge nobody else has. STP gap is measurable (10% → 40-50%). Design partner in Portugal. ~96-165 Caravela-tier carriers across 16 EU countries — virtually untouched. Technology transfers to US property. | [AGENT RESEARCH]: EU mid-market = 90-95% open, convention systems take years to build |
| "Can AI make coverage decisions?" | Human-in-the-loop always. AI recommends, adjuster decides. 3x productivity, not replacement. Legally required (GDPR, AI Act). Every decision = training data. | [RESEARCH: Section 9]: GDPR Art 22, EU AI Act high-risk classification |
| "EU market is too small" | EU alone = €50-100M TAM (360-520 mid-to-large carriers). EU + US = €100-250M TAM (560-870+ buyers). Full addressable with TPAs + MGAs = €200-650M. EU motor is the wedge, not the company. | [AGENT RESEARCH]: 16 countries validated, carrier counts per country |
| "Market is too competitive" | Only 4% of insurers have scaled claims AI. ~400-600 carriers globally use ANY claims AI tool. 90-95% of EU mid-market is untouched. Competitors focus on enterprise or single features (Bdeo = photos, Hi Marley = texting). Nobody has the decision layer. | [AGENT RESEARCH]: Competitor customer counts validated |
| "18-30 month sales cycles?" | Mid-to-small market buys faster (3-6 months). Design partner (Caravela), not cold outreach. Per-claim pricing lowers barrier. EU mid-market has 1-2 decision makers, not enterprise procurement. | [RESEARCH: Section 6]: TPAs prefer per-claim pricing |

---

### 9e. The Narrative Arc

> [TRANSCRIPT — Co-founder]: "We need to build models. We need to train data. And now I agree with you, and I think I found a way to train those models. Without hiring people."

**The story:**
We start with a simple, provable product — EAS digitization for EU motor. This builds our OCR + document AI + decision logic capabilities. We expand to property coverage AI — the same technology applied to a bigger problem. We capture decision ground truth data from every adjuster interaction. Over time, our models get smarter, and the gap between Mysa (carrier-specific, SOP-driven, decision-focused) and generic copilots (broad, template-based, task-focused) widens.

**The TAM progression — how we tell the story:**
1. **Wedge** (Year 1): Southern EU motor, Caravela tier → 54-93 carriers, prove product-market fit
2. **EU expansion** (Year 2): All 16 EU countries, all mid-market tiers → 300-520 carriers, €50-100M TAM
3. **US entry** (Year 2-3): US property mid-market + TPAs → add 400-700 buyers, €100-250M TAM
4. **Platform** (Year 3-5): Multi-line, historical data flywheel, land-and-expand → €200-650M+ TAM

The endgame: **the AI that knows how YOUR company makes claims decisions.** Not generic insurance AI — YOUR insurance AI.

---

## Part 10: Transcript Analysis — Saved

*Full transcript analysis with key decisions, features, market sizing, competitive positioning, blind spots, action items, and contradictions vs research has been saved as Section 23 of `home_property_competitive_deep_dive.md`.*

Key action items from the call:
1. Build demo block by block — start with EU motor EAS → settlement
2. Get Caravela LOI — free beta, 6 months, weekly syncs
3. Pitch to Sapphire next week for introductions
4. Share research documents between co-founders
5. Size EU market at country level — **DONE: 16 countries validated** (PT, ES, FR, IT, DE, NL, BE, AT, CH, IE, SE, DK, FI, NO, PL, CZ)
6. Define demo scenarios and build MVP

---

## Appendix: Sources

### Research Documents (This Repository)
- `claims_journey_discovery.md` — Motor claims journey mapping (Phases 0-6)
- `home_property_competitive_deep_dive.md` — Full competitive analysis, market sizing, strategic theses (22+ sections)
- `competitive_landscape_reality_check.md` — High-level competitive overview
- `SUMMARY.md` — Co-founder summary

### Key External Sources
- [Verisk XactAI Launch — Sept 2025](https://www.verisk.com/company/newsroom/verisk-introduces-new-ai-tools-to-streamline-the-property-claims-experience/)
- [Five Sigma / Starr Partnership — Jan 2026](https://www.prnewswire.com/news-releases/starr-modernizes-pc-and-specialty-claims-with-five-sigmas-ai-claims-platform-and-clive-302669986.html)
- [Shift Technology Launches Shift Claims — Sept 2025](https://www.shift-technology.com/resources/news/shift-technology-launches-shift-claims-to-power-claims-transformation-with-agentic-ai)
- [CCC/EvolutionIQ Acquisition — $730M](https://www.businesswire.com/news/home/20241220225656/en/)
- [Allianz Insurance Copilot](https://www.allianz.com/en/mediacenter/news/articles/250205-smarter-claims-management-smoother-settlements.html)
- [BLS — Claims Adjusters Fastest Declining](https://www.bls.gov/ooh/business-and-financial/claims-adjusters-appraisers-examiners-and-investigators.htm)
- [Fortune Business Insights — Claims Management Market](https://www.fortunebusinessinsights.com/claims-management-market-110629)
- [EIOPA Insurance Statistics](https://www.eiopa.europa.eu/tools-and-data/insurance-statistics_en)
- [NAIC 2024 Market Share Data](https://content.naic.org/article/naic-releases-2024-market-share-data)

### EU Country-Level Regulatory Sources (16-Country Market Sizing)
- Portugal: ASF (Autoridade de Supervisão de Seguros), ECO Sapo rankings
- Spain: DGSFP (Dirección General de Seguros), RAEA registry
- France: ACPR (Autorité de Contrôle Prudentiel), France Assureurs, FFA
- Italy: IVASS, ANIA (Associazione Nazionale fra le Imprese Assicuratrici)
- Germany: BaFin (Bundesanstalt für Finanzdienstleistungsaufsicht), GDV
- Netherlands: DNB (De Nederlandsche Bank), Verbond van Verzekeraars
- Belgium: FSMA (Financial Services and Markets Authority), Assuralia
- Austria: FMA (Finanzmarktaufsicht), VVO
- Switzerland: FINMA, SVV (Schweizerischer Versicherungsverband)
- Ireland: Central Bank of Ireland, Insurance Ireland
- Sweden: Finansinspektionen (FI), Svensk Försäkring
- Denmark: Finanstilsynet (FSA), Forsikring & Pension
- Finland: FIN-FSA (Finanssivalvonta), Finance Finland
- Norway: Finanstilsynet, Finans Norge
- Poland: KNF (Komisja Nadzoru Finansowego), PIU
- Czech Republic: CNB (Czech National Bank), CAP

### US Market Sources
- NAIC 2024 Market Share Reports, AM Best Financial Suite, Conning P&C reports, IBIS World
- McKinsey 2025 Insurance AI Survey (4% scaled AI adoption)
