# Module 1: Deep Positioning & Company Identity

**Status:** DRAFT v1.0
**Last updated:** February 9, 2026
**Feeds:** Marketing site hero/header, About page, pitch deck slides 0-2, sales pitch, internal alignment

---

## 1.1 Category Definition

### The Old Categories — And Why None of Them Fit

Insurance technology companies have been building tools for claims professionals for decades. Each falls into a well-understood category:

| Old Category | What It Is | Who's There | Why It's Wrong for Mysa |
|-------------|-----------|------------|------------------------|
| **Claims Management System (CMS)** | Database + workflow tracking for claims. Think "Salesforce for adjusters." | Guidewire ClaimCenter, Duck Creek Claims, Five Sigma, ClaimPilot, VCA Software | Commoditized. Tracks what happened — doesn't help with what to decide. |
| **Claims Copilot** | AI assistant that surfaces information and handles administrative tasks | Majesco Copilot, Microsoft Copilot for Insurance, Sedgwick Sidekick, Allianz's internal copilot | Broad but shallow. Helps you type faster — doesn't help you think better. |
| **Intake Automation** | Speeds up FNOL (First Notice of Loss — the initial claim submission) — document parsing, chatbots, automated data extraction | Assured (reported ~$1B raised) [WEB: Crunchbase], Avallon ($4.6M) [WEB: Crunchbase], FurtherAI ($30M) [WEB: Crunchbase] | Crowded, billions invested. Fixes the front door — doesn't fix what happens inside. |
| **Fraud Detection** | ML-based pattern matching on claims to flag suspicious activity | Shift Technology (~$320M raised) [WEB: Crunchbase], FRISS, SAS | Important but narrow. One of six decision steps, not the whole decision. |
| **Estimation Tools** | Calculate repair costs for auto and property damage | Verisk/Xactimate (~$35B market cap) [WEB: NYSE: VRSK], CCC Intelligent Solutions, Solera/Audatex | Entrenched monopolies. Estimation is one input to the decision — not the decision itself. |

[SOURCE: mysa_product_strategy.md, Part 1 — "The Positioning Problem: CRM vs Decision Engine"]

Every one of these categories addresses a piece of the claims workflow. **None of them address the decision itself** — the 6 expert judgment steps where an adjuster determines coverage, assesses liability, calculates reserves, and decides what to pay.

### The New Category: Claims Decision Engine

> "Everyone is trying something... everyone is trying to build a platform... And everyone is avoiding the judgment, the decision stage."
> — Tiago Brigido, Co-founder [TRANSCRIPT: Feb 7, 2026]

A **Claims Decision Engine** is a new category of software. It sits between intake (where data arrives) and settlement (where money moves) — in the space where adjusters actually think.

**What makes it different:**

| Dimension | CMS / Copilot | Decision Engine (Mysa) |
|-----------|--------------|----------------------|
| **Core function** | Track cases, surface info, automate admin | Guide expert judgment through coverage, liability, reserves, fraud |
| **Intelligence source** | Generic insurance knowledge or pre-built templates | Carrier-specific SOPs encoded into decision workflows |
| **Data captured** | Claim outcomes (what was paid) | Decision reasoning (WHY the adjuster decided) |
| **Competitive moat** | Features, integrations | Knowledge — SOP encoding, decision ground truth, convention expertise |
| **Value metric** | Time saved on admin | Claims handled per adjuster, reserve accuracy, decision consistency |
| **Learning loop** | Static rules or periodic ML retraining | Every adjuster interaction trains the model |

[SOURCE: mysa_product_strategy.md, Part 1; CLAUDE ANALYSIS on CRM vs decision engine]

### The Shift: Why Now

Three forces converge to make this category inevitable in 2025-2027:

**1. AI Cost Collapse**
Large language models are finally accurate enough to *recommend* — not automate — expert judgment calls. The cost of processing a claim through AI has dropped to approximately $6.50/month per 100 claims. Two years ago, this was economically impossible for mid-market carriers. [SOURCE: LLM_ARCHITECTURE.md — cost estimates]

**2. Workforce Crisis**
25% of claims adjusters will retire within 5 years. The profession is the 12th fastest-declining in the US. Annual attrition runs 20% at carriers, 33% at TPAs. Each departing adjuster takes ~6 years of institutional knowledge. Carriers cannot hire or train fast enough — they need technology that makes existing adjusters 3x more productive and new adjusters effective from week one. [SOURCE: mysa_product_strategy.md, Part 2a; WEB: BLS Occupational Outlook Handbook — Claims Adjusters, Appraisers, Examiners, and Investigators (bls.gov/ooh/business-and-financial/claims-adjusters-appraisers-examiners-and-investigators.htm)]

**3. Regulatory Tailwind**
The EU AI Act is expected to classify insurance claims AI as "high-risk" under Annex III (AI systems used in insurance contexts that affect access to essential services) — requiring human oversight, conformity assessment, and transparency. This creates a regulatory moat for products built with human-in-the-loop from Day 1, and raises the bar for competitors trying to bolt AI onto legacy architecture. [SOURCE: REGULATORY_COMPLIANCE.md; mysa_product_strategy.md, Part 5d; WEB: EU AI Act (Regulation 2024/1689), Annex III]

The old way — hiring more adjusters, building more spreadsheets, adding another copilot to another CMS — is structurally broken. **The decision layer is the last unautomated, highest-value part of the claims process.** Mysa is the first product built specifically to occupy it.

---

## 1.2 ICP Deep Dive

### Three Personas, Three Selling Motions

Insurance is a multi-buyer sale. The person who uses the product every day is not the person who signs the check, and neither of them is the person who cares most about the financial impact.

#### The User: Claims Adjuster

**Who they are:** The professional who processes claims daily. Desk adjusters handle straightforward motor claims from an office. Field adjusters investigate complex or high-value claims on-site. BI (bodily injury) adjusters specialize in injury claims requiring medical assessment. SIU investigators handle suspected fraud.

**Demographics:**
- Average fully loaded cost: ~$110K/year [SOURCE: mysa_product_strategy.md, Part 2a]
- Caseload: ~125 open claims at any time, 300-480 closed per year [SOURCE: mysa_product_strategy.md, Part 2a]
- Cost per closed claim: $230-$370 [SOURCE: mysa_product_strategy.md, Part 2a]
- Aging workforce: median age skewing older, 12th fastest-declining profession [SOURCE: mysa_product_strategy.md, Part 2a — BLS]

**Daily frustrations:**
- 30-40% of time spent on administrative tasks — data entry, switching between 5-7 systems, chasing documents [SOURCE: mysa_product_strategy.md, Part 2c]
- Each claim requires 65-120 minutes of decision work [SOURCE: mysa_product_strategy.md, Part 1]
- Growing backlog of long-lasting open claims from poor decision-making and peer-review bottlenecks [TRANSCRIPT: Feb 8, 2026 — "they have more and more open claims that are long lasting"]
- Constant phone calls: 20+ per day for investigation, follow-ups, broker communications [SOURCE: claims_journey_discovery.md]
- Supervisor review bottlenecks: every decision above a threshold requires peer review, creating delays [TRANSCRIPT: Feb 8, 2026]

**Psychographics:**
- **Fear:** Being replaced by AI. Being blamed for a bad decision. Getting buried under caseload.
- **Drive:** Closing claims fairly and efficiently. Being respected for expertise. Going home on time.
- **What they want from software:** "Don't make me learn another system. Don't slow me down. Give me the right information when I need it and let me do my job."

**How Mysa helps:** Reduces decision time from 65-120 minutes to 10-15 minutes per claim. AI pre-fills coverage analysis, suggests reserves, flags fraud — but the adjuster always decides. New hires follow the same SOP-driven workflows as 10-year veterans. [SOURCE: mysa_product_strategy.md, Part 1]

#### The Buyer: VP of Claims / Chief Claims Officer

**Who they are:** The executive responsible for claims operations. Reports to CEO or COO. Manages 20-500+ adjusters depending on carrier size. At a Caravela-tier carrier (€100-200M GWP), this is typically 1-2 senior decision-makers — not an enterprise procurement committee.

**What keeps them up at night:**
- Staffing: Can't hire enough adjusters. Can't train them fast enough. Losing institutional knowledge to retirement.
- Consistency: Different adjusters make different decisions on similar claims. Lack of standardization creates audit risk.
- Cycle time: Claims take too long to close. Open claims backlog grows. Customer satisfaction drops.
- STP (straight-through processing) gap: Convention systems promise 60-70% STP — claims that can be resolved in seconds with minimal human review. Actual delivery is ~10%. The gap is data quality at intake. [SOURCE: mysa_product_strategy.md, Part 2b]

**Psychographics:**
- **Fear:** Regulatory audit failure. Major lawsuit from wrongful denial. Losing top adjusters to competitors.
- **Drive:** Operational efficiency metrics. Closing the STP gap. Getting through renewal season without a staffing crisis.
- **Buying trigger:** "I need my team handling 2-3x more claims without proportional headcount growth."

**How Mysa helps:** 3x adjuster productivity (same headcount, triple the claims handled). New adjusters productive in weeks instead of years. Consistent decisions per carrier SOPs. Measurable STP improvement. [SOURCE: mysa_product_strategy.md, Parts 1, 2a, 3a]

**Sales cycle:** At mid-market carriers (€100-200M GWP), 1-2 decision-makers, 3-6 month sales cycle. No enterprise procurement bureaucracy. [SOURCE: mysa_product_strategy.md, Part 3a — "Decision-making is fast: 1-2 decision-makers"]

#### The Influencer: CFO / Finance Director

**Who they are:** The person who cares about reserves on the balance sheet. At a Caravela-tier carrier, the CFO may be the same person as the COO — or the CEO in smaller carriers.

**Why they care:**
Reserves are money set aside for expected future claim payments. They hit the P&L immediately. Over-reserving ties up capital unnecessarily. Under-reserving creates surprise losses at year-end. The difference between a good and bad reserve estimate is the difference between a profitable and unprofitable quarter.

> At a Caravela-sized carrier (57K claims/year), a 5% improvement in reserve accuracy could mean €500K-€750K in freed capital or avoided losses per year. [SOURCE: mysa_product_strategy.md, Part 9b — ROI calculation]

**Psychographics:**
- **Fear:** Surprise reserve adjustments at year-end. Regulatory capital adequacy failure. Paying more in claims than necessary.
- **Drive:** Combined ratio improvement. Capital efficiency. Demonstrable ROI on technology spend.
- **Buying trigger:** "Show me the reserve accuracy improvement. Show me the cost per claim reduction."

**How Mysa helps:** AI-calculated reserves with confidence intervals based on historical data and comparable claims. P&L impact memos per claim. Portfolio-level reserve accuracy reporting. Every decision creates data that makes reserve models more accurate over time. [SOURCE: mysa_product_strategy.md, Part 1 — Reserve calculation sub-step]

### By Geography: EU vs US Personas

| Dimension | EU Adjuster | US Adjuster |
|-----------|------------|-------------|
| **Workflow core** | Convention systems handle inter-insurer settlement semi-automatically. These are standardized protocols — IDS in Portugal, IRSA in France, CARD in Italy, CIDE in Spain — that define rules for which insurer pays in multi-party motor claims. | No convention systems — adjuster handles everything manually |
| **Legal framework** | "Pay first, recover later" — insurer pays own policyholder, then subrogate | "Deny then defend" — insurer may deny and let claimant challenge |
| **Decision burden** | Lower for convention claims (rules are deterministic), higher for non-convention/property | Higher across the board — more investigation, more judgment calls |
| **Tool landscape** | Legacy systems, some Guidewire/Duck Creek. Many mid-market carriers on homegrown or minimal systems | More standardized on Guidewire, Duck Creek, or Salesforce. Better tooling overall |
| **Call recording** | Rarely — GDPR makes phone recording complex. Digital-first communication preferred | Standard practice — all calls recorded as evidence. Voice-first workflow |
| **Key pain point** | Data quality at convention intake (garbage in → garbage out). Property claims have zero convention systems | Everything is manual. Each state has different regulations. Colossus (the dominant software for calculating bodily injury claim values in the US, ~70% market share) dominates BI valuation |

[SOURCE: claims_journey_discovery.md — EU vs US comparison; TRANSCRIPT: Feb 9, 2026 — "EU pays first then recovers, US denies then defends"; TRANSCRIPT: Feb 5, 2026 — "US has fault vs no-fault states"]

### Carrier Segmentation (Anchored to Caravela)

| Segment | Size (GWP — Gross Written Premiums) | EU Count (16 countries) | US Count | Tech Approach | Mysa Fit |
|---------|-----------|----------------------|---------|---------------|---------|
| Enterprise | >€1B / >$5B | ~36-49 groups | ~25-30 | Build in-house (badly) | NOT NOW — these are Allianz, AXA, Generali. They build internal copilots. Phase 3+ |
| Large | €200M-€1B / $1-5B | ~60-97 | ~50-80 | Buy best-of-breed or outsource to TPA | YES — longer sales cycles but higher ACV |
| **Caravela tier (PRIMARY)** | **€100-200M / $100-500M** | **~96-165** | **~200-350** | **Need it, can't build it, ~100-200 employees** | **SWEET SPOT — fast decisions, real budget, no data science team** |
| Small | €50-100M / $50-100M | ~204-260+ | ~150-250 | Want tech help, tight budgets | YES — entry-level pricing |
| Micro | <€50M / <$50M | ~443-772+ | ~3,000+ | Manual processes, minimal tech | LONG-TAIL — self-serve or per-claim only |

[SOURCE: mysa_product_strategy.md, Part 3a — validated carrier counts per country from ASF, DGSFP, ACPR, IVASS, BaFin, NAIC data]

**Why "Caravela tier" (€100-200M) is the primary target:**
- Big enough for real claims volume (~30K-60K claims/year) that justifies investment
- Small enough to lack a data science team or in-house AI capability
- Budget exists: €50K-200K/year is 0.03-0.2% of GWP — trivial if it improves STP or reserve accuracy
- Decision-making is fast: 1-2 decision-makers, not a 12-month procurement process
- Growing fast: Caravela grew 10x in 10 years — needs tools to scale without proportional headcount

> "For the mid-market ones like Caravela, they want us."
> — Jeremy Blehaut [TRANSCRIPT: Feb 7, 2026]

> "For big carriers, it will be 'don't touch this. It's my turf. It's my logic. Build our own.'"
> — Jeremy Blehaut [TRANSCRIPT: Feb 7, 2026]

---

## 1.3 All Personas in the Ecosystem

The claims adjuster doesn't work alone. Every claim involves a network of professionals, each with distinct roles and distinct pain points. Mysa touches most of them — directly or indirectly.

| Persona | Role in Claims | How Mysa Helps | Direct User? |
|---------|---------------|----------------|-------------|
| **Desk Adjuster** | Handles straightforward claims from office. Reviews documentation, makes coverage/reserve decisions. Highest volume. | Primary user. AI pre-fills 6 decision sub-steps. 65-120 min → 10-15 min per claim. SOP-guided workflows for consistency. | **YES — primary** |
| **Field Adjuster** | Investigates complex/high-value claims on-site. Inspects damage, interviews witnesses, collects evidence. | Investigation scoping, documentation generation, call recording/transcription, evidence checklist per SOP. | **YES** |
| **BI Adjuster** | Specializes in bodily injury claims. Reviews medical records, calculates injury-related costs. Complex, high-value decisions. | Medical record parsing, comparable injury analysis, reserve calculation with BI-specific models. Integration with Colossus data where available. | **YES** |
| **SIU Investigator** | Handles suspected fraud cases referred from triage or investigation. | Fraud signal agent provides risk scoring and pattern matching. SIU referral recommendations with evidence summary. | **YES — receives referrals** |
| **Supervisor / Team Lead** | Reviews adjuster decisions above authority limits. Manages team workload and quality. | Dashboard: decision audit trail, SOP compliance scores, workload distribution, bottleneck identification. Batch review of AI-recommended decisions. | **YES** |
| **Appraiser** | Estimates physical damage value (auto, property). May be internal or external (independent adjuster). | Data feeds: claim photos, repair scopes, comparable estimates. Structured output format for Mysa to ingest back into decision workflow. | **Indirect — data exchange** |
| **Medical Case Manager** | Manages ongoing medical treatment claims. Coordinates with healthcare providers. | Treatment timeline tracking, medical cost analysis, return-to-work probability scoring. | **Indirect — data exchange** |
| **Broker / Agent** | Submits claims on behalf of policyholders. First point of contact for customer. | White-labeled FNOL forms. Chrome extension for email-to-claim creation (like Superhuman). AI gap analysis reduces back-and-forth with customers. | **YES — broker flow** |
| **TPA (Third-Party Administrator)** | Processes claims on behalf of carriers who outsource. Must follow carrier-specific SOPs. | Same product as carrier — but SOPs come from client carrier, not TPA's own. Per-claim pricing model natural fit. TPAs are a distribution channel. | **YES — same product** |
| **Underwriter** | Sets policy terms, pricing, risk appetite. Doesn't process claims — but claims data informs underwriting. | Downstream: aggregated claims decision data feeds underwriting models. Loss trend analysis from Mysa's decision ground truth. | **No — downstream data consumer** |
| **Legal / Compliance** | Reviews claims decisions for regulatory compliance. Handles litigation, bad faith allegations. | Audit trail: every AI recommendation + adjuster decision + SOP compliance status. Coverage determination letters with cited policy clauses. | **Indirect — compliance reporting** |
| **Policyholder / Claimant** | The person whose property was damaged or who was injured. Files the claim, receives the settlement. | Faster claim resolution. More consistent decisions. Better communication (AI-drafted status updates). White-labeled FNOL for self-service. | **No — end beneficiary** |
| **Repair Network** | Auto body shops, contractors, restoration companies who perform repairs. | Structured repair scope exchange. Integration with estimation tools (Xactimate, Audatex). | **No — data exchange via estimation tools** |
| **Salvage / Recovery** | Handles total-loss vehicles, damaged goods disposal. | Automated total-loss flagging based on ACV rules (70-80% threshold). Salvage process initiation. | **Indirect — triggered by decision** |
| **Arbitration / Convention Body** | Resolves inter-insurer disputes (IDS in Portugal, CIDE in Spain, etc.) | Convention matching engine: deterministic rules for CIMPAS/IDS/IRSA/CARD/CIDE. Structured data output for convention submission. | **Indirect — data feeds** |

[SOURCE: claims_journey_discovery.md — full persona mapping; TRANSCRIPT: Feb 9, 2026 — "field adjusters, BI adjusters, SIU, inside counsels, supervisor, appraiser, medical case manager"; mysa_product_strategy.md, Part 5b — agent architecture]

---

## 1.4 Core Value Proposition

### The Mad-Lib

> **For** mid-market insurance carriers (€100-200M GWP) **who** struggle with adjuster productivity, decision consistency, and knowledge loss from workforce turnover,
> **Mysa is a** claims decision engine **that** encodes each carrier's SOPs into AI-guided workflows, helps adjusters make coverage, liability, and reserve decisions 4-8x faster, and captures decision reasoning as proprietary training data.
> **Unlike** claims copilots (Five Sigma/Clive) that offer generic playbooks, or intake automation tools (Assured, Avallon) that only speed up data entry,
> **Mysa** targets the decision layer that nobody else has built — the 6 expert judgment steps that consume 60-70% of adjuster time — and creates a compounding data moat from every claim processed.

[SOURCE: mysa_product_strategy.md, Part 1 — positioning, decision sub-steps, time estimates; Part 3a — ICP segmentation; Part 4 — competitive differentiation]

### The Value Stack

| Value Layer | What It Means | For Whom | Metric |
|-------------|--------------|---------|--------|
| **Adjuster Productivity** | Decision time drops from 65-120 min to 10-15 min per claim (4-8x on the decision step, which consumes ~60-70% of adjuster time). Net effect: same headcount handles 2-3x total claims, because administrative tasks remain. | VP Claims / Operations | Claims closed per adjuster per year |
| **New Hire Acceleration** | SOP-driven workflows mean a new adjuster follows the same process as a 10-year veteran from Day 1 | VP Claims / HR | Time to full productivity (6 years → weeks) |
| **Decision Consistency** | Every claim processed per carrier's own SOPs. No more "it depends on which adjuster you get" | Compliance / Legal | Decision variance across adjusters |
| **Reserve Accuracy** | AI-calculated reserves with confidence intervals. P&L impact visible per claim | CFO / Finance | Reserve development ratio, surprise adjustments |
| **STP Improvement** | Fix data quality at intake → more claims qualify for STP (straight-through processing — near-instant resolution) | COO / VP Claims | STP rate (target: 10% → 40-50%) |
| **Knowledge Preservation** | Tribal knowledge encoded into workflows. Expertise doesn't retire with the adjuster | CEO / Board | Institutional knowledge captured as system knowledge |
| **Compliance Trail** | Every decision documented: AI recommendation, adjuster action, SOP compliance, cited policy clauses | Legal / Compliance | Audit readiness, bad-faith defense |

[SOURCE: mysa_product_strategy.md, Parts 1, 2a-2d, 5d; TRANSCRIPT: Feb 8, 2026 — productivity calculations, new hire value]

---

## 1.5 The Company Description

### Investor Version (Pitch Deck, Data Room, Formal Communications)

> At Mysa, we believe that claims adjusters are the most underserved decision-makers in financial services. They handle coverage, liability, and reserves — high-stakes calls that directly hit a carrier's P&L — using fragmented data scattered across 5-7 systems, under time pressure, with institutional knowledge that walks out the door when 25% of them retire in the next five years.
>
> The industry's response has been to automate intake — digitize paperwork, speed up FNOL. Billions invested. Nobody touches what happens after. The decision layer — where adjusters actually think — is still manual, inconsistent, and unscalable.
>
> We're building the decision layer. Mysa is an AI decision engine that encodes each carrier's SOPs into workflows, learns from every adjuster interaction, and turns tribal knowledge into institutional advantage. We start where adjusters already work, augment their judgment (never replace it), and build the only dataset that captures not just what was decided, but why.

[SOURCE: Plan — Appendix A, Draft 1; informed by TRANSCRIPT: Feb 7, Feb 8, Feb 9 calls]

### Sales Version (First Call with VP Claims)

> We help claims adjusters make better decisions, faster. Right now your adjusters spend 30-40% of their time on admin — entering data, switching between systems, chasing documents. The actual decision-making — coverage, liability, reserves — gets squeezed into whatever time is left.
>
> Mysa sits on top of your existing systems. We don't change how you do intake. We take the SOPs your team already follows, encode them into AI-guided workflows, and give each adjuster a copilot that knows your carrier's rules, your authority levels, your convention system. Claims that take 65-120 minutes today take 10-15 with Mysa.
>
> The result: your adjusters handle 2-3x more claims. New hires get productive in weeks instead of years. And every decision builds a dataset that makes the system smarter over time.

[SOURCE: Plan — Appendix A, Draft 2; TRANSCRIPT: Feb 9, 2026 — "adjuster copilot and orchestrator that's proactive at every step... not only removing manual work but empowering the decision-making process"]

### Technical / Integration Version

> Mysa is an AI decision engine that sits on top of existing claims management systems. We integrate with your CMS, estimation tools, and convention platforms — adding a decision intelligence layer without replacing your stack. Adjusters get AI-guided workflows based on carrier-specific SOPs. Carriers get consistent decision-making at scale. Every interaction builds a knowledge base that compounds over time.

[SOURCE: Plan — Appendix A, Draft M3]

### The Blunt Version (Internal Alignment)

> Claims adjusters make $100K+ decisions every day using PDFs, phone calls, and gut instinct. The tools they have are either 20 years old or built for a different problem. Every startup in insurance AI is doing one of three things: intake automation (crowded), fraud detection (crowded), or estimation tools (dominated by Verisk). Nobody is touching the actual decision — because it's hard. You need to understand insurance domain deeply AND build good AI. That combination barely exists.
>
> We have it. Tiago brings deep claims domain expertise. Jeremy brings product and technical execution. We built a working OCR + decision support system for a Portuguese carrier in 8 weeks. Now we're turning that into a product that encodes any carrier's SOPs into AI-guided workflows.
>
> The bet: if we own the decision layer, we own the most valuable data in insurance — not what was paid, but why. That's the moat.

[SOURCE: Plan — Appendix A, Draft 7; informed by all Granola transcripts Feb 5-9]

---

## 1.6 Product Now vs Product Tomorrow

### Product Now (February 2026)

**What exists today:**

| Component | Status | Detail |
|-----------|--------|--------|
| **Caravela OCR Engine** | Live, 81.5% normalized accuracy | Gemini 3 Flash Preview, x3 voting, GOLDEN RULES for field normalization. 44 claims with ground truth. Processing Portuguese motor claims (EAS forms, invoices, photos). |
| **Convention Matching** | Built for Portugal | IDS/CIMPAS rules encoded. 91% inter-insurer agreement rate. Deterministic lookup from structured EAS data. |
| **Benchmark System** | Operational | benchmark-with-db.ts — tracks accuracy across models, stores results in Supabase. |
| **Caravela Commercial Deck** | Live | 12-slide pitch at caravela.mysa-health.com. Commercial deck at /commercial. Design partner conversations active. |
| **Marketing Site** | meetmysa.com | Needs update to reflect claims positioning (currently healthcare-era content). |

[SOURCE: caravela-ocr.md (memory file) — accuracy metrics, model details; mysa_product_strategy.md, Part 5c — tech stack; Caravela slides found in app/caravela/page.tsx]

**What it proves:** We can read insurance documents with AI, structure the data, and match it against convention rules — the foundational capability that everything else builds on.

**What it doesn't do yet:** Coverage determination, reserve calculation, fraud detection, investigation support, SOP-driven workflow generation, multi-carrier support, broker flow.

### Product Tomorrow (12-18 Month Vision)

**The operating system for claims adjusters globally** — an SOP-driven decision engine that learns from every claim.

| Capability | Timeline | Description |
|-----------|----------|-------------|
| **SOP Workflow Engine** | Months 1-3 | Upload carrier SOPs → AI generates decision workflows → adjuster follows carrier-specific steps |
| **6 Decision Sub-Steps** | Months 2-6 | Coverage verification, policy checking, repair assessment, cost analysis, reserve calculation, fraud detection — each with AI recommendation + confidence score |
| **Chrome Extension / Clippy** | Months 3-6 | "Insurance knowledge Clippy" — sits on top of whatever system the adjuster uses. Like Superhuman for email. Context-aware across all pages. Chat with Vault knowledge base. |
| **Broker FNOL Flow** | Months 2-4 | White-labeled intake forms. Email → claim creation. AI gap analysis. Removes broker ↔ customer back-and-forth. |
| **Multi-Carrier** | Months 4-8 | Same platform, different SOPs per carrier. Spain (CIDE), France (IRSA), Italy (CARD). |
| **Investigation Support** | Months 4-8 | Scoping, call recording/transcription, document generation, investigation checklist per SOP |
| **Decision Ground Truth** | Months 6-12 | Every adjuster accept/modify/reject captured as training data. Models learn carrier-specific decision patterns. |
| **Property Module** | Months 8-14 | Coverage determination (no convention system). Water damage, fire, storm. Same 6 decision sub-steps but different data sources. |
| **Historical Data Ingestion** | Months 3-6 | Ingest carrier's historical claims → pre-configure comparable matching → Day 1 value from existing data |
| **Near-STP** | Months 12-18+ | Routine claims processed with minimal human review. Complex claims still human-decided but AI-pre-populated. |

[SOURCE: mysa_product_strategy.md, Part 5a — product flow; TRANSCRIPT: Feb 9, 2026 — Clippy/Superhuman architecture, Vault, Chrome extension; TRANSCRIPT: Feb 9, 2026 — "the product is proactive on every single step"; mysa_product_strategy.md, Part 1 — flywheel timeline]

**The key distinction:** Today's product is a document processing engine for one carrier. Tomorrow's product is the decision layer for any carrier, any line of business, learning from every claim. The OCR/document AI is a means — the decision engine is the end.

---

## 1.7 Founder-Market Fit

### This Is a Market-Pull Story, Not a Pivot Story

Mysa didn't start by deciding to build claims AI. Insurance companies pulled the founders in.

> "We didn't set out to build claims AI. Insurance companies pulled us in. While building healthcare pre-authorization tools, we kept hearing the same thing from carriers: 'Our real problem isn't intake — it's what happens after. Our adjusters are drowning.'"
> [SOURCE: Plan — Appendix A, Draft 6]

The origin: Jeremy and Tiago were building healthcare pre-authorization tools (the original Mysa product for clinics — code mapping, insurer rule management, denial prevention). Through that work, they built relationships with insurers — including AdvanceCare/Generali and Caravela. Those conversations surfaced a much bigger, more urgent problem: claims adjustment.

The specific pull: Caravela, a Portuguese insurer (€188M GWP, 57K claims/year, 7th in Portuguese non-life), became a design partner. They needed help digitizing their EAS (European Accident Statement) forms and improving claims processing. That pilot — 8 weeks from start to working OCR engine — validated both the technology and the market need.

[SOURCE: mysa_product_strategy.md, Part 6a; AI_NATIVE_ARCHITECTURE_SPEC.md — AdvanceCare/Generali meeting; TRANSCRIPT: Feb 7, 2026 — Caravela partnership details]

### The Founders

**Tiago Brigido — Co-founder, Domain Expert**

[PLACEHOLDER — Bio to be provided by Tiago]

Key qualifications surfaced from calls:
- Deep insurance claims domain expertise — understands SOPs, convention systems, adjuster workflows, carrier operations at a practitioner level
- Network in Portuguese insurance market (Caravela, Fidelidade connections)
- Understands the EU regulatory landscape (GDPR, convention systems across countries)
- Can speak the language of VP Claims buyers — not selling technology, selling operational improvement

> "It's basically, I'm getting, you are hiring me and you need to onboard me. Need to tell me exactly how I am working." — Tiago, explaining SOPs [TRANSCRIPT: Feb 9, 2026]

> "Everyone is avoiding the judgment, the decision stage." — Tiago [TRANSCRIPT: Feb 7, 2026]

**Jeremy Blehaut — Co-founder, Product & Technology**

[PLACEHOLDER — Bio to be provided by Jeremy]

Key qualifications surfaced from calls:
- Built the Caravela OCR engine (81.5% accuracy) in 8 weeks using Gemini
- Technical product execution — Next.js, Supabase, Vercel, LLM integration
- Product instinct for positioning and go-to-market (framed "decision engine" category, identified mid-market ICP)
- Previous experience building AI products (healthcare pre-auth tools)
- Fundraising experience and investor network

> "For the mid-market ones like Caravela, they want us." — Jeremy [TRANSCRIPT: Feb 7, 2026]

> "Right now, I went for Gemini because it's us. But if we wanted to build a really robust thing, we could go somewhere else." — Jeremy [TRANSCRIPT: Feb 7, 2026]

### Why This Team, Specifically

The decision layer hasn't been built because it requires **both** deep insurance domain expertise AND modern AI engineering capability. That combination barely exists:

| Requirement | Why It's Hard | How Mysa Has It |
|-------------|--------------|-----------------|
| Insurance domain depth | Convention systems, SOPs, adjuster workflows, carrier operations — this takes years to learn | Tiago's practitioner-level domain knowledge |
| AI/LLM engineering | Production OCR, agent architectures, prompt engineering at scale | Jeremy's working system (81.5% accuracy on real claims) |
| Carrier relationships | Mid-market carriers are hard to reach without network | Tiago's Portuguese insurance network, Caravela partnership |
| EU regulatory knowledge | GDPR, AI Act, per-country insurance regulation | Both founders EU-based, building compliance-first |
| Speed of execution | 8 weeks from concept to working OCR — typical insurtech takes 12-18 months for less | Proven: Caravela pilot is live |

> "Everyone is trying to build a platform. And everyone is avoiding the hard part — the judgment, the decision stage. They'll parse your documents, they'll route your claims, they'll score your fraud risk. But the moment an adjuster needs to decide 'is this covered, what do I owe, and why' — they're on their own. We built the decision layer."
> [SOURCE: Plan — Appendix A, Draft 3 — Tiago's voice]

---

## 1.8 One-Liner + Elevator Pitches

### One-Liners (by context)

| Context | One-Liner |
|---------|-----------|
| **Website hero** | The AI decision engine for insurance claims adjusters |
| **Sales intro** | We help adjusters make better decisions, faster — without changing how you work |
| **Investor hook** | Everyone automated intake. Nobody built the decision layer. We did. |
| **Investor hook (data)** | Billions poured into claims intake automation. $0 into claims decision intelligence. That's where we are. |
| **Technical** | A compiler for claims decisions — SOPs in, consistent outcomes out |
| **Broker pitch** | Create a claim from an email. We handle the rest. |
| **Workforce angle** | 25% of adjusters retire in 5 years. Their expertise doesn't have to retire with them. |
| **Data moat** | We capture why decisions are made, not just what was decided. Nobody else has this data. |
| **Casual / cocktail** | You know how AI is changing how lawyers work? We're doing the same thing for insurance claims adjusters. |

[SOURCE: Plan — Appendix, one-liner variants]

### 30-Second Elevator Pitch

> Insurance claims adjusters make high-stakes coverage and liability decisions — hundreds per week — using PDF printouts, phone calls, and gut instinct. The industry spent billions automating the data entry before the decision — over $1B into Assured alone, $320M into Shift Technology, $30M into FurtherAI [WEB: Crunchbase]. Nobody automated the decision itself. Mysa is the AI decision engine that does. We encode each carrier's procedures into AI-guided workflows, so adjusters handle 3x more claims, new hires perform like veterans, and every decision trains a smarter system. We're live with a Portuguese carrier and expanding across Southern Europe.

### 2-Minute Elevator Pitch

> Every year, insurance adjusters across the US and Europe process an estimated 80-95 million claims [SOURCE: mysa_product_strategy.md, Part 3b — ~45-50M US + ~55-70M EU, validated via NAIC and EIOPA data]. For each one, they make six judgment calls: Is this covered? What does the policy say? Is the repair reasonable? What does it cost? How much should we reserve? Is this fraud? Today, each of those calls takes 10-30 minutes of manual work — checking 5-7 different systems, reading through policies, comparing against historical claims.
>
> The industry has invested billions automating what comes before those decisions — intake automation, document parsing, chatbots. But the decision itself — the part that actually determines what gets paid and why — is untouched. It's manual, inconsistent, and unscalable. And 25% of the people who make those decisions are retiring in the next five years.
>
> That's what Mysa builds. We take each carrier's standard operating procedures — the rules their adjusters are supposed to follow — and encode them into AI-guided decision workflows. An adjuster gets a claim, and Mysa walks them through coverage, liability, reserves, and fraud checks per their carrier's own rules. Claims that take 65-120 minutes today take 10-15 with Mysa. New adjusters follow the same SOP-driven workflows as 10-year veterans. And every decision an adjuster makes trains the system — we capture not just what was decided, but why.
>
> We're starting in European motor claims — Portugal, Spain, France, Italy — where convention systems give us a technical wedge nobody else has. Our design partner is a €188 million Portuguese carrier. Same buyers write property insurance, which adds 60-70% revenue per carrier. The EU mid-market — 96-165 carriers in our primary tier, 200+ including adjacent segments — is 90-95% untouched by AI claims tools.
>
> We're Tiago and Jeremy. Tiago brings deep claims domain expertise — he understands SOPs, convention systems, and carrier operations at a practitioner level. Jeremy built the OCR engine that reads claims documents at 81.5% accuracy in 8 weeks. Insurance companies pulled us into this — we didn't go looking for it.

### 5-Minute Pitch

*The 2-minute pitch above, plus:*

> **The competitive landscape:** Over $1B raised by Assured alone for intake automation, $30M by FurtherAI, $4.6M by Avallon [WEB: Crunchbase]. $320 million into Shift Technology for fraud [WEB: Crunchbase]. Verisk, a $35B public company, dominates estimation [WEB: NYSE: VRSK]. Zero invested in the decision layer. The closest competitor is Five Sigma — $10 million revenue, 180% year-over-year growth — but they're a CMS with generic AI playbooks, not a decision engine with carrier-specific SOP workflows. They don't do convention systems. They don't capture decision reasoning. They serve mostly US carriers. The EU mid-market is wide open.
>
> **Why now:** Three things converged. LLMs are finally accurate enough to recommend expert judgment — not automate it, recommend it. The workforce crisis is creating urgent buyer need that can't wait for 12-month enterprise procurement cycles. And the EU AI Act creates a regulatory moat for products built with human-in-the-loop from Day 1.
>
> **The moat:** Three layers. First, convention system intelligence — country-by-country expertise that takes years to replicate. Second, SOP-encoded workflows — once a carrier's procedures are in Mysa, switching costs are prohibitive. Third, decision ground truth data — we capture the reasoning behind every decision, not just the outcome. That's a new data category that nobody else has. CCC and Verisk have claim outcomes. Anthropic and OpenAI have general intelligence. We have adjuster decision reasoning.
>
> **The business model:** Per-claim SaaS (landing) plus platform license (expansion). €50K-€2M per carrier per year depending on size. We start with EU motor — 54-93 carriers in our primary target across four countries. Same carriers write property, adding 60-70% revenue with zero new customer acquisition. EU plus US mid-market: €160-425 million TAM.

[SOURCE: mysa_product_strategy.md, Parts 1-9; all Granola transcripts Feb 5-9; Plan — all appendix variants]

---

## Unresolved Positioning Tensions

The founder calls reveal competing framings that Module 1 presents but does not resolve. Jeremy and Tiago should lock these during review.

| Tension | Option A | Option B | Founder Positions |
|---------|----------|----------|-------------------|
| **Category name** | "AI decision engine" | "Copilot + orchestrator" / "Compiler" | Jeremy leans "decision engine" (Feb 8: "AI decision engine for insurance claims adjusters"). Tiago says "copilot and orchestrator" (Feb 9) and previously used "compiler" framing (Feb 7). |
| **Lead positioning** | Decision layer (nobody else does it) | Intake + decision (we fix garbage-in AND decide) | Both agree decision is the moat. But intake is the wedge — Tiago: "The intake is non-negotiable. We need to do the intake very well." [TRANSCRIPT: Feb 9] |
| **Audience framing** | Investor: workforce crisis + category creation | Sales: "I don't change how you do intake, I help with the decisions you already make" | Different language for different rooms. Both needed. This module provides both. |
| **Moat claim** | "Nobody has built the decision layer" | Historical data flywheel + SOP lock-in | First is punchier. Second is more defensible. Recommendation: lead with "nobody built it" for attention, follow with data flywheel for substance. |

**Recommendation:** Use "AI decision engine" as the primary category. Use "copilot and orchestrator" as the product description (what it feels like to use). Use "compiler" for technical audiences ("SOPs in, consistent outcomes out"). These aren't contradictions — they're different lenses on the same product for different audiences.

[SOURCE: TRANSCRIPT: Feb 7, Feb 8, Feb 9 calls — all positioning discussions]

---

## Sources

| Source | Type | Sections Used |
|--------|------|--------------|
| `mysa_product_strategy.md` Parts 1-3, 5 | Primary — positioning, ICP, product architecture | 1.1-1.4, 1.6, 1.8 |
| Feb 9 Granola call — Claims workflow | Transcript | 1.1, 1.3, 1.5, 1.6, Tensions |
| Feb 9 Granola call — Market strategy | Summary | 1.2, 1.7 |
| Feb 8 Granola call — Strategy review | Transcript | 1.1, 1.2, 1.4, 1.6, Tensions |
| Feb 7 Granola call — Mid-market strategy | Summary | 1.1, 1.2, 1.7, Tensions |
| Feb 5 Granola call — Workflow analysis | Summary | 1.2 (EU vs US) |
| `AI_NATIVE_ARCHITECTURE_SPEC.md` | Secondary — architecture philosophy | 1.1, 1.6 |
| `LLM_ARCHITECTURE.md` | Secondary — cost estimates | 1.1 |
| `REGULATORY_COMPLIANCE.md` | Secondary — EU regulatory framework | 1.1 |
| `caravela-ocr.md` (memory) | Internal — accuracy metrics | 1.6 |
| Plan — Appendix A (company descriptions) | Plan document — drafted variants | 1.5, 1.8 |
