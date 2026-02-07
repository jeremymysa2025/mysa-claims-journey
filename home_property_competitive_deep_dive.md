# Home/Property Claims — Deep Competitive Landscape

*Research date: February 7, 2026*

---

## TL;DR — The Honest Picture

**The property claims adjuster market is NOT wide open.** The big TPAs (Sedgwick, Crawford, Davies) are investing heavily in AI and workflow tools. But there is a genuine, confirmed gap: **nobody has built the unified "adjuster operating system" for property claims.** The field remains fragmented point solutions — adjusters use 5-6 separate systems per claim. The question is whether that gap is an opportunity or a feature of the market (i.e., it stays fragmented because no one can unify it).

---

## 1. The Big TPAs Are NOT Sitting Still

### Sedgwick ($5B revenue, 33,000+ employees, valued at $13.2B)

**What they've built:**
- **smart.ly** — Cloud-based multilingual intake portal with AI triage, RPA, OCR, and auto-adjudication for simple claims. Won CIO 100 Award. Genuinely sophisticated for intake.
- **Sidekick Agent** (April 2025) — Agentic AI built on Azure OpenAI/GPT-4. The only **validated** capability is medical document summarization (98%+ accuracy on 50,000+ documents). The "real-time guidance," "claim trajectory forecasting," and "next best action" features are marketing-heavy, specifics are thin.
- **Digital Adjust Pro** (May 2025) — NOT software. It's a managed service/BPO offering — experienced desk adjusters + Sedgwick's tech stack, outsourced to carriers. Claims up to $100K. 81% NPS.
- **Lightning App** (July 2025) — Mobile app for field adjusters. View loss details, capture photos, enter scope data, sync to JURIS. Standard field inspection app — not AI-powered, not differentiated.
- **viaOne** — Client analytics platform. Mature RMIS but built on older Oracle architecture. Migrating to Snowflake with Kipi.ai.

**What they DON'T have:**
- No proprietary AI model — entirely dependent on Microsoft/Azure/OpenAI
- No property damage estimation tool (they use Xactimate like everyone else)
- Lightning app is catch-up, not innovation
- AI is narrow: document summarization works, "agentic" claims are aspirational
- JURIS (their core CMS) is legacy Oracle-based architecture
- **They do NOT license their technology.** You can't buy Sidekick or JURIS — you must buy the full TPA service.

**Glassdoor: 3.2/5, 54% recommend.** Low pay, high turnover, poor training. The tech may be good but the people operating it are under stress.

Sources: Sedgwick press releases, Computerworld CDO interviews, CIO 100 Awards, Glassdoor

---

### Crawford & Company ($1.29B revenue, ~9,000 employees, public NYSE: CRD)

**What they've built:**
- **Turvi** (launched 2025) — Standalone insurtech subsidiary, spun out to sell AI tools to the broader market. Three products:
  - **CoverAI** — AI-driven policy coverage review. Interprets complex policy language for faster coverage decisions.
  - **Asservio** — Digital estimate review tool.
  - **Digital Desk** — Claims triage solution.
- **Contractor Connection** — Largest independently-managed contractor network. 6,000+ vetted contractors, 350,000 annual assignments, $2.5B in project costs. This is a real competitive advantage for property.
- **edjuster/exclaim** (acquired 2021) — Digital contents valuation. LKQ matching, 40% adjuster productivity improvement for contents claims.
- **WeGoLook** — 45,000+ gig-economy inspectors ("Lookers") for on-demand field documentation. Average 1.6 days from loss notification to report. Still active but quality concerns (2.2/5 compensation rating).
- **YouGoLook** — Policyholder self-service photo/documentation app.

**What they DON'T have:**
- Turvi is very early stage (3 products, 2025 launch, startup within a corporation)
- No equivalent to Sedgwick's agentic AI claims agents
- WeGoLook is low-skill inspection, not professional adjusting
- Public company constraints limit tech investment vs PE-backed competitors
- January 2026 global restructure into US/International divisions creates transition risk

**Strategic move:** Crawford is the only big TPA trying to **sell** AI tools externally (via Turvi) rather than just using them internally. This is significant — it means they see a market for standalone claims AI.

Sources: Crawford innovation pages, Turvi launch coverage, edjuster acquisition, WeGoLook reviews

---

### Davies Group (~$1.7B revenue, 8,500+ employees, UK-based)

**What they've built:**
- **ClaimPilot** (acquired 2023) — SaaS CMS for TPAs, independent adjusters, and self-insured entities. Property, liability, workers comp, auto. 99% client retention. 81+ organizations. **This is licensed externally** — it was a standalone product before Davies bought it.
- **Agentic AI Agents** (H2 2025) — Two LLM-powered agents:
  - **Claim Opening Agent** — Auto-reads incoming documents, opens claims autonomously, escalates ambiguity to humans. Self-learning.
  - **Validation & Injury Valuation Agent** — Automates claim validation and BI injury valuation. Combines LLMs with traditional data science.
- **E-claim** — UK digital FNOL-to-settlement platform. Reduces cycle by up to 70%. Customers self-serve the entire journey.
- **Vision 2030** — Grow from ~$1B to $2.5-3B by 2030. $370M Blackstone credit facility specifically for M&A + GenAI investment.
- **SCM Insurance Services** (acquired Nov 2025) — Canada's largest claims processor. Adds ClaimsPro (adjusting), IPG (TPA), Pario (forensic engineering).

**What they DON'T have:**
- AI agents are **casualty-focused** (claim opening + injury valuation). No property-specific AI agent for damage assessment, estimate review, or scope validation.
- Multi-platform integration risk: ClaimPilot (US), E-claim (UK), ClaimsPro (Canada) are three different systems.
- Agentic AI is brand new (H2 2025) — unproven at scale.
- 50+ acquisitions in 10 years = significant integration debt.

**Key distinction:** Davies is the only big TPA that **licenses ClaimPilot externally as standalone SaaS.** They are both a TPA and a tech vendor.

Sources: Davies announcements, ClaimPilot features page, Insurance Edge, Reinsurance News

---

## 2. The Measurement/Documentation Layer

### Hover ($136.7M raised, $490M post-money valuation at Series D)

**What they do:** Smartphone photos → accurate 3D property models. Exterior measurements, now expanding to interior.

**Key facts:**
- 22 billion sq ft of digitally reconstructed property (massive data moat)
- "9 of top 10 insurance carriers" (unnamed) use Hover
- Investors include Travelers, State Farm, and Nationwide (Series D)
- 40% revenue growth in 2024
- 300,000+ insurance and construction professionals use it
- Saves carriers $400-500 per claim vs. traditional inspection

**Recent expansion:**
- **Interior solution + Virtual Walkthrough** (April 2025) — Moving from exterior-only to full property documentation
- **Guided Estimates** — Generates material line items and quantities from 3D measurements, flows directly into Xactimate
- **Inspections** — Photo-driven checklist for carrier-compliant loss documentation
- Now embedded **within Xactimate** (Verisk partnership)

**What Hover is NOT:**
- Not a claims workflow system. It's measurement + documentation.
- No triage, no task management, no reserve calculation, no correspondence
- Expanding toward estimation but not toward full adjuster workflow
- Still a point solution, not an operating system

**Competitors in measurement:** EagleView (aerial imagery, 3B+ photos, 94% US coverage), Nearmap, CAPE Analytics, Cotality/CoreLogic Claims Scope

Sources: Hover press releases, Verisk partnership announcement, TechCrunch, Seeking Alpha

---

### CAPE Analytics (property intelligence from aerial imagery)

- 80+ property insights via computer vision/ML (roof condition, age, risk scores)
- **Hail Roof Damage Rating** (with Canopy Weather) — predicts post-storm roof damage with 96%+ accuracy. Can identify claims eligible for straight-through processing within hours of a hailstorm.
- Primarily **underwriting-focused** but has clear claims applications (CAT triage, proactive claims outreach)
- Expanded Hail Intelligence Suite (2024): Hail Experience Rating, Vulnerability Rating, Risk Rating, Loss Severity Rating

### EagleView (aerial imagery leader)
- 3+ billion high-res property photos, 94% US population coverage
- 20+ year archive
- Roof measurement, damage assessment, underwriting
- Complementary to Hover (aerial vs. ground-level)

---

## 3. The Estimation Layer (The Real Monopoly)

### Xactimate / Verisk — The 800-Pound Gorilla

- **75-80% of ALL property claims** are estimated using Xactimate
- Virtually every TPA, carrier, and independent adjuster uses it or integrates with it
- **Any tool selling to property claims MUST integrate with Xactimate data** — this is non-negotiable
- Verisk is actively building ecosystem around Xactimate: XactAnalysis (workflow), XactContents (contents valuation), Hover integration, Claims Connect
- **But:** Xactimate is estimation-centric, not a full adjuster workflow system

### Cotality / CoreLogic (Symbility) — Distant #2
- **Symbility** — the main Xactimate competitor. Cheaper, mobile-first, more flexible reports
- Liberty Mutual switched from Xactimate to Symbility
- **Claims Scope** — automated roof estimate generation from measurements
- **Claims Estimate** — full estimating platform with monthly pricing updates
- Xactimate estimates tend to run 15-20% higher than Symbility for same line items

---

## 4. Assured — The Direct Competitor We Missed

### Assured ($1B valuation, ~65 employees, Palo Alto)

**Founded:** 2019 by Justin Lewis-Weber (CEO, Stanford aero/astro) and Theo Patt (CTO)
**Funding:** Series A at $1B valuation (March 2025), backed by ICONIQ Capital + Kleiner Perkins
**Traction:** 50+ million customer interactions for "the largest insurers in the world"

**This is essentially the "adjuster operating system" that the Mysa discovery doc was describing.** Their platform:

| Module | What It Does |
|---|---|
| **Digital FNOL** | Self-service intake with dynamic question flows, 50+ external data sources, 3D vehicle damage painting, auto-translate, digital signatures |
| **Emma** (AI agent) | Handles **70% of interactions autonomously** — collects docs, photos, medical releases, sends reminders, answers questions. Delegates to adjusters when empathy/judgment needed. 50M+ interactions processed. |
| **Messaging** | Omnichannel (SMS, chat, etc.) between adjusters, claimants, service providers |
| **First Contact** | Digital follow-up — questions, document gathering, service assignment |
| **Sidekick** | Standardizes contact center interactions |
| **Fraud Detection** | Built-in: prevent, corroborate, validate |
| **CAT** | Catastrophe prediction, preparation, recovery |
| **Flow Builder** | Low-code customization of question sequences by LOB/location |
| **ClaimView** | Adjuster dashboard |
| **Customer360** | Analytics + session replays |

**Key design:** They explicitly "augment your core system, not replace it" — layers on top of Guidewire, Duck Creek, etc. Modular, line-of-business-specific. Covers "every major P&C line."

**Where Assured is strong:** Auto claims (3D vehicle damage model, collision dynamics, child safety seats). 70% autonomous interaction rate. Deep FNOL. Omnichannel communication.

**Where Assured appears weak:**
- Product examples are heavily **auto-focused** — no evidence of property-specific features
- No mention of Xactimate integration, field inspection workflows, scope-of-loss, contractor coordination, or supplement cycles
- No EU convention system support (IRSA, CARD, IDS, CIDE)
- No evidence of EU operations or GDPR/AI Act compliance positioning
- US-only as far as can be determined

**Implication for Mysa:** For US motor claims, Assured is essentially what Mysa was envisioning, years ahead with $1B in backing. For EU motor and for property claims, the gap remains.

Sources:
- [Bloomberg — Assured $1B Valuation](https://www.bloomberg.com/news/articles/2025-03-04/iconiq-kleiner-perkins-back-insurance-startup-assured-at-1-billion-valuation)
- [Assured Platform](https://www.assured.com/platform)
- [Assured Emma](https://www.assured.com/emma)
- [Assured FNOL](https://www.assured.com/fnol)
- [Tracxn Profile](https://tracxn.com/d/companies/assured-insurance-technologies/__iDb1wUZyPNvXT9_-KxRcoK6_-92koK9yUlkXckTIjHY)

---

## 5. The AI Startup Wave (Horizontal, Not Property-Specific)

| Company | Funding | What They Do | Property-Specific? |
|---|---|---|---|
| **Assured** | $1B valuation | Most deployed agentic AI in P&C. AI agent "Emma" for omnichannel messaging. FNOL + STP. | No — all P&C |
| **Five Sigma / Clive** | ~$20M | AI claims adjuster multi-agent system on top of existing CMS | No — all P&C |
| **FurtherAI** | $30M (a16z) | AI workforce for insurance. 30x faster intake, 95% accuracy. | No — all lines |
| **Avallon** | $4.6M (YC) | AI agents for calls, docs, data entry. 10x revenue growth during YC. | No — all lines |
| **Agentech** | $3M seed | 100+ AI agents per claim file. 4x output increase. NVIDIA Inception. | No — all P&C |
| **Elysian** | $6M seed | AI-native TPA for commercial insurance. Dynamic Claim Review. | No — commercial |
| **ClaimSorted** | $3.5M (YC) | AI-first TPA. 3-10x faster processing. | No — all lines |
| **Sprout.ai** | $38M | Document AI, 98% accuracy, 100+ languages. | No — all lines |
| **Reserv** | $55M | Full-stack AI-native TPA. 80+ MGA clients, 20+ carriers. | No — all lines |
| **MarvelX** | €5.4M (2025) | Amsterdam. "ClaimOS MaX" — EU-first agentic AI for claims processing, fraud detection, customer comms. | No — all lines, EU-first |
| **omni:us** | ~€45M | Berlin. End-to-end claims AI. 70% auto-settlement. Allianz Austria customer. | No — all lines, EU-strong |

**The pattern:** Every funded startup is building horizontal (all P&C lines) AI that layers on top of existing CMS. **Nobody is building property-specific.** They automate intake, triage, document processing, and correspondence — but they don't touch the property-specific workflow (field inspection, scope creation, Xactimate integration, contractor coordination, supplement cycles).

**EU-specific note:** MarvelX (Amsterdam, €5.4M, founded 2025) is the closest to an "EU Assured" — building ClaimOS MaX as an EU-first agentic AI platform for insurers. omni:us (Berlin, ~€45M) has real EU traction with Allianz Austria. Both are early but represent the EU thesis being pursued.

---

## 5. Property-Specific Tools (Fragmented Point Solutions)

| Tool | What It Does | Who Uses It | Notes |
|---|---|---|---|
| **Encircle** | Field documentation: photos, videos, floor plans, moisture readings, contents inventory | Restoration contractors, adjusters, carriers | Professional-grade field docs. Not a CMS. |
| **n2uitive** | Recorded statement lifecycle management. AI SummaryAssist saves 30 min/statement. | 40+ insurers/TPAs, 10,000+ adjusters/month, 25M+ statements | Not property-specific — all P&C lines |
| **BuildArray** | Mobile field inspection/scoping forms. Offline-capable. Standardized scope reports. | Independent adjusters, field teams | Scoping only, not full workflow |
| **Magicplan** | AR-based floor plan creation from mobile phone | Adjusters, policyholders | Interior measurement only |
| **Encircle** | Field documentation (photos, video, floor plans, moisture, contents) | Contractors, adjusters | Documentation layer only |
| **Dragonfile** | CMS for flood and P&C adjusters. Workflow, tasks, mobile, analytics. | Flood adjusters, P&C adjusters | Niche, recently launched DragonfileONE for solo adjusters |
| **VCA Software** | Cloud CMS for IA firms, TPAs, self-insured. Auto, property, liability, CAT. | Mid-market IA firms, TPAs | More enterprise-grade but not property-specific |
| **ClaimWizard** | CRM for public adjusters (policyholder side). $99/mo starting. | Public adjusting firms | Wrong side of the market for Mysa |
| **Claim Titan** | CRM for property claim professionals. | Public adjusters, contractors | Same — policyholder side |
| **Brush Claims** | Tech-enabled TPA. Hubvia platform + HubOnsite field app. | Carriers needing outsourced adjusting | Services + tech bundled |
| **Brelly** | AI Claims Copilot for public adjusters. Reviews damage docs, codes, estimates. | Public adjusters, policyholders | Policyholder side |

---

## 6. The TPA Buyer — Can a Startup Actually Sell to Them?

### Market Size
- US insurance TPA market: **$115B (2024) → $255B by 2034** (8.3% CAGR)
- Property-specific TPA segment: estimated **$15-30B**

### Who's Who

| TPA | Revenue | Property Focus | Tech Approach |
|---|---|---|---|
| Sedgwick | ~$5B | Yes (+ WC, auto, liability) | Build internally. No licensing. |
| Crawford | $1.29B | Yes (strong: Contractor Connection, edjuster) | Build + spin out (Turvi). |
| Gallagher Bassett | ~$1.6B | Some | Subsidiary of AJG |
| Davies | ~$1.7B | Yes (via ClaimPilot) | Buy + build. Licenses ClaimPilot. |
| CorVel | $870M | Less (WC-heavy) | Proprietary CareMC Edge + CogencyIQ AI |
| Engle Martin | ~$60-750M | **Commercial property specialist** | Likely buys tech |
| ESIS (Chubb) | Not disclosed | Some | Captive TPA |

### How They Buy

- **Big TPAs (Sedgwick, Crawford, CorVel): Build internally.** Will resist external tools unless ROI is overwhelming.
- **Mid-tier TPAs ($50-500M, ~20-40 of them): Buy.** Use Guidewire, VCA, Five Sigma, or Snapsheet as CMS. More open to point solutions.
- **Sales cycle: 18-30 months** from first contact to scaled deployment (12-18 months sales + 6-9 months implementation)
- **Buyer is a committee:** VP Claims champions, CTO gates, CFO approves
- **Security overhead:** SOC2, CCPA, state insurance regulations required before pilot
- **Per-claim pricing ($50-200/claim)** is preferred over large platform fees — aligns with TPA economics
- **Typical contract: $500K-$2M ACV** for mid-tier TPAs

### The Pain That Creates Budget

1. **Adjuster shortage is CRITICAL.** 50% of insurance workforce retiring in 15 years. 25% of adjusters within 5 years. Claims adjusters = 12th fastest-declining profession by 2030.
2. **Admin burden:** 30-40% of adjuster time on low-value tasks (data entry, rekeying, correspondence). Industry-wide: ~$160B efficiency loss over 5 years (Accenture).
3. **Claims leakage:** 7-14% of total claims spend is preventable overspend. For a TPA handling $1B in claims = $70-140M lost.
4. **Caseload pressure:** Quality benchmark is 100-125 open claims per adjuster. Many carry 150+. Overload = worse decisions = higher leakage.
5. **Turnover:** 20% annual adjuster attrition. Each departure = ~6 years institutional knowledge lost. High-turnover insurers see 12% higher operational costs and 20% higher indemnity payouts.

### The "3x Productivity" Math

**Current state (per property adjuster):**
- Fully loaded cost: ~$110K/year (median $71K salary x 1.5)
- Caseload: ~125 open claims
- Claims closed/year: ~300-480
- Cost per closed claim (labor): $230-$370

**If 3x productive:**
- Same adjuster closes 900-1,440/year
- Cost per claim drops to $75-$125
- Savings: $45K-$120K/year per adjuster

**Scaled to a TPA:**
- Mid-tier (200 property adjusters): saves **$9-24M/year**
- At 20% value capture = **$2-5M/year contract**
- More realistic year-1 (1.3-1.5x improvement): **$600K-$1.6M ACV**

### What TPAs Optimize For (in order)
1. Cycle time (days FNOL to close) — THE top metric
2. Cost per claim (indemnity + ALAE)
3. Claims leakage rate
4. Adjuster caseload / claims per adjuster
5. Customer/carrier satisfaction (NPS)
6. Reserve accuracy
7. Litigation rate
8. Reopen rate

---

## 7. The Confirmed Gap — What Nobody Has Built

**Today, a property adjuster uses 5-6 separate systems per claim:**

```
Xactimate (estimation) + Hover or EagleView (measurements) +
CMS (VCA/Guidewire/JURIS) + n2uitive (recorded statements) +
Encircle or BuildArray (field docs) + carrier portal (reporting)
```

**Nobody has stitched these together into a single property-specific operating system.**

### What's been attempted at integration:
- **Verisk/Xactware** is building an ecosystem around Xactimate (XactAnalysis, XactContents, Hover integration) but it's still estimation-centric
- **Cotality/CoreLogic** has Symbility + Claims Scope + Claims Estimate + aerial data but products aren't tightly integrated
- **Hover** is expanding from exterior to interior to virtual walkthroughs but is still measurement/documentation, not workflow

### What's genuinely unaddressed:
1. **Unified property adjuster workflow** — single pane of glass across estimation, documentation, communication, task management
2. **Automated scope-of-loss creation** from photos/video
3. **Estimate accuracy validation** against regional pricing data
4. **Supplement cycle automation** (the back-and-forth between contractors and carriers on scope changes — one of the biggest time sinks)
5. **Real-time building code compliance** checking against local jurisdictions
6. **Decision ground truth capture** — why did the adjuster decide X? (training data moat)
7. **Cross-system data sync** eliminating the rekeying problem

---

## 8. The Honest Assessment — Where Does Mysa Fit?

### Arguments FOR property claims as Mysa's entry:

1. **No CCC equivalent.** Motor has CCC ($13B+ market cap) locking down the estimating + workflow layer. Property has Xactimate for estimation but **no one owns the workflow layer**. The gap is real.

2. **TPAs are a concrete buyer.** Mid-tier property TPAs (20-40 of them, $50-500M revenue) buy rather than build. They have budget pressure (adjuster shortage, leakage, turnover) and a measurable value prop.

3. **Works in US AND EU.** Unlike motor (where EU conventions create fundamentally different processes), property claims are structurally similar across markets. No EAS equivalent, no convention system. Same process: inspect, document, estimate, pay. Mysa could build one product for both.

4. **The fragmentation is the opportunity.** 5-6 systems per claim = integration pain. A startup that unifies even 2-3 of these (workflow + estimation data + documentation) creates immediate value.

5. **Adjuster shortage creates urgency.** This isn't a nice-to-have — TPAs literally cannot hire enough adjusters. Any tool that makes existing adjusters handle more claims has a forcing function buyer.

6. **Xactimate integration is the wedge.** Every property adjuster uses Xactimate. Build the workflow layer that makes Xactimate data flow better, and you have instant relevance.

### Arguments AGAINST:

1. **18-30 month sales cycles.** A startup needs 2+ years of runway before meaningful revenue. Can Mysa survive that?

2. **Sedgwick, Crawford, and Davies are investing heavily.** They're not standing still. Sidekick Agent, Turvi/CoverAI, and Davies' agentic AI are real products shipping in 2025. By the time Mysa has a product, they'll have 1-2 more years of iteration.

3. **Consolidation risk.** Mid-tier TPAs are getting acquired. Your customer might become a Sedgwick subsidiary mid-contract. (Counter: the acquirer might adopt your tech, or fear of acquisition makes mid-tiers more aggressive on tech.)

4. **Xactimate/Verisk could do this.** They already have the estimation data, the workflow (XactAnalysis), and the Hover partnership. If they decide to build the full adjuster operating system, they start from a position of strength no startup can match.

5. **Assured ($1B valuation) exists.** They're the most-deployed agentic AI in P&C. If they decide to go deep on property, they have the capital and customer base. Same for Five Sigma/Clive.

6. **No proprietary data to start.** The data moat (decision ground truth, claim patterns) only builds once you have customers. Chicken-and-egg.

### The Realistic Path:

**Start narrow, prove value, expand:**

1. **Pick ONE pain point** for property desk adjusters at mid-tier TPAs — the supplement cycle, or document intake + triage, or the Xactimate data sync problem
2. **Integrate with Xactimate** (non-negotiable) and one CMS (VCA or Guidewire)
3. **Sell per-claim** ($50-150/claim) to lower the barrier
4. **Target 3-5 mid-tier property TPAs** for pilot (Engle Martin-sized)
5. **Prove cycle time reduction and leakage prevention** (not headcount reduction — TPAs are short-staffed, they want more output from existing staff)
6. **Capture decision data** from day one — this becomes the moat over time
7. **Expand to more of the workflow** once you have trust and data

**The honest question for the co-founder conversation:** Can you survive 18-30 months to first meaningful revenue, and can you move fast enough that Verisk/Xactimate doesn't build this themselves?

---

## 9. EU Competitive Landscape — Is There an Assured for Europe?

### EU Claims AI Players

| Company | HQ | Funding | What They Do | Traction |
|---|---|---|---|---|
| **omni:us** | Berlin | ~€45M | End-to-end claims AI. 70% auto-settlement rate. | Allianz Austria (processed 2024 storms with zero backlog) |
| **Sprout.ai** | London | ~$38M | Document AI for claims. 98% accuracy. 100+ languages. | AXA, MetLife, Lloyd's Banking Group, AdvanceCare. UK, EU, Americas, Japan. |
| **MarvelX** | Amsterdam | €5.4M | "ClaimOS MaX" — EU-first agentic AI. Claims processing, fraud detection, customer comms. | Founded 2025. Pre-traction. |
| **ClaimSorted** | London | €11.4M | AI-first TPA. 3-10x faster processing. | US, UK, EU |
| **Afori** | Germany | €4M | AI sidebar for insurance brokers. Email/doc → structured tasks. | Founded 2025. Germany-first. |
| **Davies (ClaimPilot)** | UK | ~$1.7B revenue | SaaS CMS + agentic AI agents (casualty-focused). | 81+ organizations on ClaimPilot. |

**None of these are Assured-scale.** Assured has $1B valuation and 50M+ interactions. The EU landscape is seed/Series A with much less traction. omni:us is the most mature (Allianz customer, 70% automation) but is document-processing-focused, not a full workflow OS.

### Does the EU Even Need Its Own Claims AI Platform?

**Yes, for structural reasons US platforms can't easily solve:**

1. **GDPR Article 22** — Generally prohibits fully automated decisions with legal effect. Claims decisions affect finances → legal effect. Any AI that auto-settles claims in EU needs explicit consent, human-in-the-loop safeguards, and right-to-explanation. This is architectural, not a checkbox.

2. **EU AI Act** — Claims AI is classified as **high-risk**. Requires conformity assessment, technical documentation, data governance, human oversight, accuracy testing, transparency. Applies to US companies serving EU customers too.

3. **EU Convention Systems (Motor)** — IRSA, CARD, IDS, CIDE — no US platform has built support because they don't need to. These are EU-specific.

4. **Language + Market Fragmentation** — Each country: different language, different insurance regulations, different convention systems, different distribution models, different document standards, different settlement timing rules. Country-by-country localization, not just translation.

5. **Data Residency** — Many EU insurers require data in-region. US SaaS platforms run on US infrastructure.

### But Is It Venture-Scale?

**Arguments yes:**
- omni:us proves EU insurers will buy (Allianz is a customer)
- GDPR/AI Act create a regulatory moat against US entrants
- EU convention systems are genuinely unaddressed
- MarvelX just raised €5.4M for this exact thesis

**Arguments no:**
- EU market is fragmented — country-by-country GTM
- Each country is relatively small vs. entire US
- Convention systems are country-specific (Portugal ≠ France ≠ Italy)
- Sprout.ai and omni:us have been at this for years and are still relatively small
- MarvelX is literally building this right now from Amsterdam

Sources:
- [Debevoise — EU AI in Insurance](https://www.debevoisedatablog.com/2025/05/21/europes-regulatory-approach-to-ai-in-the-insurance-industry/)
- [Blue Arrow — AI Act and Insurance](https://bluearrow.ai/ai-act-and-insurance/)
- [EIOPA AI Governance Opinion](https://www.eiopa.europa.eu/eiopa-publishes-opinion-ai-governance-and-risk-management-2025-08-06_en)
- [MarvelX Raise](https://www.eu-startups.com/2025/05/insurance-services-are-at-a-pivotal-moment-amsterdam-based-marvelx-raises-e5-4-million-for-ai-platform/)
- [omni:us](https://omnius.com/)
- [ClaimSorted Raise](https://www.vestbee.com/insights/articles/claim-sorted-raises-11-4-m)

---

## 10. EU Adjusters Work COMPLETELY Differently From US

### Motor Claims — The Adjuster Is Barely Involved

In the EU, most motor claims **never see an external loss adjuster**. Here's how it actually works:

```
ACCIDENT → EAS filled out → Submitted to OWN insurer → Internal claims handler processes it
                                                              |
                                            ┌─────────────────┼──────────────────┐
                                            ▼                 ▼                  ▼
                                    Convention match?    Unclear EAS?       Complex/BI?
                                            |                 |                  |
                                    Auto-resolve (STP)   Handler calls     External loss
                                    No adjuster needed    for clarification  adjuster assigned
                                            |                 |                  |
                                    ~10% actual STP     ~60% of claims    ~20-30% of claims
                                    (should be 60-70%)   human handler      get an adjuster
```

**Key insight:** The EU "adjuster" for motor is really a **perito/expert** — a damage inspector who goes to the repair shop to validate the repair cost. They are NOT making liability decisions (the convention does that) or investigating what happened (the EAS captures that). Their job is narrow: "does this repair estimate match the actual damage?"

**Audatex/Solera** (not Xactimate) dominates EU motor damage estimation. Qapter does photo-based AI estimation. This part of the workflow is already well-served.

### Property/Home Claims — Adjusters ARE Involved But Structured Differently

EU property claims DO need loss adjusters, similar to US. But the structure differs:

| | **US** | **EU** |
|---|---|---|
| **Who employs adjusters** | Staff adjusters, TPAs (Sedgwick, Crawford), independent adjusters | Mostly **independent loss adjusters** commissioned per-claim by insurer |
| **TPA market** | Massive ($115B). Carriers outsource to TPAs. | **Minimal.** Carriers handle claims internally. Loss adjusting firms are commissioned per-claim. |
| **Estimation tools** | Xactimate (75-80% market share) | **No single standard.** Cotality/CoreLogic in UK. Country-specific tools elsewhere. |
| **Field vs desk** | Clear desk/field split (40/60 trending to 60/40) | Trending to virtual/remote. Spain already offers video assessment links. |
| **Who buys adjuster tools** | TPAs and carriers | **Carriers directly** and **loss adjusting firms** (Crawford EU, McLarens, Sedgwick Europe, Charles Taylor) |
| **Major loss adjusting firms** | Crawford, Sedgwick, Engle Martin | Crawford (70+ countries), McLarens (230+ offices, 45 countries), Sedgwick Europe (via Cunningham Lindsey acquisition), Charles Taylor |

### The TPA Gap — Why the US Playbook Doesn't Work in EU

**This is the killer finding for Mysa's strategy.**

In the US, the TPA market is $115B. Mid-tier TPAs buy software. They're the natural customer for an "adjuster operating system."

In the EU, **there is no equivalent TPA market for property claims.** European carriers handle claims internally with their own claims handlers. External loss adjusters are brought in per-claim for complex cases, not as standing outsourced relationships. The "sell to mid-tier TPAs" strategy that works in the US has no EU equivalent.

**Who would buy adjuster tools in EU?**
1. **Carriers directly** — but they have long procurement cycles (24-36 months), conservative IT departments, and usually build internally
2. **Loss adjusting firms** — Crawford EU, McLarens, Sedgwick Europe — but these are the same big firms that are building their own tools (Turvi, Sidekick, etc.)
3. **Independent loss adjusters** — fragmented, small, low technology budget

---

## 11. The STP Reality Gap — Deep Dive

This is the single most important finding from all the Mysa research. Here's why.

### What the Convention Systems Promise

EU convention systems are **pre-built decision engines** that have operated for decades:

| Country | Convention | Coverage | Fault Logic | Speed |
|---|---|---|---|---|
| **France** | IRSA | ~80% of material motor claims | 13 cases, outputs 0/50/100% only | Deterministic |
| **Italy** | CARD | Mandatory for 2-vehicle claims, <9% permanent disability | Civil code principles + CAI form | Days |
| **Spain** | CIDE/ASCIDE/CICOS | 70-83% of all motor claims | Tabla de Culpabilidad + CICOS platform | 2.5M claims/year processed |
| **Portugal** | IDS | ~100% market participation | Direct compensation protocol | **1.94 days** avg decision, **91% agreement** |

The convention lookup itself is trivial — it's a database query:

```
INPUT: EAS checkbox data (17 circumstances per vehicle) + impact points + road layout
LOOKUP: Match to convention case (e.g., IRSA Case 10 = rear-end = 100% rear vehicle)
OUTPUT: Fault percentage (0%, 50%, or 100% in France)
```

**In theory, 60-70% of motor claims could be resolved straight-through** (no human intervention) because they match a convention case cleanly.

### What Actually Happens

**Only ~10% of claims actually achieve STP.** The 50+ point gap between theoretical and actual is the single biggest inefficiency in EU motor claims.

### Why the Gap Exists — The 5 Bottlenecks

**1. Paper EAS forms (~50% of all EAS)**
The European Accident Statement is a brilliant concept — a standardized carbon-copy form signed by both parties at the scene. But ~50% are still filled out on paper by stressed people with shaking hands:
- Illegible handwriting
- Unclear checkbox ticks (is box 8 checked or just smudged?)
- Ambiguous diagrams (freehand sketches of the accident)
- Missing fields (people skip sections in the chaos)
- Wet, damaged, crumpled paper

**2. Poor diagram quality**
The sketch/diagram section is the hardest to interpret. Two stressed people draw the road, their vehicles, and the movement. The result is often:
- Stick figures and blobs instead of clear vehicle positions
- No indication of direction of travel
- Missing road markings, signs, or lane information
- Contradictory with the checkboxes (the sketch shows one thing, the boxes say another)

**3. Contradictory checkbox data**
Both drivers fill out their side independently. Often:
- Both drivers check boxes that imply the other was at fault
- One driver checks boxes that contradict their own diagram
- Boxes are checked inconsistently (e.g., "turning left" checked but diagram shows straight road)

**4. Missing context for edge cases**
Even when the form is cleanly filled out, ~30-40% of cases don't fit neatly into one of the convention's predefined scenarios:
- The accident happened on a roundabout with unusual geometry
- Three vehicles were involved but one left (partial hit-and-run)
- The diagram shows a scenario between two convention cases
- Weather or road conditions were relevant but the convention ignores them

**5. Data entry / digitization gap**
Even when the paper EAS arrives at the insurer, someone has to:
- Physically receive the paper form
- Read and interpret it
- Key the data into the claims management system
- Make a judgment call on ambiguous fields
- Route it to the right handler

This manual intake process adds days and introduces transcription errors.

### The Math: Where the 50 Points Go

```
100% of motor claims

  → ~20% fall outside convention scope entirely (3+ vehicles, BI, foreign plates, etc.)

  → 80% are convention-eligible

     → of those 80%, ~50% have clean, unambiguous EAS data
        → of those, ~60-70% map to a convention case cleanly
           → THIS IS THE ~25-28% that COULD be fully STP today
           → But only ~10% actually achieve it (insurer systems, internal routing, QA checks)

     → ~50% have messy, ambiguous, or paper-only EAS data
        → These require human intervention to interpret
        → Claims handler calls driver, asks for clarification
        → Handler makes judgment call on checkboxes/diagram
        → Maybe sends perito for vehicle inspection
        → Takes days to weeks instead of minutes
```

### What "Fixing" the Gap Actually Means

**Layer 1: Digitize the EAS (partially solved)**
- France has **e-constat auto** — official app that digitizes the EAS, pre-fills policyholder data, includes geolocation
- But adoption is still ~50% — the other half is paper
- Other countries have similar apps but adoption varies

**Layer 2: Improve data quality at the point of capture (NOT solved)**
This is the real opportunity:
- **Guided photo capture** — AI-guided photos of the accident scene that supplement the sketch
- **Structured diagram creation** — instead of freehand, drag-and-drop vehicle positions on a map
- **Checkbox validation** — real-time logic that flags contradictions ("you checked 'turning left' but your diagram shows a straight road")
- **Automatic field completion** — pull vehicle data from registration, pull policy data from insurer, pre-fill weather from API
- **OCR for paper forms** — when paper EAS arrives, extract and structure the data with high accuracy

**Layer 3: Convention matching engine (technically trivial, politically hard)**
- The actual lookup is simple code — match checkboxes to convention cases
- The challenge is **accessing the convention rules** (proprietary to national insurer associations)
- And handling the **30-40% that don't match cleanly** — this is where AI judgment matters

**Layer 4: Insurer system integration (the hard part)**
- Even if you have perfect structured data and a matching engine, you need to push the result into the insurer's claims management system
- Each insurer has different systems (Guidewire, Sapiens, proprietary, mainframe)
- Integration is a 6-12 month project per insurer

### Who Benefits From Closing the Gap

| Stakeholder | Current Pain | Value of STP |
|---|---|---|
| **Claims handler** | Spends 30% of time on data extraction + reconciliation | Frees up capacity for complex claims |
| **Policyholder** | Waits days-weeks for simple claim resolution | Gets resolved in hours |
| **Insurer** | Pays claims handler salary for routine work | Reduces cost per claim by 40-60% for STP-eligible |
| **Convention system** | 91% agreement rate (Portugal) but slow | Faster resolution = lower leakage |

### What It Would Take to Build

**Phase 1: Better EAS capture (the wedge)**
- Mobile app for policyholders at the accident scene
- AI-guided photo capture (damage, scene, road layout)
- Structured diagram builder (not freehand)
- Real-time checkbox validation
- Auto-fill from vehicle registration + policy data
- **This is the product that improves data quality upstream**

**Phase 2: Convention matching + insurer push**
- Structured EAS data → convention lookup engine
- Covers IRSA (France), CARD (Italy), CIDE (Spain), IDS (Portugal)
- API integration to push results into insurer CMS
- Dashboard showing match rate, STP rate, exception cases

**Phase 3: Exception handling AI**
- The 30-40% that don't match cleanly
- AI interprets ambiguous diagrams, contradictory checkboxes
- Suggests most likely convention case with confidence score
- Human-in-the-loop for low-confidence cases

### The Honest Assessment of This Opportunity

**What's genuinely attractive:**
- The problem is real and quantified (50+ point STP gap)
- The convention systems are unique to EU — no US competitor has this
- The value is measurable (cost per claim reduction, cycle time, handler capacity)
- Portugal's IDS (1.94-day decisions, 91% agreement) proves the model works when data is clean
- France's e-constat shows digital EAS capture is possible — but adoption is only ~50%

**What's genuinely hard:**
- **Country-by-country.** Each convention has different rules, different thresholds, different fault logic. You can't build one engine for all of EU — you build per-country.
- **Convention rules are proprietary.** GCA (France), ANIA/CONSAP (Italy), UNESPA/TIREA (Spain), APS (Portugal) own the rules. You need their cooperation or at least their tolerance.
- **The buyer is the carrier.** Not a TPA, not an adjuster — the insurer's claims department. Long sales cycles, conservative buyers.
- **e-constat exists.** France already has an official digital EAS app. You're competing with or complementing a government-backed standard.
- **Small market per country.** Portugal has ~210K IDS claims/year. France is bigger but still a fraction of the US motor market.
- **The conventions themselves are updating.** IRSA forfait amounts change, eligibility thresholds change, the Netherlands is still building its DSA. You're building on a moving foundation.
- **MarvelX and omni:us are here.** They're not specifically targeting the STP gap, but they're in the EU claims AI space.

**The co-founder question:** Is a 50-point STP improvement for EU motor claims — sold country-by-country to carriers — a venture-scale business? Or is it a valuable feature that someone like omni:us or MarvelX will bolt on?

Sources:
- [Full EU Convention Systems Research](./EU_Convention_Systems_Deep_Research.md)
- [FUEDI — European Federation of Loss Adjusting Experts](https://fuedi.eu/)
- [Insurance Business Review Europe — Strategic Reinvention of Claims](https://www.insurancebusinessrevieweurope.com/news/the-strategic-reinvention-of-claims-loss-adjustment-in-european-insurance-nwid-1057.html)
- [C1 Brokers — Claims in Portugal](https://c1brokers.pt/en/claims-in-portugal/)
- [Sedgwick Europe](https://www.sedgwick.com/europe/)
- [McLarens Europe](https://www.mclarens.com/region/europe/)
- [Cotality Claims Estimate UK](https://www.cotality.com/uk/products/claims-estimate)

---

## 12. EU SME Insurer Market — Document Intake, Parsing & Agent Management

### The Caravela Benchmark

**Caravela Seguros:** €187.7M GWP (2024), grew 17% YoY. In 2023, Caravela was one of the top market share gainers in Portuguese non-life alongside Ageas and Mapfre. Toscafund (PE owner) was weighing a sale in 2025. **This is a mid-market insurer, not a small one.**

Key Caravela facts:
- €187.7M GWP = roughly 40,000-60,000 non-life policies, ~10,000-20,000 motor claims/year
- Bought Mysa's OCR product in **~3 months** — not 18-30 months
- On legacy/custom systems, not Guidewire or Sapiens (those start at €500K+/year)
- Has peritos, repair shops, brokers/agents as third parties to coordinate

**This is the template customer.** Not AXA, not Allianz. A €100-300M GWP insurer in Southern/Central EU, growing, on legacy tech, with a CTO who can make decisions without a 12-person committee.

### How Many Insurers Are We Talking About?

**EIOPA data (April 2025):** 2,153 solo insurance undertakings + 93 insurance groups across EU/EEA.

Breaking it down by size (estimated from EIOPA structure + Solvency II proportionality data):

| Segment | GWP Range | Count (est.) | Claims/yr per co. | Can they buy? |
|---|---|---|---|---|
| **Micro** | <€25M | ~800-1,000 | 1,000-5,000 | ❌ Too small. Can't justify €30K+ software. Many are niche/specialty. |
| **Small** | €25-100M | ~400-500 | 5,000-20,000 | ⚠️ Possible. Budget-constrained but feeling the pain. €30-80K deals. |
| **Mid-market (Caravela-sized)** | €100-500M | ~200-300 | 15,000-80,000 | ✅ **Sweet spot.** Have budget, acute pain, can decide fast. €80-200K deals. |
| **Upper mid** | €500M-2B | ~100-150 | 80,000-300,000 | ✅ Bigger deals (€200-500K) but more procurement friction. |
| **Large groups** | €2B+ | ~50-80 | 300,000+ | ❌ Build their own (Allianz, AXA, Generali). Or buy enterprise (Guidewire). |
| **Total solo undertakings** | | **2,153** | | |

### The Full Market Aggregate — People, Premium, Claims

EU insurance industry: ~920,000 total employees (2023, Insurance Europe). Non-life = ~50-55% = ~460,000-500,000. Here's what each segment looks like **in total across all companies in that band:**

| Segment | Companies | Avg Employees | **Total Employees** | **Claims Staff** | **Total GWP** | **Total Claims/yr** |
|---|---|---|---|---|---|---|
| **Micro** (<€25M) | ~900 | ~100 | ~90,000 | ~13,500 | ~€11B | ~2.7M |
| **Small** (€25-100M) | ~450 | ~300 | ~135,000 | ~22,500 | ~€25B | ~5.4M |
| **Mid-market** (€100-500M) | ~250 | ~600 | ~150,000 | ~30,000 | ~€62B | ~10M |
| **Upper mid** (€500M-2B) | ~125 | ~2,500 | ~312,000 | ~62,500 | ~€125B | ~18.8M |
| **Large groups** (€2B+) | ~65 | ~4,000+ | ~260,000+ | ~52,000+ | ~€260B | ~20M+ |
| **TOTAL** | **~1,790** | | **~947,000** | **~180,000+** | **~€483B** | **~57M** |

*Sanity checks: Total employees (~947K) vs. Insurance Europe figure (~920K) ✅. Total non-life GWP (~€483B) vs. Insurance Europe figure (~€480-520B est. 2024) ✅.*

**The addressable market (€25M-2B GWP, the ones who'd actually buy):**

| | Companies | Total Employees | **Claims Staff** | Total GWP | Total Claims/yr |
|---|---|---|---|---|---|
| **Small + Mid + Upper** | **~825** | **~597,000** | **~115,000** | **~€212B** | **~34M claims** |

**The primary sweet spot (€100-500M, "Caravela segment"):**

| | Companies | Total Employees | **Claims Staff** | Total GWP | Total Claims/yr |
|---|---|---|---|---|---|
| **Mid-market alone** | **~250** | **~150,000** | **~30,000** | **~€62B** | **~10M claims** |

**What this means in plain terms:**
- There are ~250 Caravela-sized insurers across the EU, employing ~150,000 people, of which ~30,000 are claims staff processing ~10 million claims per year
- Expanding to include small (€25-100M) and upper-mid (€500M-2B), it's ~825 companies, ~115,000 claims staff, ~34 million claims per year
- **115,000 claims professionals across 825 companies** = the total population you're selling to and building tools for
- At per-seat pricing: 115,000 × €500-1,500/seat = €57-172M (another way to sanity-check the TAM)

**Non-life focused (motor, property, liability) = ~60-65% of total = ~1,300-1,400 undertakings.**

**Realistic addressable (€25M-2B GWP, non-life):** ~500-700 insurers.

**Primary target (€100M-500M, "Caravela segment"):** ~200-300 insurers.

### Country Breakdown

| Country | Non-life insurers (approx) | "Caravela segment" (€100-500M) | Key context |
|---|---|---|---|
| **Portugal** | 53 licensed (25 foreign branches) | ~8-12 domestic | Caravela here. IDS convention. Small market but fast-moving. |
| **Spain** | ~200+ total, 28 private mutuals | ~40-60 | CIDE/ASCIDE/CICOS. Regional mutuals + mid-size national players. Huge. |
| **Italy** | ~200+ total | ~40-60 | CARD mandatory. Highest claims frequency (~7%). Very fragmented. |
| **France** | ~300+ total | ~50-70 | IRSA. Largest motor market. Many mutual/cooperative insurers (MAIF, MACIF, etc). |
| **Germany** | ~400+ total | ~50-70 | Largest EU market. Sparkassen-linked insurers, regional mutuals. |
| **Benelux** | ~150+ total | ~20-30 | Broker-dominated. Moderate tech maturity. |
| **Nordics** | ~100+ total | ~15-20 | High digital maturity — may not need help, or may be early adopters. |
| **CEE** | ~300+ total | ~30-50 | Growing, lower tech adoption, tight budgets but hungry for modernization. |
| **Total** | ~1,700+ | **~250-370** | |

### How Small Are the Small Ones?

The floor of viability matters. Here's what the bottom of the market looks like:

**€25-50M GWP insurer (~400 across EU):**
- Maybe 5,000-10,000 claims/year
- Staff: 50-200 employees total, 10-30 in claims
- IT: 2-5 people, often outsourced
- Tech stack: Custom legacy system built 10-20 years ago, or spreadsheets + email + paper
- Budget for claims tech: €20-50K/year — **tight but real if you solve acute pain**
- Sales cycle: 1-3 months (CTO + CEO decide, no procurement committee)
- Example: a niche motor insurer in Romania, a small mutual in southern Spain

**€50-100M GWP insurer (~200 across EU):**
- 10,000-20,000 claims/year
- Staff: 200-500, 30-80 in claims
- IT: 5-15 people
- Tech stack: Older vendor CMS (maybe Sapiens lite, or local vendor like Novabase in PT), customized over years
- Budget: €50-100K/year for claims tech
- Sales cycle: 2-4 months
- Example: a regional property insurer in Italy, a transport insurer in Belgium

**€100-300M GWP insurer (Caravela-sized, ~150-200 across EU):**
- 15,000-50,000 claims/year
- Staff: 300-1,000, 50-200 in claims
- IT: 10-30 people, maybe a CTO
- Tech stack: Mix of older vendor + custom modules + manual processes
- Budget: €100-250K/year for claims tech
- Sales cycle: **2-4 months** (Caravela = 3 months, real data point)
- Example: Caravela (PT), medium mutual in France, regional insurer in Germany

### Who's Actually Selling to Them Today?

**Almost nobody is specifically targeting the €25-500M EU insurer for claims AI.** Here's why:

| Competitor | Who they sell to | Selling to "Caravela segment"? |
|---|---|---|
| **omni:us** (Berlin, ~€45M) | ~30 pilots — Allianz Austria, UNIQA | **No.** Targeting big carriers. |
| **Sprout.ai** (London, $38M) | AXA, MetLife, Lloyd's Banking Group, Scottish Widows | **No.** Enterprise play. |
| **MarvelX** (Amsterdam, €5.4M) | 1 customer (Companjon, embedded insurance) | **No.** Just launched. Pre-traction. |
| **ClaimSorted** (London, €11.4M) | 20+ insurers US/UK/EU — but as a TPA | **Not as software.** They're a TPA. |
| **FurtherAI** (NYC, $25M from a16z) | ~100 US partners. Accelerant, MSI, Leavitt. $15B premiums. | **No.** US-only. Zero EU. |
| **Assured** ($1B valuation) | 50M+ interactions, US auto carriers | **No.** US auto only. |
| **Guidewire** | ~450 insurers globally, Tier 1 | **No.** Too expensive (€500K+/year). |
| **Sapiens** | Mid-large carriers | **Rarely.** Starts at €500K/year. |

**The gap is real.** Every AI claims startup goes after big carriers first because the deals are 5-10x larger. But that leaves the 500-700 mid-market EU insurers underserved. They're stuck on legacy systems, processing claims with paper/email/spreadsheets, and the big vendors are too expensive for them.

### What Would They Buy? (The Multi-Product Opportunity)

This is the key insight: **these insurers don't just need one tool — they need 5-6 products.** And they'll buy them from whoever gets in the door first.

**Product 1: Document Intake & OCR (Land)** — €20-40K/year
- EAS forms, police reports, damage photos, repair estimates arrive as PDFs, photos, faxes, emails
- Digitize and structure everything automatically
- **This is the easiest sell — immediate ROI, low risk, fast deployment**
- Caravela bought this first

**Product 2: Claims Parsing & Field Extraction** — €30-50K/year
- Map extracted data to their CMS fields
- Validate completeness, flag missing data
- Auto-populate claims records

**Product 3: Convention Matching & Auto-Triage** — €30-50K/year
- Map EAS checkboxes to IRSA/CARD/IDS/CIDE fault tables
- Auto-triage: STP-eligible vs needs handler vs needs investigation
- **This is where the STP gap value lives**

**Product 4: Third-Party Management** — €40-80K/year
- Coordinate with repair shops, peritos (inspectors), rental agencies, medical providers
- Track assignments, deadlines, costs
- Structure the work of brokers/agents submitting claims
- **This is a workflow product, not an AI product — and it's sticky**

**Product 5: Broker/Agent Portal** — €30-60K/year
- Let distribution network submit claims digitally
- Structured intake instead of email/phone/portal rekeying
- Real-time status visibility for brokers

**Product 6: Analytics & Reporting** — €20-40K/year
- Claims dashboards, STP rates, handler productivity
- Regulatory reporting (Solvency II, ASF, IVASS)
- Convention system performance monitoring

### The Land-and-Expand Math

**This changes the TAM calculation fundamentally.**

| | Year 1 (Land: Product 1) | Year 2 (Add Products 2-3) | Year 3+ (Full Platform: Products 1-6) |
|---|---|---|---|
| ACV per customer | €30-50K | €80-120K | €150-300K |
| Addressable customers | 500-700 | 500-700 | 500-700 |
| **TAM** | **€15-35M** | **€40-84M** | **€75-210M** |

**Weighted average (assuming 30% at land, 40% at mid-expand, 30% at full platform):**

| | Conservative | Moderate | Optimistic |
|---|---|---|---|
| Customers | 400 | 600 | 800 |
| Weighted ACV | €100K | €150K | €200K |
| **TAM** | **€40M** | **€90M** | **€160M** |

**Net Revenue Retention math (the magic of land-and-expand):**
- Land at €35K → expand to €150K over 3 years = **~130% NRR**
- Cost to upsell existing customer: ~24% of cost to acquire new customer (industry data)
- Means every €1 in acquisition investment generates €4+ in lifetime value

**Cross-check with top-down:**
- EU claims management software market: €4.3B (2024) → €6.1B (2030)
- SME segment (~30%): ~€1.3B
- Claims workflow layer (intake + parsing + triage + third-party mgmt): ~10-15% of claims management: **€130-195M**
- ✅ Consistent with bottom-up moderate-optimistic

### The Sales Velocity Advantage

**The 18-30 month sales cycle assumption was wrong for this segment.** That's the Allianz/AXA cycle. The Caravela cycle is different:

| | Big Carrier (AXA, Allianz) | Mid-Market (Caravela-sized) | Small (€25-100M) |
|---|---|---|---|
| Decision makers | 12-person committee, VP Claims + CTO + CFO + Procurement + Legal + Compliance | CTO + CEO (maybe CFO) | CTO or IT Manager alone |
| Sales cycle | 18-30 months | **2-4 months** | **1-3 months** |
| Proof of concept required? | Yes, 3-6 months | Maybe, 2-4 weeks | Quick demo + trial |
| Deal size | €500K-2M | €30-150K | €20-80K |
| Procurement process | Formal RFP | Informal evaluation | "Show me it works" |
| Implementation time | 6-12 months | 2-4 months | 2-6 weeks |
| Existing vendor lock-in | Guidewire/Sapiens (hard to displace) | Legacy/custom (easier to integrate alongside) | Spreadsheets/email (anything is better) |

**At 2-4 month cycles, a 2-person sales team could close 15-25 deals/year.** Compare that to enterprise where 1 AE closes 3-5 deals/year.

### The Honest Revised Assessment

**€90-160M TAM with 130% NRR and 2-4 month sales cycles is a meaningfully different business than what I initially described.**

It's still not a $1B TAM. But:

1. **The unit economics work for bootstrapping:** €35K landing deals, 2-4 month cycles, expand to €150K. You can get to €2-3M ARR with a small team before needing outside capital.

2. **NRR makes the growth math work:** With 130%+ NRR, you can grow 40-50%/year even with moderate new customer acquisition. That's B2B SaaS math that works.

3. **The competitive landscape is genuinely empty for this segment.** Every AI startup is chasing AXA and Allianz. Nobody is building for the 500-700 mid-market EU insurers.

4. **Multi-product is the moat.** Once you're doing intake + parsing + convention matching + third-party management, switching costs are enormous. You're embedded in their daily workflow.

5. **The path to venture-scale is the platform expansion.** Start with claims intake/workflow for motor → expand to property → expand to the STP gap (convention matching) → become the "claims operating system for mid-market EU insurers."

**This could be a €20-40M ARR business at maturity, sold for 8-15x revenue = €160-600M exit.** Or, with the right platform expansion, a venture-scale outcome.

**The risk isn't competition — it's execution.** Can you build 6 products fast enough, in enough languages, integrated with enough legacy systems, across enough convention systems, to capture the market before someone else notices it's there?

---

## 13. Venture-Scale Math — STP Gap vs. Property Adjuster OS

### The STP Gap Opportunity (Motor, EU-Only)

**What is it:** Fix the 50+ point gap between theoretical STP (60-70%) and actual STP (~10%) in EU motor claims by fixing upstream data quality.

**The math:**

| Metric | Value | Source |
|---|---|---|
| EU registered vehicles | ~334 million | Insurance Europe |
| Motor claims frequency | ~4-6% average (varies: Finland 2.4%, Portugal 7.3%) | EIOPA, Insurance Europe |
| **Total EU motor claims/year** | **~15-20 million** | Derived (334M × 5%) |
| Convention-eligible claims (material damage, cooperative, matching scenario) | ~60-70% = **10-14 million** | Convention system design |
| Currently STP'd | ~10% = **1-1.5 million** | Industry estimates (validated in our research) |
| **The gap: could be STP'd but aren't** | **~9-12 million claims/year** | Derived |
| Average EU motor claim cost | ~€5,000-6,000 | Italy avg: €5,000, cross-EU estimate |
| Processing cost per claim (adjuster/handler time) | ~€200-500 | Industry estimate |
| **Annual waste from the STP gap** | **€1.8-6B** | 9-12M × €200-500 |

**So what's the TAM for the software that fixes it?**

Not €6B — that's the waste, not the willingness to pay. The TAM is:

**Model A: Per-claim pricing**
| | Conservative | Moderate | Optimistic |
|---|---|---|---|
| Claims improved per year | 3M | 6M | 10M |
| Price per claim | €5 | €10 | €15 |
| **Revenue** | **€15M** | **€60M** | **€150M** |

**Model B: Per-insurer SaaS**
| | Conservative | Moderate | Optimistic |
|---|---|---|---|
| Addressable insurers | 300 | 500 | 800 |
| Average ACV | €80K | €150K | €250K |
| **Revenue** | **€24M** | **€75M** | **€200M** |

**Realistic TAM: €60-150M** (moderate scenarios)

**Defensibility:** ✅✅✅ — Genuinely EU-specific
- No US competitor can touch this (no convention systems in US)
- Requires deep knowledge of IRSA, CARD, IDS, CIDE/ASCIDE/CICOS — each country is different
- Need to handle EAS in 24+ languages
- GDPR Article 22 + EU AI Act compliance = barrier to US players entering
- **Decision ground truth capture** (why the adjuster/handler decided what they decided) creates a data moat over time

**Weaknesses:**
- €60-150M TAM is borderline venture-scale. Depends heavily on pricing power.
- The STP gap is caused by **data quality** not software gaps — you're selling a data quality fix, which is harder to demonstrate ROI on than "here's a tool"
- Incumbents could fix this themselves (Allianz already building Insurance Copilot, omni:us already doing 70% auto-settlement for Allianz Austria)
- Individual country integration is expensive — each convention system has different rules, different insurer APIs, different regulators
- Sales cycle is still 12-24 months for insurers

**Verdict: Defensible but tight on TAM. Needs aggressive pricing (per-claim at €10+) or platform expansion to be venture-scale.**

---

### The Property Adjuster OS Opportunity (US-First, Expand to EU)

**What is it:** Build the unified operating system for property adjusters — replacing the 5-6 point solutions they use today with one platform.

**The math:**

| Metric | Value | Source |
|---|---|---|
| US property claims/year | ~35-40 million | Industry reports |
| US adjusters (all types) | ~200,000-250,000 | BLS, industry estimates |
| TPA adjusters (Sedgwick, Crawford, etc.) | ~60,000-85,000 | 25-35% of total |
| Average property claim | ~$15,000 | III data |
| Claims processing cost (adj. time + tools) | ~$500-1,500 per claim | McKinsey estimates |
| **Total US property claims processing spend** | **$17-60B** | 35M × $500-1,500 |
| EU property claims/year | ~15-20 million | Estimated from EU non-life data |
| EU property adjusters | ~80,000-120,000 | Estimated (less TPA structure) |

**TAM calculation:**

**Model A: Per-adjuster seat**
| | Conservative | Moderate | Optimistic |
|---|---|---|---|
| Addressable adjusters (US) | 50,000 | 100,000 | 200,000 |
| Price per seat/year | $3,000 | $5,000 | $8,000 |
| **US Revenue** | **$150M** | **$500M** | **$1.6B** |
| Add EU (40% of US) | $60M | $200M | $640M |
| **Total** | **$210M** | **$700M** | **$2.2B** |

**Model B: Per-claim pricing**
| | Conservative | Moderate | Optimistic |
|---|---|---|---|
| Claims processed (US) | 5M | 15M | 30M |
| Price per claim | $10 | $20 | $30 |
| **US Revenue** | **$50M** | **$300M** | **$900M** |

**Realistic TAM: $300M-700M** (clearly venture-scale)

**Defensibility:** ⚠️ — Venture-scale but crowded
- Verisk owns Xactimate (75-80% market share in estimation) and acquired Hover. They could build this.
- Assured ($1B valuation) is coming from the auto side but could expand to property
- Sedgwick, Crawford, Davies are building their own tools (but don't license them — only sell as part of TPA service)
- CoreLogic/Cotality has property data + claims products
- Microsoft Copilot for Insurance (via Avanade) is platform play

**Weaknesses:**
- 18-30 month enterprise sales cycles
- Adjusters resist change (documented: "tools that adjusters don't adopt are worthless")
- Integration with Xactimate is essential — Verisk could block or disadvantage competitors
- No EU equivalent of the TPA buyer market — in EU, insurers handle claims internally, independent adjusters are per-claim contractors, not TPA employees
- Hidden damage problem limits AI automation to augmentation, not replacement

**Verdict: Clearly venture-scale TAM. But faces convergence from Verisk, Assured, and big TPAs. The "who wins?" question is about distribution and switching costs, not about whether the market exists.**

---

### Head-to-Head Comparison

| | STP Gap (Motor, EU) | Property Adjuster OS (US+EU) |
|---|---|---|
| **TAM** | €60-150M | $300M-700M |
| **Venture-scale?** | Borderline (need platform expansion) | Yes, clearly |
| **Defensibility** | ✅✅✅ Very high (EU-specific, convention expertise) | ⚠️ Medium (convergence risk) |
| **Competition** | omni:us, MarvelX, Sprout.ai (all sub-€50M raised) | Verisk, Assured ($1B), Sedgwick, Crawford |
| **Sales cycle** | 12-24 months (EU insurers) | 18-30 months (TPAs, carriers) |
| **Geographic** | EU-only (by design) | US-first, EU expansion possible but different |
| **Data moat** | Decision ground truth + convention mapping | Adjuster workflow data + estimation patterns |
| **Time to revenue** | Faster (smaller deals, SME insurers) | Slower (larger deals, enterprise) |
| **Exit scenarios** | Acquired by CCC, Guidewire, or EU insurer (€100-300M) | IPO or strategic acquisition ($500M-2B) |
| **Biggest risk** | Insurers fix it themselves (Allianz model) | Verisk builds it from Xactimate + Hover |

### The Real Strategic Question

**These aren't mutually exclusive — they're sequenceable.**

**Path 1: STP Gap First (Wedge → Platform)**
1. Build the EU motor claims data quality layer (EAS digitization + convention matching)
2. Win 50-100 SME insurers in 2-3 countries (Portugal, Spain, Italy)
3. Expand into triage, settlement, subrogation automation
4. Use distribution + data moat to expand to property
5. **Year 1-3: €2-8M ARR (bootstrappable). Year 3-6: Raise Series A for platform expansion.**

**Path 2: Property Adjuster OS First (Venture)**
1. Raise $5-10M seed for US property adjuster OS
2. Win 5-10 TPA customers in year 1-2
3. Race against Verisk/Assured convergence
4. Expand to EU (but EU property market is structurally different — no TPAs)
5. **Year 1-2: $0-2M ARR (burning cash). Year 2-4: $5-15M ARR if it works.**

**Path 3: Document Intake Wedge (Bootstrap)**
1. Build Caravela-style document intake/parsing for EU SME insurers
2. Win 20-50 customers in Southern EU (Portugal, Spain, Italy)
3. Expand to convention matching, then full workflow
4. Stay bootstrapped or raise small round for acceleration
5. **Year 1-2: €500K-2M ARR. Year 3-5: €5-10M ARR. Lifestyle or PE exit.**

**The co-founder conversation is really about Path 1 vs Path 2 vs Path 3 vs Path 4.** Path 1 is the most defensible. Path 3 is the safest bootstrap. And Path 4 (below) is the wildcard — a completely different business model that attacks the supply crisis directly.

---

## 14. The Adjuster Workforce Platform — US Only

### Why This Section Is US-Only

We established in Section 10 that EU adjusters work completely differently:
- EU motor claims rarely need external adjusters (internal handlers + conventions do the work)
- EU "peritos" are narrow damage inspectors at repair shops, not full adjusters making coverage/liability decisions
- No TPA market in EU like US ($115B US TPA market has no EU equivalent)
- EU property uses independent loss adjusters commissioned per-claim, not TPA employees

**An adjuster marketplace/training platform makes sense for the US, not the EU.** The US has 200,000-250,000 adjusters, massive shortage, 20% attrition, and TPAs that desperately need staffing. The EU doesn't have this structure.

### The US Adjuster Supply Crisis

| Metric | Data | Source |
|---|---|---|
| Total US adjusters | ~200,000-250,000 | BLS |
| Claims adjusters job ranking | **12th fastest-declining profession by 2030** | WEF Future of Jobs 2025 |
| Insurance workforce retiring | **50% within 15 years** | Industry estimates |
| Adjusters retiring | **25% within 5 years** | Industry estimates |
| Annual attrition | **20%** | Industry data |
| Institutional knowledge lost per departure | ~6 years | Industry estimates |
| Impact of high turnover | 12% higher operational costs, 20% higher indemnity payouts | Accenture/industry research |

**Alacrity Solutions** (one of the largest independent adjusting firms) went into restructuring in late 2024 and private credit lenders took control by January 2025. The old staffing model is literally breaking.

### What Exists Today

| Platform | Model | Gap |
|---|---|---|
| **WeGoLook** (Crawford) | 45,000 gig "Lookers" for low-complexity on-demand inspections. Acquired for $36M. | **Not adjusters.** Lookers take photos and fill checklists. No coverage decisions, no estimates, no investigation. |
| **AdjusterPro** | Online licensing courses + exam prep + IA firm directory | Training only. No marketplace. No placement. Old-school website. |
| **AE21, 360training, USCI** | Pre-licensing courses for insurance adjusters | Same — training content only. No connection to demand side. |
| **CatAdjuster.org** | Community forum + job board | Not a platform. No matching, no tools, no training. |
| **Frontier Adjusters** | National network of independent adjusters | Traditional staffing firm. Phone calls and spreadsheets. Not tech. |
| **Independent Adjusting firms** (Pilot, etc.) | Recruit, (barely) train, dispatch adjusters | Staffing agencies, not platforms. Alacrity's bankruptcy shows this model failing. |
| **Sedgwick "Digital Adjust Pro"** | Experienced desk adjusters + Sedgwick's tech stack, outsourced to carriers. Claims up to $100K. | **Closest to the vision** but: not a marketplace, not a training pipeline, not open, US only through Sedgwick's own staff. You must buy the full TPA service. |

**What DOESN'T exist:**
1. A two-sided marketplace matching insurers/TPAs with licensed adjusters on-demand
2. A "train → license → equip → dispatch" pipeline
3. Training that includes AI-powered tools (everyone trains on Xactimate, nobody trains on AI-assisted adjustment)
4. A platform where the adjuster gets the tools AND the work through the same system

### Licensing Requirements — Lower Barrier Than Expected

**US licensing is NOT hard:**
- **No college degree needed** — high school diploma/GED is sufficient
- ~35 states require a license, ~15 states don't require one at all
- Pre-licensing education: 40-120 hours of online courses depending on state
- Pass a state licensing exam
- Background check
- **Total time: 2-4 months from zero to licensed adjuster**
- Texas and Florida are the most popular "Designated Home States" for non-residents
- CAT adjusters get licensed in multiple states ($50-200 per state fee)
- Professional certifications (AIC, CPCU) help but aren't required

**This means you could train someone from scratch to a licensed adjuster in 3-4 months.** That's fast enough to build a pipeline.

### The Proposed Model: Software + Training + Dispatch

This is NOT a pure marketplace. It's a **tech-enabled adjusting workforce** — you control the supply side.

| Layer | What | Revenue | Margin |
|---|---|---|---|
| **1. The Suite** | AI-powered adjuster tools: intake, triage, estimation assist, documentation, task management, carrier portal | SaaS: $3,000-8,000/seat/year or $50-150/claim | ~70-80% |
| **2. Training** | Online courses to get licensed + trained on YOUR tools. 3-4 month program. Ongoing CE. | Tuition: $2,000-5,000/student or free (subsidized by dispatch revenue) | ~80% on tuition, or loss-leader |
| **3. Dispatch** | Match your trained, tool-equipped adjusters with insurers/TPAs who need capacity. On-demand or contract. | Take rate: 15-25% on each engagement, or per-claim fee to insurer | ~20-30% |

**Why this model works:**

1. **Your adjusters use YOUR tools.** You train them on your platform, they do all their work through your platform. You own the workflow data, the decision data, and the relationship.

2. **Every claim generates training data.** The decision ground truth moat we identified — WHY the adjuster decided what they decided — accumulates automatically because they're working in your system.

3. **You solve supply AND tools simultaneously.** An insurer/TPA doesn't just get software or just get people — they get people equipped with the best tools. That's a much stronger value prop than either alone.

4. **The training pipeline creates captive supply.** If you're the one who trained them, licensed them, and gave them their first clients — they're loyal to your platform. Switching costs are high.

5. **AI makes less-experienced adjusters perform at senior level.** The 3-4 month pipeline works because your AI tools (coverage guidance, estimation assist, documentation automation) fill the experience gap. A year-1 adjuster on your platform performs like a year-5 adjuster without it.

6. **CAT spikes = massive demand = surge pricing.** When a hurricane hits, every insurer needs 500 adjusters overnight. If you have a trained, licensed network of 5,000+ adjusters who already know your tools — you're the first call.

### US Market Sizing

**The demand side:**

| Buyer Segment | Count | Adjusters Needed | Willingness to Pay |
|---|---|---|---|
| **Mid-tier TPAs** ($50-500M) | ~20-40 | 200-2,000 each | $500K-5M/year for staffing + tools |
| **Regional carriers** | ~200-400 | 20-200 each | $100K-1M/year |
| **Large carriers** (overflow/CAT) | ~30-50 | 500-5,000 during events | Per-claim or per-day rates |
| **MGAs needing claims capacity** | ~100-200 | 5-50 each | Per-claim fees |
| **Public adjusting firms** | ~1,000+ | 2-20 each | Lower budget but high volume |

**The supply side:**

| Metric | Value |
|---|---|
| New adjusters needed per year (to replace 20% attrition of 200K) | **~40,000** |
| Current training pipeline (all platforms combined) | Probably ~15,000-20,000/year |
| **Supply gap** | **~20,000-25,000 adjusters/year** |

**TAM calculation:**

| Revenue Stream | Conservative | Moderate | Optimistic |
|---|---|---|---|
| SaaS (tools to adjusters + insurers) | $30M | $75M | $150M |
| Dispatch (take rate on placements) | $50M | $150M | $400M |
| Training (courses, licensing) | $10M | $30M | $75M |
| **Total** | **$90M** | **$255M** | **$625M** |

**Blended margins:** ~40-55% (higher than pure services, lower than pure SaaS)

### Why Nobody Has Built This Yet

1. **Insurance is a relationships business.** Insurers have trusted their IA firms for decades. Building a tech platform to disrupt that requires the relationships breaking down first — and they're breaking down NOW (Alacrity bankruptcy, carrier churn, shortage crisis).

2. **Liability concerns.** If a marketplace adjuster makes a bad call, who's liable? E&O insurance is expensive and complex. BUT: Sedgwick's Digital Adjust Pro proves the model works — outsourced adjusters making coverage decisions up to $100K.

3. **Two-sided marketplace chicken-and-egg.** You need adjusters to attract insurers, and insurers to attract adjusters. BUT: if you start with training, you create the supply side yourself. You don't wait for adjusters to show up — you create them.

4. **Capital-intensive to start.** Training programs, licensing, E&O insurance, CMS integration. More expensive than pure SaaS. BUT: the economics improve at scale (each new adjuster = recurring revenue from dispatch + SaaS).

5. **Insurance is conservative.** Carriers don't want to be the first to try something new. BUT: the shortage is forcing their hand. When you can't hire enough adjusters, you'll try anything.

### How This Connects to the EU Strategy

**It doesn't — directly.** This is a US-only play because:
- US has 200,000+ adjusters and massive TPA market ($115B)
- EU has no equivalent adjuster marketplace or TPA structure
- EU motor barely uses external adjusters (conventions + internal handlers)
- EU property uses independent adjusters but per-claim, not as TPA employees

**BUT — there's an indirect connection:**
- The **SaaS tools** you build for US adjusters (intake, triage, estimation assist, documentation) could be adapted for the EU claims handler market
- The **training methodology** (AI-assisted tools that make juniors perform like seniors) applies anywhere
- **Revenue from the US dispatch business** could fund the EU SaaS expansion

**A possible dual-strategy:**
- **US:** Software + Training + Dispatch (adjuster workforce platform)
- **EU:** SaaS-only (document intake, parsing, convention matching, third-party management for mid-market insurers)
- **Shared:** Core AI/ML models, product infrastructure, design system

This is two different go-to-market strategies on shared technology. More complex to execute but addresses both markets with the right model for each.

---

## 15. Updated Strategic Paths (All Four)

| | Path 1: EU STP Gap | Path 2: US Property Adjuster OS | Path 3: EU Doc Intake Wedge | Path 4: US Adjuster Workforce Platform |
|---|---|---|---|---|
| **What** | Fix data quality → unlock convention STP | Unified property adjuster tools | Document intake/parsing/extraction for EU SME insurers | Software + Train + Dispatch adjusters |
| **Where** | EU only | US first, maybe EU | EU only | US only |
| **TAM** | €60-150M | $300-700M | €90-160M (with land-and-expand) | $90-625M |
| **Defensibility** | ✅✅✅ Very high | ⚠️ Medium | ✅✅ High (no one targeting segment) | ✅✅ High (supply creation = moat) |
| **Competition** | omni:us, MarvelX (small) | Verisk, Assured ($1B), Sedgwick | Nobody specifically | WeGoLook (narrow), dying IA firms |
| **Sales cycle** | 2-4 months (SME insurers) | 18-30 months (TPAs) | 2-4 months (SME insurers) | 3-6 months (TPAs need people NOW) |
| **Revenue model** | SaaS per-insurer | SaaS per-seat or per-claim | SaaS per-insurer (land & expand) | SaaS + take rate + training |
| **Margins** | ~70-80% | ~70-80% | ~70-80% | ~40-55% (blended) |
| **Time to revenue** | 6-12 months | 18-30 months | 3-6 months (Caravela = proof) | 6-12 months |
| **Capital needed** | Bootstrap possible | $5-10M seed | Bootstrap possible | $3-5M seed |
| **Venture-scale?** | Borderline (need expansion) | Yes, clearly | Borderline (need expansion) | Yes (moderate to optimistic) |
| **Exit** | €100-300M acquisition | $500M-2B IPO/acquisition | €160-600M PE/acquisition | $300M-1B acquisition |
| **Key risk** | Insurers fix it themselves | Verisk convergence | Market too fragmented | Liability + quality at scale |

### The Combinable Strategies

**Option A: EU-only (Paths 1 + 3 combined)**
- Start with document intake wedge (Path 3) for fast revenue
- Layer in STP gap / convention matching (Path 1) for defensibility
- Bootstrap → PE/strategic exit
- **Founders who want control, EU-based, technical**

**Option B: US-only (Paths 2 + 4 combined)**
- Start with adjuster workforce platform (Path 4) for supply + tools
- Expand into full property adjuster OS (Path 2) once you have distribution
- Raise venture capital
- **Founders who want to go big, US-based or willing to relocate**

**Option C: Dual-market on shared tech (Paths 3 + 4)**
- EU: SaaS for mid-market insurers (doc intake → parsing → convention → workflow)
- US: Software + Train + Dispatch for adjusters
- Shared: AI/ML models, product infrastructure
- Most ambitious but also most complex
- **Requires co-founders in both markets**

---

## 16. Why Nobody Is Building for the Hard Part of Adjusting

### The Pattern We Documented

Look at every startup in section 5:

| Company | What they automate | What they DON'T touch |
|---|---|---|
| **Assured** ($1B) | FNOL, messaging, document collection, correspondence | Coverage decisions, investigation, damage estimation |
| **FurtherAI** ($25M) | Intake, policy comparison, compliance checks | Coverage decisions, investigation, estimation |
| **Avallon** ($4.6M) | Calls, emails, document triage, data entry | Coverage decisions, investigation, estimation |
| **Sprout.ai** ($38M) | Document AI, triage, fraud detection | Coverage decisions, investigation, estimation |
| **Strada** | Voice AI for FNOL | Everything after FNOL |
| **Agentech** ($3M) | 100+ AI agents per claim file | Claims they describe as "4x output" are admin tasks |
| **MarvelX** (€5.4M) | Claims processing, fraud, customer comms | Coverage decisions, investigation, estimation |
| **omni:us** (~€45M) | End-to-end claims automation, document processing | Their "70% auto-settlement" is for SIMPLE claims only |

**Every single startup automates the ADMIN around the adjuster's work — none of them automate the actual ADJUSTER'S WORK:**
- Triage: Which claims need investigation vs. can be fast-tracked?
- Coverage analysis: Does this policy cover this loss? What's excluded?
- Investigation: What actually happened? Is this fraudulent?
- Damage estimation: What does this repair actually cost?
- Liability determination: Who's at fault and for how much?
- Reserve setting: How much should we set aside for this claim?
- Settlement negotiation: What's the right amount to offer?

### 5 Reasons Startups Avoid the Hard Part

**1. Liability terror — "bad faith" lawsuits**

This is the #1 reason. If your AI recommends "deny this claim" or "pay $5,000" and the adjuster follows it, and the policyholder sues for bad faith — **your startup is in the blast radius.** This isn't theoretical:
- Dozens of lawsuits have already been filed over AI-influenced claims decisions (as of 2025)
- Courts are starting to examine whether AI-assisted denials constitute unfair claims practices
- "If an adjuster cannot explain why a claim was denied, it's more difficult for the insurer to prevail"
- State regulators demand explainability — opaque AI denials = regulatory risk

**The FNOL/intake/correspondence layer is SAFE** — nobody sues because your AI collected their photos faster. The coverage decision layer is a MINEFIELD. So every startup rationally picks the safe side.

**2. Regulation is a moving target (US)**

- By late 2025: 23 states + DC adopted the NAIC AI Model Bulletin
- Each state has different Unfair Claims Practices Acts
- AI cannot make "final" coverage decisions without human review — required by law in most states
- Algorithmic bias concerns: AI trained on historical data may perpetuate past discrimination
- Result: you can't build "AI that decides claims" — you must build "AI that assists humans who decide claims"
- This makes the product more complex (human-in-the-loop design) and the value prop softer ("assists" vs "automates")

**3. Xactimate gravity for estimation**

- 75-80% of ALL property claims estimated in Xactimate
- Verisk's Xactimate ecosystem is OPEN — APIs, third-party integrations, partner program (RoofScope, Hover, Scope Technologies all plug in)
- So you CAN integrate. But you're building on Verisk's platform, and they could build your feature any day.
- Competing with Xactimate on estimation is essentially impossible
- You must build AROUND Xactimate (workflow, triage, investigation) not AGAINST it

**4. Domain expertise gap**

Building triage/decision/investigation tools requires DEEP insurance knowledge:
- Policy language interpretation (coverage A vs B vs C, exclusions, endorsements, sub-limits)
- State-by-state regulation differences (50 states × different rules)
- Coverage nuances (is this "sudden and accidental" or "gradual"? — the answer determines coverage)
- Claims investigation methodology (scene documentation, recorded statements, cause & origin)
- Fraud indicators (SIU referral criteria, red flags, behavioral analysis)

**Tech founders don't have this knowledge.** And insurance people who do have it usually don't start tech companies — they become senior adjusters or claims managers making $120-180K/year. The talent intersection of "deep claims expertise" + "can build software" is incredibly thin.

**5. The easy stuff is where the quick wins are**

VCs want fast traction. The fastest path to showing metrics is:
- "We automated FNOL intake — 30x faster!" (FurtherAI)
- "70% of interactions handled autonomously!" (Assured)
- "98% accuracy on document processing!" (Sprout.ai)

These are real, measurable, fast to build, and easy to sell. Telling a VP Claims "we'll help your adjusters make better coverage decisions" is harder to quantify, longer to prove, and scarier to buy.

### Why This Gap Is the ACTUAL Opportunity

**Everyone is crowding into the same safe space.**

Assured, FurtherAI, Avallon, Sprout.ai, Strada, Agentech — they're all fighting over FNOL, document intake, correspondence, and data entry. That space is getting crowded FAST. $1B+ in combined funding competing for the same admin automation layer.

**The hard part — triage, coverage analysis, investigation, estimation workflow, settlement — is where:**
- The actual money is spent (~70% of claims cost is in the decision + investigation + settlement phases, not the admin)
- The adjuster shortage hurts most (you can't automate a coverage decision with a chatbot)
- The moat is deepest (domain expertise + decision data = defensible)
- The competition is lightest (everyone's scared of liability + regulation)

**The startups that ARE starting to touch it:**

| Company | What they're doing | How far along |
|---|---|---|
| **Five Sigma / Clive** ($20M) | "Automates coverage validation" + "determines liability through AI-driven analysis" | Most aggressive — actually building the decision layer |
| **CCC EvolutionIQ** ($730M acquisition) | Tells adjusters "what to do next" on injury claims — triage + investigation guidance | Production at scale, but injury/casualty only, not property |
| **Crawford Turvi / CoverAI** | AI-driven policy coverage review — interprets policy language for coverage decisions | Early (2025 launch), Crawford-only initially |
| **Shift Technology** ($320M) | Fraud → expanding to full claims automation | Fraud-first, moving toward decisions |

**Notice: these are the BEST-FUNDED players.** Clive has $20M but is the most aggressive on decisions. CCC paid $730M for EvolutionIQ specifically because it's the decision guidance layer. Crawford built CoverAI as Turvi's flagship product. Shift raised $320M and is expanding from fraud into decisions.

**The market is TELLING you where the value is** — the most money flows to companies that touch decisions, not admin.

### What "Building for the Hard Part" Actually Looks Like

You don't build "AI that makes coverage decisions" (that's illegal in most states). You build **"AI that makes adjusters faster and better at the hard parts":**

**Triage Copilot:**
- Claim comes in → AI analyzes docs, photos, policy → recommends: fast-track / standard / complex / SIU referral
- Adjuster reviews recommendation, overrides or confirms
- System learns from every override (decision ground truth)

**Coverage Analysis Assist:**
- Adjuster opens claim → AI reads the policy, highlights relevant coverage sections, flags exclusions, identifies sub-limits
- "Based on this policy and loss description, Coverage A applies with $X deductible. Note: exclusion for gradual water damage may apply — recommend investigation of causation."
- Adjuster makes the call, but AI did 80% of the reading work

**Investigation Guidance:**
- Based on claim type and initial data → AI suggests investigation steps: "Request recorded statement from insured. Order cause & origin inspection. Check weather data for reported date."
- Tracks investigation progress, flags overdue items
- Learns which investigation patterns lead to accurate resolutions

**Estimation Workflow (around Xactimate, not replacing it):**
- Pulls Xactimate estimate data → validates against regional pricing, historical patterns, carrier guidelines
- Flags: "This estimate is 23% above regional average for this claim type. Line items X and Y appear elevated."
- Supplement cycle management — tracks back-and-forth between contractor and carrier

**Reserve Assist:**
- Based on claim data, coverage, initial estimate → AI suggests reserve range
- "Similar claims in this ZIP code with this loss type settle for $12,000-$18,000. Suggest initial reserve of $15,000."
- Tracks reserve accuracy over time → learns

### Why the Liability Risk Is Manageable

The legal key is: **AI recommends, human decides.** This is already established:

- CCC EvolutionIQ does exactly this — "guidance" not "decisions" — and CCC is a $13B public company. If they can manage the liability, a startup can too.
- Five Sigma/Clive explicitly "automates coverage validation" — they're already in the decision space.
- Crawford's CoverAI interprets policy language for coverage decisions — at a public company with $1.3B revenue.
- Every state's Unfair Claims Practices Act requires a human to make the final decision. As long as your product is a "copilot" not an "autopilot," you're within the regulatory framework.

The comparison: **Doctors use AI diagnostic tools (e.g., radiology AI). The AI flags potential findings, the doctor makes the diagnosis. The AI company is not liable for the doctor's decision.** Same structure applies to claims.

### The Honest Assessment

**The hard part of adjusting (triage, coverage, investigation, estimation, settlement) is the biggest gap in the market.** Everyone avoids it because of liability fear, regulatory complexity, and domain expertise requirements. But:

1. The liability is manageable with human-in-the-loop design (CCC, Five Sigma, Crawford prove this)
2. The regulation requires explainability, not avoidance — build explainable AI, not black boxes
3. The domain expertise is the MOAT — if it's hard for you, it's hard for every other startup too
4. The value is 5-10x higher than admin automation — adjusters don't need faster document intake, they need help making better decisions faster
5. The competition is lightest precisely where the value is highest

**This is the contrarian bet.** Everyone else is building the safe, obvious thing (FNOL/intake/docs). The outlier outcome comes from building the hard, scary thing (decisions/investigation/estimation workflow) — with the right guardrails.

---

## 17. The Unbiased Opportunity Assessment — Which Is Actually Bigger?

*Setting aside who the founders are, where they're located, or what they've built so far. Pure opportunity analysis.*

### Why the US Adjuster Workforce Platform Is the Bigger Opportunity

**1. Urgency creates demand NOW.**
EU mid-market insurers have been on legacy systems for 20 years — they can wait another year. US TPAs literally cannot find adjusters TODAY. Alacrity (major IA firm) just went bankrupt. 20% attrition every year, 25% retiring within 5 years. When the buyer is desperate, sales cycles collapse and willingness to pay goes up. Urgency is the single best thing a startup can have.

**2. You can manufacture supply — that's rare.**
Most labor marketplaces can't create supply — training doctors takes 10 years, lawyers 7, engineers 4. Insurance adjusters? High school diploma + 40-120 hours online + state exam = **licensed in 3-4 months.** You can literally produce the supply side of your marketplace. Andela did this for software developers in Africa ($1.5B valuation). Same playbook.

**3. AI is the actual disruption, not just a feature.**
In the EU SaaS play, AI makes document processing faster. Nice but incremental — the insurer was processing documents before, just slower. In the US adjuster play, AI fundamentally changes WHO can do the job. A 3-month trained adjuster with AI tools performs like a 5-year veteran. You're not filling the supply gap — you're **changing the economics of the entire profession.** That's a platform shift, not a product improvement.

**4. The moat is the supply network itself.**
Once you've trained 5,000 adjusters on your tools, given them work, and built their track record — you have:
- Captive supply (they won't switch — you trained them, equipped them, gave them their career)
- Workflow data from every claim (AI keeps getting better with each claim processed)
- Insurer trust (proven track record, quality metrics, consistent output)
- Network effects (more adjusters → more insurers → more adjusters → more data → better AI)

The EU SaaS moat is convention expertise + distribution. Real but replicable — someone with enough engineers and domain experts could rebuild it. The US workforce moat is the supply network itself — 5,000 trained, equipped, tracked adjusters with performance history. That takes years to replicate.

**5. The incumbents are weaker than they appear.**
- IA firms are dying (Alacrity bankrupt, carriers cutting loose independent firms)
- WeGoLook is deliberately limited to photos/inspections — Crawford chose NOT to go further
- AdjusterPro/360training are content companies, not platforms — they train people and wave goodbye
- Sedgwick's Digital Adjust Pro is bundled with their TPA service — can't buy just the tools + people
- **Nobody — not one company — combines train + equip + dispatch as a standalone platform**

**6. The "services" stigma is outdated.**
VCs used to penalize anything that wasn't pure SaaS. That's 2015 thinking. Today's market values "software-enabled services" where you own the workflow AND the supply side:
- Rippling (software + HR services): $13.5B valuation
- Deel (software + compliance services): $12B valuation
- Andela (software + developer marketplace): $1.5B valuation
- Hims & Hers (software + health services): $5B+ public

The pattern: software that creates and controls a supply network is valued HIGHER than pure SaaS because it's harder to displace.

### The Honest Bear Case

**1. Quality at scale is genuinely the hardest part.**
Training 50 good adjusters is manageable. Training 5,000 across specialties (property, auto, liability, workers comp, CAT) with consistent quality? That's an operations beast. One bad adjuster who misses fraud, botches a $200K claim, or mishandles a policyholder creates liability AND reputation damage. You need robust QA, supervision, ongoing training, and performance management. This is NOT a "ship code and forget it" business.

**2. Liability is real and expensive.**
Adjusters make coverage decisions worth thousands to millions. E&O (Errors & Omissions) insurance is significant cost. If your platform-trained adjuster makes a bad call, the insurer comes after you. This isn't Uber where the driver's personal insurance covers accidents — you're in the liability chain.

**3. CAT dependency creates revenue volatility.**
The adjuster shortage is worst during catastrophe season (hurricanes, wildfires, hailstorms). Quiet years = less demand. Revenue could swing 30-40% year-over-year based on weather. VCs hate revenue volatility. Counter: climate change is making CAT events more frequent, not less.

**4. The big TPAs could unbundle.**
If Sedgwick decides to sell Digital Adjust Pro as standalone (not just as part of their TPA service), they start with 33,000 employees and every carrier relationship. Same if Crawford opens WeGoLook to full adjusting. They haven't yet — but they could.

**5. Margins will always be lower than pure SaaS.**
40-55% blended vs 70-80% pure SaaS. This matters for valuation multiples. You'd need to prove the SaaS layer grows faster than the services layer over time, eventually becoming the majority of revenue.

### The Pure-Opportunity Head-to-Head

| | EU SaaS (Mid-Market Insurers) | US Adjuster Workforce Platform |
|---|---|---|
| **Buyer urgency** | Low — lived with legacy for years | **HIGH — can't hire, people retiring NOW** |
| **TAM** | €90-160M | $90-625M |
| **Disruption level** | Incremental (faster doc processing) | **Structural (AI changes who can do the job)** |
| **Moat type** | Convention expertise + distribution | **Supply network + workflow data + AI flywheel** |
| **Moat durability** | Medium (replicable with enough effort) | **High (supply network takes years to build)** |
| **Revenue quality** | Pure SaaS, 70-80% margins | Blended 40-55%, but 3 revenue streams |
| **NRR potential** | ~130% (land and expand) | ~140%+ (more adjusters + more tools per adjuster) |
| **Competitive intensity** | Low (nobody targeting segment) | Medium (incumbents exist but are weak/narrow) |
| **Execution complexity** | Lower (pure software) | Higher (ops + software + training + QA) |
| **Capital to start** | Low (bootstrap possible) | Medium ($3-5M seed) |
| **Time to revenue** | 3-6 months | 6-12 months |
| **Venture potential** | Borderline (€160-600M exit) | **Strong ($300M-1.5B+)** |
| **Comparable exits** | omni:us, MarvelX (still small) | Andela ($1.5B), Rippling ($13.5B model) |

### The Verdict

**The US adjuster workforce platform is the bigger, more disruptive, more venture-scale opportunity.**

The urgency is real (not theoretical), the disruption is structural (not incremental), the moat is harder to replicate (supply network vs software features), and the market rewards this model today (Andela, Deel, Rippling prove it).

The EU SaaS play is safer, cheaper to start, more capital-efficient, and genuinely defensible in its niche. It's a great business — potentially €20-40M ARR with strong margins. But it's a smaller game with a lower ceiling.

**If you're optimizing for probability of building a good business** → EU SaaS (Paths 1+3)
**If you're optimizing for the size of the outcome** → US Adjuster Workforce (Path 4)
**If you want both and can handle the complexity** → Dual-market (Option C)

The co-founder conversation should be about which optimization function matters more — and whether you have (or can find) the right people for each path.

---

## 18. Complete Market Sizing — All Buyer Types, EU and US

*Research compiled February 7, 2026. Sources at bottom of section.*

### The Big Picture — Side by Side

| | **United States** | **European Union/EEA** |
|---|---|---|
| **Total non-life premiums** | ~$1.06 trillion DWP (2024) | ~€400-450B GWP (2023) |
| **Total non-life claims/year** | ~45-50 million | ~55-70 million |
| **Total losses + LAE** | $632B (2024) | ~€300-350B (2023 est.) |
| **Insurance carriers** | ~4,100 entities (~647 groups) | ~2,141 solo undertakings + 95 groups |
| **Insurance employees (carriers)** | ~666,000 (P&C carriers) | ~460,000-500,000 (non-life) |
| **Claims adjusters/examiners** | ~313,000-356,000 (all settings) | ~180,000+ (est. claims staff) |
| **TPAs** | ~300-500 significant P&C firms, $115B market | Growing, ~$91B market (2023), less mature |
| **MGAs** | ~850-1,000+, $114B managed premium | 650+, €18B GWP |
| **Brokers/agencies** | ~443,000 total (39,000 independent P&C) | 10,000+ brokerage firms + hundreds of thousands of agents |
| **Independent adjusting firms** | ~53,000 businesses, $11.7B market | Fragmented — Crawford EU, McLarens, Sedgwick Europe |

---

### US MARKET — Carriers by Size Band

**~4,100 P&C legal entities (~647 groups) writing $1.06 trillion in DWP.** The top 10 groups hold 51.4% market share. The top 25 hold ~70%.

| Size Band | DWP Range | # of Companies | % of Companies | Aggregate DWP | % of Industry | Avg Employees | Claims Staff | Claims/yr per co. |
|---|---|---|---|---|---|---|---|---|
| **Micro** | <$50M | ~2,800-3,000 | ~70% | ~$40-50B | ~4-5% | 50-150 | 15-40 | 1,000-3,000 |
| **Small** | $50-250M | ~600-700 | ~16% | ~$75-90B | ~7-8% | 200-600 | 60-150 | 3,000-15,000 |
| **Mid-market** | $250M-1B | ~250-300 | ~7% | ~$125-150B | ~12-14% | 800-2,500 | 200-600 | 10,000-50,000 |
| **Upper-mid** | $1B-5B | ~100-120 | ~3% | ~$200-250B | ~20-23% | 3,000-10,000 | 800-2,500 | 50,000-200,000 |
| **Large** | $5B+ | ~40-50 | ~1% | ~$550-600B | ~52-55% | 10,000-70,000 | 3,000-15,000 | 200,000+ |

**Caravela equivalent in US (~$200M DWP):** ~600-700 companies in the $50-250M band. Demotech classified 147 as "Super Regional" ($100M+ surplus, $50M+ net premiums). A $200M carrier typically: 300-600 employees, 80-150 claims staff, 15,000-40,000 claims/year (varies by line mix).

**Line mix matters enormously:**
- Personal auto-heavy $200M carrier: ~30,000-40,000 claims/year (high frequency)
- Homeowners-heavy $200M carrier: ~4,800 claims/year (lower frequency, higher severity)
- Commercial multi-line $200M carrier: ~8,000-12,000 claims/year
- Workers' comp $200M carrier: ~10,000-15,000 claims/year

---

### US MARKET — TPAs (Third Party Administrators)

| Metric | Value |
|---|---|
| US TPA market size | **$115B** (2024) → $255B by 2034 (8.3% CAGR) |
| Significant P&C TPAs | **~300-500 firms** (IBISWorld counts 123K but that includes all IA shops + health TPAs) |
| Market concentration | Low — top 10 TPAs hold only 3-5% |
| Share of all P&C claims | **~20-30%** handled by TPAs/outsourced adjusters |

**Major TPAs:**

| Company | Revenue | Employees | Claims/Year | Key Facts |
|---|---|---|---|---|
| **Sedgwick** | ~$5B (P&C: ~$3.2B) | 33,000 | 8M+ claims (2023) | World's largest. $13.2B enterprise value. 10,000+ clients. |
| **Gallagher Bassett** | ~$500M+ | ~4,200 | 800,000+ new/yr | Subsidiary of AJG. 100+ offices. |
| **Davies Group** | ~$1.7B | 8,500 | 200,000+ (TPA alone) | Largest UK TPA. Licenses ClaimPilot externally. |
| **Crawford / Broadspire** | $1.29B (Broadspire ~$750M) | ~9,000 | Multi-million | Only big TPA selling AI externally (Turvi). |
| **CorVel** | ~$780M | ~5,500 | N/A | Public. WC and auto heavy. |
| **ESIS (Chubb)** | Not disclosed | Part of Chubb 31K | N/A | Captive TPA. WC, liability. |

**Mid-tier TPAs ($50-500M revenue):** Estimated **50-100 firms** — Tristar, Helmsman (Liberty), Charles Taylor, York Risk Services, CompManagement. These are the buyers who buy rather than build. Consolidating rapidly — coordinated state exams across 41 states force smaller TPAs to join larger platforms.

---

### US MARKET — MGAs (Managing General Agents)

| Metric | Value |
|---|---|
| Total US MGAs | **~850-1,000+** (Conning identifies 850+ from statutory filings) |
| Total DWP via MGAs | **$114.1B** (2024, Conning) — 16% YoY growth, 4th consecutive year of double-digit growth |
| MGA share of US P&C market | **~10%+** |
| Average premium per MGA | ~$114M (heavily skewed — most smaller, top 5 = 20%) |

**Do MGAs handle claims?** It varies. ~20-30% of MGAs have some level of claims-handling authority, but full settlement authority is rarer. The trend is toward MGAs taking on more claims functions. Most MGAs do underwriting only — claims revert to the carrier.

**Top US MGA players:** Ryan Specialty ($2.52B revenue, 21% growth), Brown & Brown, Amwins, CRC Group, AmRisc (#1 independent for 4 years). ~3,000 MGA enterprises globally; 2,170+ projected to generate $10M+ in premiums by 2025.

**As Mysa buyer:** MGAs with claims authority are a real buyer segment. They need claims tools but are too small to build. Per-claim pricing works well for them. ~200-300 MGAs with claims authority = addressable segment.

---

### US MARKET — Brokers & Agencies

| Metric | Value |
|---|---|
| Total brokers/agencies (all lines) | **442,833** (IBISWorld 2025) |
| Independent P&C agencies specifically | **~39,000** (down from 40K in 2022) |
| Market revenue | **$261.7B** |
| Independent agency channel market share | **61.5%** of all P&C insurance (2024) |

**Size distribution of independent agencies (2024 Agency Universe Study):**
- Under $150K revenue: 27.1% (~10,500 agencies)
- Under $500K revenue: 51.6% (~20,100 agencies)
- Over $500K revenue: 48.4% (~18,900 agencies)
- Trend: agencies getting larger (10-point shift toward $500K+)

**Top brokers (2024 revenue):** Marsh McLennan (~$24B), Aon (~$14B), Gallagher (~$10.6B), WTW (~$10B), Brown & Brown (~$4.8B).

**Do US brokers handle claims?** **No.** They are a distribution channel. Claims advocacy only (help clients navigate the process, recommend TPAs). They do NOT adjudicate, investigate, or settle claims. **Brokers are NOT a buyer for claims tools** — they're a buyer for distribution/intake tools.

---

### US MARKET — Independent Adjusting Firms

| Metric | Value |
|---|---|
| Claims Adjusting industry market size | **$11.7B** (IBISWorld 2025) |
| Number of businesses | **53,358** (IBISWorld 2024) |
| Total claims adjusters (all settings, BLS) | **312,810-356,100** |
| BLS median wage | $76,790 |
| Employment outlook (2024-2034) | **-5% decline** |

**Major players:** Pilot Catastrophe ($969M), Alacrity Solutions (~$856M, restructured 2025), E.A. Renfroe (~$348M), Crawford (also counted above), Claim Assist Solutions (2,000 employees + 17K contractors). Independent adjusters handle **~3.5M claims/year** and distribute **>$500B in claim payments**.

**The Alacrity story:** BlackRock acquired for ~$560M in PE equity. By late 2024, entered restructuring. March 2025: eliminated ~$1B in debt, BlackRock lost entire $560M investment. Control passed to Antares/Blue Owl/KKR. Cautionary tale about CAT-dependent business models.

---

### US MARKET — Claims Volume by Line

| Line | Claims/Year | Total Losses | Avg Claim Size |
|---|---|---|---|
| **Auto — Collision** | ~11M | — | $5,489 |
| **Auto — Comprehensive** | ~10.5M | — | $2,306 |
| **Auto — PD Liability** | ~6.6M | — | $6,770 |
| **Auto — BI Liability** | ~2.1M | — | $28,278 |
| **Total Auto** | **~30-32M** | **$263B** | Mixed |
| **Homeowners** | **~4.2M** (5.3% of 80M insured homes) | **~$104B** | $17,059 avg |
| **Commercial Lines** | ~10-15M (est.) | **$234B** | Mixed |
| **Total P&C** | **~45-50M** | **$632B (losses+LAE)** | — |

**Homeowners by peril (2023):** Wind/hail 42.5%, water damage 29.4%, fire/lightning ~5%, theft 0.7%.

---

### EU MARKET — Carriers by Size Band

**~2,141 solo insurance undertakings + 95 groups (EIOPA 2024). Non-life focused = ~1,300-1,400 undertakings.**

| Size Band | GWP Range | # of Companies | Avg Employees | Total Employees | Claims Staff | Total GWP | Claims/yr per co. | Total Claims/yr |
|---|---|---|---|---|---|---|---|---|
| **Micro** | <€25M | ~900 | ~100 | ~90,000 | ~13,500 | ~€11B | 1,000-5,000 | ~2.7M |
| **Small** | €25-100M | ~450 | ~300 | ~135,000 | ~22,500 | ~€25B | 5,000-20,000 | ~5.4M |
| **Mid-market** *(Caravela)* | €100-500M | ~250 | ~600 | ~150,000 | ~30,000 | ~€62B | 15,000-80,000 | ~10M |
| **Upper mid** | €500M-2B | ~125 | ~2,500 | ~312,000 | ~62,500 | ~€125B | 80,000-300,000 | ~18.8M |
| **Large groups** | €2B+ | ~65 | ~4,000+ | ~260,000+ | ~52,000+ | ~€260B | 300,000+ | ~20M+ |
| **TOTAL** | | **~1,790** | | **~947,000** | **~180,000+** | **~€483B** | | **~57M** |

**Portugal specifically:** 66 companies / 40 groups. Top 3 = 59.2% (Fidelidade 30.2%, Ageas 16.3%, Generali 12.9%). Caravela at €187.7M sits roughly 5th-10th among Portuguese non-life.

**Country breakdown of mid-market (€100-500M) insurers:**

| Country | Mid-Market Insurers (est.) | Key Context |
|---|---|---|
| **Germany** | ~80-120+ | Largest. Regional mutuals, Sparkassen. BaFin-supervised. |
| **France** | ~60-80+ | Many mutuelles (MAIF, MACIF, Groupama). ACPR-supervised. |
| **Spain** | ~20-30 | CIDE/ASCIDE. Regional mutuals. Mapfre dominates. |
| **Italy** | ~20-30 | CARD mandatory. Generali/Unipol dominate. |
| **Benelux** | ~15-25 | Broker-dominated. Moderate tech maturity. |
| **Nordics** | ~20-30 | High digital maturity. Mid-market mutuals/cooperatives. |
| **Portugal** | ~5-10 | Small but fast-moving. Caravela here. |
| **CEE** | ~30-50 | Growing, lower tech adoption. |
| **Total** | **~250-400** | |

---

### EU MARKET — Brokers & Intermediaries

| Metric | Value |
|---|---|
| EU brokerage market revenue | **~€59B** |
| Intermediated GWP | **~€261B** (2024) → €371B by 2029 |
| Broker share of premiums | **~33%** (brokers alone); **55%** (all intermediaries) |
| Total intermediaries across EU | **Hundreds of thousands** (Germany alone: ~194K) |

**Country-level broker counts:**

| Country | Intermediaries | Broker Share (Non-Life) | Model |
|---|---|---|---|
| **Germany** | ~194,000 (148K tied agents + 46K brokers) | 41% broker / 46% tied agent | Mixed, shifting to brokers |
| **France** | ~64,000+ (ORIAS register) | Growing (18.5% in life) | Bancassurance dominant in life |
| **Spain** | ~56,900 (54K exclusive agents + 2.7K corredores) | Low broker share | Agent-dominated |
| **Italy** | Tens of thousands | 10.2% broker / 77% tied agent | Agent-dominated |
| **Belgium** | ~5,000 (down from 8K in 2012) | ~61% | Strongly broker-dominated |
| **Netherlands** | Thousands | 60.5% | Strongest broker market in EU |
| **UK** | Thousands of FCA-authorized | ~54% | Broker-dominated, esp. commercial |

**Major EU broker players (2024 revenue):**

| Broker | Revenue | Key Facts |
|---|---|---|
| **Howden Group** | GBP 3.01B (+23% YoY) | 20,000 employees. 28 European deals in 2024. |
| **Ardonagh Group** | $1.98B (+24% YoY) | 68 acquisitions in 2024. $14B enterprise valuation. |
| **PIB Group** | GBP 515-530M (+14% YoY) | 25+ acquisitions in 2024. Expanded to France, Portugal, Spain, Germany, Poland. |

**Do EU brokers handle claims?** Varies by country:
- **UK/Netherlands/Belgium:** Brokers play significant claims advocacy/intermediation role
- **Germany:** Brokers provide claims support, but adjusters manage formal process
- **Italy/Spain/Portugal:** Claims handled in-house by insurers or peritos. Brokers minimally involved.

**As Mysa buyer:** Brokers are NOT direct claims tool buyers. But they ARE the intake channel — a broker portal product (Product 5 from Section 12, €30-60K/yr) serves them. In UK/NL/BE where brokers handle claims notification, they're a more natural buyer for intake/triage tools.

---

### EU MARKET — TPAs

| Metric | Value |
|---|---|
| Europe TPA market | **$91.2B** (2023) → $156B by 2030 (6.9% CAGR) |
| Market maturity vs US | **Less mature** — driven by Lloyd's, insurer outsourcing, run-off |
| Most active countries | **UK** (most mature), Germany, Nordics, Benelux |
| Least active | **Southern Europe** — insurers handle claims in-house |

**Major EU TPA players:**

| Company | EU Revenue/Scale | Key Facts |
|---|---|---|
| **Davies Group** | ~$1.7B total, 1,000+ TPA team | Largest UK TPA. 200K+ claims/yr for 150+ clients. >GBP 1.5B annual claims spend. |
| **Sedgwick** | Part of 33K global | Offices in Belgium, Germany, Scandinavia. Complex property/liability, marine. |
| **Crawford** | International ops $418.6M (2024) | Belgium: 30K+ claims/yr. 12+ EU countries. |
| **Charles Taylor** | Specialist | London Market & Lloyd's focus. |
| **Gallagher Bassett** | Strong UK/Ireland | Part of Arthur J. Gallagher. |

**The TPA gap is still real:** In the US, mid-tier TPAs ($50-500M) buy software. In the EU, there is no equivalent mid-tier TPA market for property claims. European carriers handle claims internally. Independent loss adjusters come in per-claim for complex cases.

---

### EU MARKET — MGAs

| Metric | Value |
|---|---|
| Total EU MGAs | **650+** (Howden Re 2025) |
| Total EU MGA GWP | **€18B** (2024) |
| 5-year CAGR | **~23%** — outpacing US and global |
| Fastest growing in | UK (350+ MGAs, >GBP 4.7B), Benelux (180+, €3.5B), Italy (100+, €2.6B) |

**Regional breakdown:**

| Region | MGAs | GWP |
|---|---|---|
| **UK** | 350+ | >GBP 4.7B (>10% of UK GI market) |
| **Benelux** | 180+ | €3.5B |
| **Italy** | 100+ | €2.6B |
| **France** | 80-85 | €900M |
| **Spain & Portugal** | 80-85 | €320M |
| **Germany** | 60-70 | €950M |
| **Nordics** | 60-70 | €750M |

**Do EU MGAs handle claims?** Increasingly yes — AI-based triage, proprietary pricing engines, API-integrated claims. But full claims authority is still a minority. Lloyd's has flagged concerns about delegated authority quality. Trend is toward more MGA claims handling, especially in specialty lines.

**As Mysa buyer:** EU MGAs with claims authority (~130-200 of them) are a natural buyer segment. Small, tech-forward, need claims tools, can decide fast. The UK MGA boom (350+ and growing) is especially relevant.

**Global context (Insuramore 2024):** ~3,000 MGA enterprises globally. $29.25B global MGA revenue. $250B+ in written premiums. Top 500 by geography: US (267), UK (68), Canada (32), Germany (18), Netherlands (18).

---

### EU MARKET — Loss Adjusters

| Company | European Presence | Key Scale |
|---|---|---|
| **Crawford** | 12+ EU countries | International ops: $418.6M (2024). Belgium: 30K+ claims/yr. |
| **McLarens** | 230+ offices, 45 countries | 25% EMEA revenue growth (2024-2025). Acquired VWJ (Netherlands). |
| **Sedgwick** | Belgium, Germany, Scandinavia | 33,000 globally. Complex property/marine. |
| **RTS Group** | Spain-focused, 35+ years | Spanish/Portuguese market. |
| **ABACO International** | Spain + broader Europe | International loss adjuster network. |

**The perito model (Southern Europe):** In Spain/Portugal/Italy, loss adjusters are "peritos" — damage assessors employed by or exclusively contracted to specific insurers. Less independent than Anglo-Saxon model (Crawford/McLarens). This is Caravela's world — in-house peritos for motor and property, external peritaje firms for complex losses.

---

### EU MARKET — Claims Volume by Country

| Country | Non-Life GWP | Motor Claims/yr (est.) | Total Claims (est.) |
|---|---|---|---|
| **Germany** | €85.5B | ~8M | ~15-18M |
| **UK** | €60-65B | ~4-5M | ~10-12M |
| **France** | €50-55B | ~9M | ~14-16M |
| **Italy** | €35-40B | ~5-6M | ~9-11M |
| **Spain** | €25-30B | ~3-4M | ~6-8M |
| **Netherlands** | €20-25B | ~1.5-2M | ~4-5M |
| **Belgium** | €12-15B | ~1-1.5M | ~2.5-3M |
| **Nordics** (combined) | €30-35B | ~2-3M | ~5-7M |
| **CEE** (combined) | €25-30B | ~3-4M | ~5-7M |
| **Other EU** | €15-20B | ~1-2M | ~3-4M |
| **TOTAL** | **~€400-450B** | **~40-50M motor** | **~55-70M non-life** |

---

### Claims Processing Economics — US vs EU

| Metric | US | EU |
|---|---|---|
| **LAE as % of premium** | 9-12% | 6-9% |
| **Total LAE** | ~$80B (2024) | ~€30-40B (est.) |
| **Claims processing cost per claim** | $500-$1,500 (auto PD), $3K-$10K (BI), $1K-$3K (homeowners) | Lower — fewer legal costs |
| **Independent adjuster fee** | $415-$640 per claim | Per-claim perito fee varies by country |
| **IT spend as % of premium** | 5.0% (2024, up from 3.6%) | Similar trend but lower base |
| **Claims technology market** | Part of $4B CMS market | Part of €4.3B EU claims mgmt market (12.8% CAGR → €6.1B by 2030) |
| **Key difference** | US: much higher litigation costs ("social inflation") | EU: more regulated processes, lower litigation |

---

### The Complete Buyer Landscape — All Segments

**US — Who Would Buy Claims Tools?**

| Buyer Segment | Count | Revenue/Scale | Claims/yr | Willingness to Buy? | ACV Range |
|---|---|---|---|---|---|
| **Large carriers** ($5B+) | ~40-50 | $550-600B DWP | 200K+ each | ❌ Build their own | N/A |
| **Upper-mid carriers** ($1-5B) | ~100-120 | $200-250B DWP | 50-200K each | ⚠️ Long procurement, some buy | $500K-2M |
| **Mid-market carriers** ($250M-1B) | ~250-300 | $125-150B DWP | 10-50K each | ✅ Emerging buyer | $200K-500K |
| **Small carriers** ($50-250M) *Caravela equiv* | ~600-700 | $75-90B DWP | 3-15K each | ✅ **Sweet spot** | $50K-200K |
| **Micro carriers** (<$50M) | ~2,800-3,000 | $40-50B DWP | 1-3K each | ❌ Too small | N/A |
| **Big TPAs** (Sedgwick, Crawford, etc.) | ~10 | $10B+ combined | 10M+ combined | ❌ Build their own | N/A |
| **Mid-tier TPAs** ($50-500M) | ~50-100 | $5-15B combined | Several million | ✅ **Primary TPA buyer** | $500K-2M |
| **MGAs with claims authority** | ~200-300 | $25-35B managed | Varies | ✅ Need tools, decide fast | $50K-200K |
| **Independent adjusting firms** | ~53,000 | $11.7B market | 3.5M+ | ⚠️ Per-seat, small budgets | $5K-50K |

**EU — Who Would Buy Claims Tools?**

| Buyer Segment | Count | Revenue/Scale | Claims/yr | Willingness to Buy? | ACV Range |
|---|---|---|---|---|---|
| **Large carriers** (€2B+) | ~65 | ~€260B GWP | 300K+ each | ❌ Build their own (Allianz, AXA) | N/A |
| **Upper-mid carriers** (€500M-2B) | ~125 | ~€125B GWP | 80-300K each | ⚠️ Some buy, longer cycles | €200-500K |
| **Mid-market carriers** (€100-500M) *Caravela* | ~250 | ~€62B GWP | 15-80K each | ✅ **Sweet spot** (2-4 month sales) | €80-200K |
| **Small carriers** (€25-100M) | ~450 | ~€25B GWP | 5-20K each | ⚠️ Tight budgets, decide fast | €30-80K |
| **Micro carriers** (<€25M) | ~900 | ~€11B GWP | 1-5K each | ❌ Too small | N/A |
| **EU TPAs** (Davies, Crawford EU, etc.) | ~20-50 significant | Part of $91B EU market | 200K+ (Davies alone) | ⚠️ Big ones build, mid ones buy | €200K-1M |
| **MGAs with claims authority** | ~130-200 | Part of €18B | Varies | ✅ Fast-growing buyer segment | €30-100K |
| **EU brokers** (for intake tools only) | ~10,000+ firms | €59B revenue | Claims advocacy only | ⚠️ Intake/portal products only | €20-60K |
| **Loss adjusting firms** (Crawford EU, McLarens) | ~50-100 significant | ~€5-10B market | Millions combined | ⚠️ Build or buy internally | €100-500K |

---

### The Addressable Market — Consolidated

**US Addressable (companies that buy rather than build):**

| Segment | Companies | Total Claims/yr | TAM (low ACV × count) | TAM (high ACV × count) |
|---|---|---|---|---|
| Mid-market carriers ($250M-1B) | ~275 | ~8M | $55M | $138M |
| Small carriers ($50-250M) | ~650 | ~6M | $33M | $130M |
| Mid-tier TPAs | ~75 | ~3M | $38M | $150M |
| MGAs with claims authority | ~250 | ~1.5M | $13M | $50M |
| **Total US addressable** | **~1,250** | **~18.5M** | **$138M** | **$468M** |

**EU Addressable (companies that buy rather than build):**

| Segment | Companies | Total Claims/yr | TAM (low ACV × count) | TAM (high ACV × count) |
|---|---|---|---|---|
| Mid-market carriers (€100-500M) | ~250 | ~10M | €20M | €50M |
| Small carriers (€25-100M) | ~450 | ~5.4M | €14M | €36M |
| Upper-mid carriers (€500M-2B) | ~125 | ~18.8M | €25M | €63M |
| MGAs with claims authority | ~165 | ~1M | €5M | €17M |
| EU TPAs (mid-tier) | ~30 | ~1M | €6M | €30M |
| **Total EU addressable** | **~1,020** | **~36.2M** | **€70M** | **€196M** |

**Combined US + EU Addressable: ~2,270 companies, ~55M claims/year, $200-650M TAM**

**With land-and-expand (Section 12 model, 130% NRR):**
- Year 1 land at low ACV → Year 3+ at 3-4x ACV
- Effective TAM with expansion: **$400M-1.3B** at maturity

---

## 19. The Contrarian Bet Reframed — US (Motor + Property + Commercial)

*What's genuinely open vs what's already being built*

### The crowded spaces (don't go here)

Everyone is fighting over intake and admin. Assured, FurtherAI, Avallon, Sprout.ai, Strada — all competing to automate FNOL, document processing, and data entry. CCC + EvolutionIQ just spent $730M to own adjuster guidance for **auto casualty and workers' comp**. Verisk launched [XactAI](https://www.verisk.com/resources/campaigns/empowering-the-human-side-of-insurance/) in September 2025 — AI tools bundled free inside Xactimate Pro. The front door and the estimation tool are being automated.

### What nobody is building: the decision layer between intake and estimate

After FNOL is done and before the estimate opens, there's a critical workflow where adjusters:
- **Interpret coverage** — is this "sudden and accidental" water loss or a maintenance exclusion? Does the commercial manuscript form cover this scenario?
- **Triage complexity** — desk review, virtual inspection, or boots on the ground?
- **Scope investigation** — what needs validation before committing to a number?
- **Set reserves** — what's the realistic exposure here?
- **Decide the claim path** — pay, investigate, deny, negotiate, litigate?

That workflow lives in the adjuster's brain. There's no software for it. Xactimate prices the damage — it doesn't decide whether the damage is covered. The CMS tracks the file — it doesn't tell you what to do next. CCC's EvolutionIQ does this for auto casualty but **not property, not commercial, not specialty**.

### The competitive reality (honest)

**Verisk/XactAI** is in every property adjuster's hands but only does photo labels and transcription summaries — features, not decisions. Bundled free with Xactimate Pro. They COULD build a real decision engine on top of their 4.5B+ data points. That's the existential risk.

**Five Sigma/Clive** ($20M raised, [landed Starr](https://www.prnewswire.com/news-releases/starr-modernizes-pc-and-specialty-claims-with-five-sigmas-ai-claims-platform-and-clive-302669986.html) in Jan 2026) is the closest direct threat. Multi-agent AI adjuster copilot that works on any CMS. But they're selling a **full CMS + AI stack** — bigger sale, longer cycle, higher switching cost. An AI decision layer that works ON TOP of any CMS without ripping out infrastructure is a different, faster wedge.

**CCC + EvolutionIQ** ($730M, [targeting mid-market and large carriers](https://www.investing.com/news/company-news/ccc-intelligent-solutions-q1-2025-slides-aidriven-growth-and-evolutioniq-acquisition-93CH-4106995)) owns auto casualty guidance. 7 of top 15 disability carriers. $45-50M revenue in year one. But they have **zero property/commercial footprint** and no EU presence. Their moat is the 35,000-business auto network, which doesn't transfer to property.

**Crawford/Turvi** launched CoverAI (AI coverage review), Asservio (digital estimate review), and Digital Desk (triage). This is the closest to building the decision layer — but it's Crawford's proprietary product sold as part of their TPA stack, not available standalone.

**Shift Technology** ($320M, 25+ countries) just launched Shift Claims with agentic AI. AXA Switzerland reports 60% automation rate. But Shift starts downstream of coverage decisions — they automate the workflow AFTER triage, they don't make the triage decision itself. And they lead with fraud.

### The addressable market

- **500-600 mid-market P&C carriers** ($50M-$1B DWP) — too small for Guidewire enterprise sales, too big for manual workflows at 8,000-40,000 claims/year each
- **50-100 mid-tier TPAs** ($50-500M revenue) — differentiation pressure from Sedgwick/Crawford above, margin pressure from automation below
- **200+ MGAs with claims authority** — fastest growing segment (16% YoY), increasingly handling claims but with no purpose-built tools
- Combined: **~800 potential buyers**, processing **10-20M claims/year**

### The gap stated precisely

**Nobody is building a standalone AI decision engine for property and commercial claims adjusters that works on any CMS and doesn't require ripping out existing infrastructure.**

Not FNOL (crowded). Not estimation (Verisk's moat). Not auto casualty guidance (CCC's moat). The coverage → triage → investigation → reserve workflow for mid-market US buyers who use Xactimate for pricing but have nothing for deciding.

### The risk you need to name

Verisk has the data (every Xactimate estimate ever written) and the distribution (75-80% market share). If they decide to build a real decision engine inside Xactimate — not just photo labels, but actual coverage analysis and triage — they could own this overnight. Your window is how long it takes Verisk to move from features to platform. Crawford's Turvi/CoverAI is the early warning signal — if they start licensing it standalone, the gap is closing.

---

## 20. The Contrarian Bet Reframed — EU Motor

*The STP gap is the opportunity — but the threats are real*

### Who's competing in EU claims

**[Shift Technology](https://www.shift-technology.com/products/claims)** ($320M raised, 25+ countries) just launched "Shift Claims" in September 2025 — agentic AI for the full claims lifecycle. AXA Switzerland is an early adopter reporting [60% automation rate, 30% faster handling, >99% accuracy](https://www.shift-technology.com/resources/news/shift-technology-launches-shift-claims-to-power-claims-transformation-with-agentic-ai). **This is the most dangerous EU competitor.** They started in fraud detection but are now building the full adjuster workflow engine.

**[Solera/Audatex](https://www.solera.com/solutions/vehicle-claims/audatex/)** is the Verisk equivalent for EU motor. Founded in Germany, 1966. 4.5B+ vehicle damage images. Qapter AI does photo-to-estimate in seconds. They own motor damage estimation across Europe the way Xactimate owns US property. Huge data moat. If they build upstream from estimation to fault determination, they could own the full motor claims pipeline.

**[Tractable](https://tractable.ai/)** — London-based, computer vision for motor damage. Works with Aviva (UK), Admiral Seguros (Portugal/Spain). AI-generated repair estimates and triage in seconds. 70-75% of customers complete claims digitally.

**[Bdeo](https://bdeo.io/en/)** — Spanish startup, visual intelligence for motor AND property. Works with 7 of 10 top Spanish auto insurers (Zurich, Mutua Madrileña, Mapfre). Present in 20 countries. Similar to Tractable but stronger in Southern EU and expanding into property.

**[Sprout.ai](https://sprout.ai/)** — London-based. Has AXA, MetLife, AdvanceCare (Generali group). [3M+ claims processed, 96% accuracy, 70% STP](https://www.insurancetimes.co.uk/news/insurance-times-awards-2025-sproutai-claims-96-accuracy-in-claims-processing/1457041.article). But focused on **claims intake automation**, not adjuster decisions or convention matching.

**[Five Sigma/Clive](https://fivesigmalabs.com/clive/)** — 30% EU presence, adjuster copilot on any CMS. Landed Starr. Growing but early in EU.

**[ClaimSorted](https://www.claimsorted.com/)** — London-based AI-first TPA, €11.4M raised. UK + EU + US expansion.

**[Afori](https://www.eu-startups.com/2025/10/former-unicorn-team-to-launch-german-startup-afori-with-e4-million-to-bring-ai-powered-efficiency-to-insurance-brokers/)** — German, €4M, AI admin automation for insurance brokers. Not claims.

### What NONE of them are building

**1. Convention system automation.** This remains the single biggest confirmed gap across the entire competitive landscape. IRSA (France), CARD (Italy), CIDE/ASCIDE/CICOS (Spain), IDS (Portugal) — pre-computed fault lookup tables that COULD auto-resolve 60-70% of motor claims but actually only achieve ~10% STP. Nobody — not Shift, not Solera, not Tractable, not Bdeo — is building the pipeline from messy EAS data → structured fields → convention match → automated settlement. The convention lookup itself is trivial (a database query matching checkboxes to fault percentages). **The hard problem is upstream: turning a paper EAS with shaky handwriting and unclear checkboxes into structured, machine-readable data that can feed the convention tables.** That's an OCR + document understanding problem.

**2. The EAS-to-STP pipeline.** Solera/Audatex estimates the COST of motor damage. Tractable and Bdeo assess damage from PHOTOS. Shift automates the WORKFLOW. But none of them solve the FAULT DETERMINATION step for convention-eligible claims. In EU motor, fault determination IS the convention lookup — but only if the EAS data is clean. The bottleneck isn't the convention table, it's the data going in.

### The honest EU competitive map

| Layer | Motor | Who |
|-------|-------|-----|
| **Damage estimation** | Solera/Audatex (dominant) | Monopoly position |
| **Photo damage assessment** | Tractable, Bdeo, Solera Qapter | Competitive |
| **Claims intake/FNOL** | Sprout.ai, Shift | Competitive |
| **Fraud detection** | Shift Technology (dominant) | Well-funded |
| **Full claims workflow** | Shift Claims (new, Sept 2025) | Early but well-funded |
| **Convention matching/STP** | **NOBODY** | **Open** |
| **EAS data quality** | **NOBODY** | **Open** |
| **Adjuster copilot** | Five Sigma/Clive (30% EU) | Early |
| **Coverage decision support** | **NOBODY** | **Open** |

### The addressable market

- ~250-400 mid-market EU insurers (€100M-€500M GWP) — Germany (~80-120 regional mutuals), France (~60-80 mutuelles), plus Italy, Spain, Nordics, Benelux
- EU convention systems process ~30-40M motor claims/year across the big 5 markets
- The STP gap = 50+ percentage points of claims that COULD auto-resolve but don't
- Even moving STP from 10% to 30% would eliminate millions of adjuster-hours per year

### The gap stated precisely

**The real EU motor contrarian bet is not about the adjuster decision workflow (that's the US thesis). It's about the data quality layer that unlocks convention STP.**

In the US, convention systems don't exist — every claim needs human investigation. In EU, the system EXISTS and works beautifully... when it gets clean data. Nobody is fixing the data quality problem because:
- Solera/Audatex makes money from damage estimation, not fault resolution
- Tractable/Bdeo make money from photo assessment, not document processing
- Shift makes money from fraud detection and workflow automation, but starts downstream of the EAS
- The convention systems themselves are maintained by insurer associations, not tech companies

The opportunity: land with EAS digitization (OCR + document understanding) → convention matching → automated STP → then expand into adjuster copilot for non-convention claims.

### The risks you need to name

**Shift Technology risk:** They're well-funded ($320M), have AXA, and just launched full claims automation. If they decide to build EAS processing + convention matching as part of Shift Claims, they could close this gap. But right now they're focused on downstream workflow automation — they start AFTER the data is already in the system. The bet is that fixing what happens BEFORE the system (EAS capture → structured data → convention match) is a document AI problem, not a workflow automation problem, and Shift won't prioritize it.

**Solera risk:** They have 4.5B images and the motor estimation monopoly. If they build upstream from estimation to fault determination, they could own the full motor claims pipeline. But they're focused on damage COST, not liability FAULT. Different question, different data, different product.

**EU AI Act risk:** Insurance AI is classified as "high risk" under the EU AI Act, requiring transparency, human oversight, and documentation. This is a barrier to entry BUT also a moat if you build compliance-first — competitors that bolt on compliance as an afterthought will struggle in regulated EU markets.

---

## 21. The Contrarian Bet Reframed — Home/Property (Both EU and US)

*The third thesis — because home claims are structurally different from motor*

### Why home/property needs its own thesis

The EU motor thesis (Section 20) is about convention STP — a mechanism that doesn't exist for home claims. The US thesis (Section 19) leans toward property/commercial but doesn't fully separate it from motor dynamics. Home/property claims are structurally different from motor in BOTH markets:

| | **Motor** | **Home/Property** |
|---|---|---|
| Counterparty? | YES — another driver | Usually NO — you vs the peril |
| Agreed document? | EAS (EU) | NONE — anywhere |
| Core question | WHO caused it? | WAS it covered? |
| Convention/STP? | EU: Yes (10% actual) | NONE — anywhere |
| Adjuster needed? | EU: Often NO | Almost ALWAYS |
| EU structural advantage? | YES (EAS, conventions) | **NO — EU and US face the same problems** |

**This is critical: unlike motor, EU has zero structural advantage for home/property claims.** No EAS, no convention system, no pre-computed fault tables. A water damage claim in Munich is handled roughly the same way as one in Minneapolis — an adjuster (perito in EU) shows up, determines causation, checks coverage, estimates cost.

### What home/property adjusters actually do (the decision workflow)

Whether it's a US field adjuster or an EU perito, the workflow is:

1. **Coverage determination** — "Is this sudden and accidental water damage (covered) or a gradual leak from deferred maintenance (excluded)?" This is the HARDEST decision. It requires reading the policy, understanding exclusions, evaluating physical evidence, and often making judgment calls on causation timelines. No AI does this today.

2. **Triage** — Desk review (<$3K, simple causation, photo evidence sufficient) vs virtual inspection (medium complexity, video walkthrough) vs field inspection (hidden damage suspected, large loss, fraud indicators). Getting triage WRONG is expensive: sending a field adjuster when desk review sufficed wastes $500-1,000+; desk-reviewing a claim with hidden damage leads to supplement hell and litigation.

3. **Investigation scope** — What do I need to validate? Proof of ownership? Maintenance records? Contractor invoices? Prior claims history? Photos vs video vs moisture reading vs destructive testing? Every investigation decision costs time and money.

4. **Reserve setting** — What's the realistic exposure? Under-reserving triggers regulatory scrutiny. Over-reserving ties up capital. Requires estimating both the visible damage AND the probability of hidden damage, supplements, litigation.

5. **Causation analysis** — This is property-specific. "Was the roof damage from this week's storm (covered) or pre-existing deterioration (excluded)?" "Did the pipe burst suddenly (covered) or was it a slow leak over months (excluded)?" Causation determines coverage, and it's often ambiguous.

### The competitive landscape for property (both markets)

**US-specific players:**

- **Verisk/Xactimate + XactAI** — 75-80% of US property claims use Xactimate for estimation. XactAI (Sept 2025) adds photo labeling and transcription, bundled free with Pro licenses. But Xactimate estimates COST — it doesn't determine COVERAGE or CAUSATION. Verisk has the data moat and distribution to build a decision engine, but hasn't yet.
- **Crawford/Turvi CoverAI** — The closest to a property coverage decision tool. AI-driven policy coverage review that interprets complex policy language. But it's Crawford's proprietary product, not available standalone. Early signal to watch.
- **CAPE Analytics + EagleView** — Aerial/satellite imagery for pre-inspection risk assessment and damage detection. Pre-loss, not claims decision workflow.
- **Hover** — 3D property models from smartphone photos. Integrated with Xactimate for measurement. But measurement, not decisions.

**EU-specific players:**

- **Bdeo** — Spanish startup with visual intelligence for property insurance. Can identify cause of damage, assess severity, and recommend repair professional. Works with 7 of 10 top Spanish auto insurers, expanding into property. Active in 20 countries. **The most relevant EU property competitor.**
- **No Xactimate equivalent** — EU property estimation is fragmented. Different tools by country, many insurers use bespoke or legacy systems. There is no estimation monopoly to build on top of (or defend against).
- **Perito model** — In Southern EU (Spain, Portugal, Italy), peritos are mostly insurer employees or exclusive contractors, not independent adjusting firms. The buyer is the carrier's claims department directly, not a TPA.

**Both markets:**

- **Shift Technology** — Fraud detection → full claims workflow. Property claims are a target, but Shift starts with fraud signals and workflow automation, not coverage determination.
- **Five Sigma/Clive** — Adjuster copilot on any CMS. Works for property but not purpose-built for the coverage determination problem.
- **Encircle / BuildArray** — Field documentation tools. Capture data during inspections. Important for evidence gathering but not decision support.

### The honest competitive map for property

| Layer | US | EU | Gap? |
|-------|-----|-----|------|
| **Damage estimation** | Xactimate (monopoly) | Fragmented (no monopoly) | No |
| **Photo damage assessment** | Hover, CAPE, EagleView | Bdeo | Getting competitive |
| **Claims intake/FNOL** | Assured, Sprout.ai, Shift | Sprout.ai, Shift | Crowded |
| **Fraud detection** | Shift, carriers in-house | Shift | Shift dominates |
| **Field documentation** | Encircle, BuildArray | Limited | Some tools exist |
| **Coverage determination** | Crawford/Turvi CoverAI (proprietary) | **NOBODY** | **Open** |
| **Causation analysis** | **NOBODY** | **NOBODY** | **Wide open** |
| **Triage decision (desk/virtual/field)** | **NOBODY** (standalone) | **NOBODY** | **Open** |
| **Reserve recommendation** | Gradient AI (underwriting-focused) | **NOBODY** | **Mostly open** |
| **Adjuster copilot** | Five Sigma/Clive | Five Sigma/Clive (30% EU) | Early |

### The gap stated precisely

**The property claims decision workflow — coverage determination, causation analysis, triage, and reserve setting — is unaddressed by any standalone product in either market.** Crawford's CoverAI touches coverage review but is bundled inside their TPA stack. Everyone else does FNOL, fraud, estimation, or documentation — not the decisions between them.

The coverage question is genuinely harder than the fault question in motor:
- Motor fault in EU = convention lookup (deterministic, structured checkboxes → fault %)
- Property coverage = policy interpretation × causation analysis × physical evidence (probabilistic, requires judgment, varies by policy form)

**That's both the opportunity and the reason nobody's built it.** It's hard. The AI needs to read policy language (ISO forms, manuscript endorsements, exclusion schedules), match it against physical evidence (photos, moisture readings, inspection notes), assess causation timelines, and recommend a decision — all while being auditable and compliant.

### The addressable market (both markets combined)

**US property:**
- ~4.2M homeowner claims/year, ~10-15M commercial claims/year
- ~500-600 mid-market carriers + 50-100 TPAs + 53K adjusting firms
- Xactimate is the integration point (every estimate flows through it)

**EU property:**
- ~8-12M property claims/year
- ~250-400 mid-market carriers
- No estimation monopoly (more fragmented, harder integration story)
- Perito model means selling to carriers directly, not TPAs

**Combined: ~12-27M property claims/year across ~800+ buyers in both markets**

### How property differs from the US/EU motor theses

| | **US Motor** | **EU Motor** | **Property (Both)** |
|---|---|---|---|
| **Opportunity** | Adjuster decision copilot | Convention STP unlock | Coverage + causation AI |
| **Hard problem** | No convention → every claim needs human judgment | Paper EAS → bad data prevents STP | Causation ambiguity → requires policy × evidence analysis |
| **Data advantage** | None (fragmented) | EAS structure (if digitized) | Historical claim patterns (if captured) |
| **Estimation monopoly** | CCC (auto) | Solera/Audatex | Xactimate (US), fragmented (EU) |
| **Biggest competitor** | CCC/EvolutionIQ | Shift Technology | Crawford/Turvi CoverAI (proprietary) |
| **STP possible?** | Not really (no conventions) | Yes — 50+ point gap | Very limited (hidden damage, causation) |
| **Buyer** | Carriers + TPAs + MGAs | Carriers (mutuals heavy) | Carriers + TPAs (US), carriers (EU) |

### The risk

**For property, the biggest risk is that coverage determination may be too hard to automate reliably.** Unlike motor fault (structured checkboxes → deterministic lookup), property coverage requires interpreting policy language, assessing physical evidence, and making probabilistic causation judgments. Current AI is at ~70% accuracy for damage detection — you need >95% for coverage decisions that affect payouts. Getting this wrong means wrongful denials (lawsuits, regulatory action) or overpayment (leakage).

The mitigation: build for **recommendation, not automation**. The AI suggests a coverage determination with confidence score and supporting evidence. The adjuster decides. Human-in-the-loop. This is the "3x adjuster productivity" play, not the "replace the adjuster" play.

**The Verisk risk (US):** Same as Section 19. They have every Xactimate estimate ever written. If they build coverage analysis on top of that data, they own US property.

**The fragmentation risk (EU):** No estimation monopoly means no natural integration point. You'd need to integrate with multiple legacy systems per country. The EAS-to-STP pipeline (Section 20) is a cleaner EU wedge because it has a standardized input document.

---

## 22. How the Three Theses Fit Together — Sequencing and Strategy

### The three distinct opportunities

| # | Thesis | Market | Core problem | Wedge product |
|---|--------|--------|-------------|---------------|
| 1 | **Convention STP** | EU motor | Paper EAS → bad data → 10% STP vs 60-70% theoretical | EAS digitization + convention matching |
| 2 | **Adjuster decision copilot** | US (all lines except auto casualty) | No software between FNOL and estimate for coverage/triage/reserve | AI decision layer on any CMS |
| 3 | **Coverage + causation AI** | EU + US property | Coverage determination requires policy × evidence × causation | Coverage recommendation engine |

### Why these are complementary, not competing

**Thesis 1 (EU motor STP) feeds Thesis 3 (property coverage AI):**
- EAS digitization builds OCR + document understanding muscle
- Convention matching builds structured decision logic
- These capabilities transfer to property: policy document parsing, coverage clause matching, structured decision trees
- Land in EU motor (cleaner problem, standardized input, measurable STP improvement), expand to property

**Thesis 2 (US adjuster copilot) is the same product as Thesis 3 (property coverage AI) with different packaging:**
- The US buyer wants a "copilot" because they have no convention system — every claim needs human judgment
- The product underneath is the same: coverage analysis, triage recommendation, reserve suggestion, investigation scoping
- In US, you sell it as "makes your adjusters 3x more productive"
- In EU property, you sell it the same way (no convention advantage for property)

### Possible sequencing

**Option A: EU motor first (land), then US + EU property (expand)**
- Land with EAS → convention STP (measurable, provable, clear ROI)
- Build OCR + document AI + decision logic capabilities
- Expand to property coverage AI in both markets
- Expand to US auto (harder — CCC's territory)

**Option B: US property first (land), then EU (expand)**
- Land with adjuster decision copilot for US mid-market carriers
- Larger immediate market (~500-600 carriers vs ~250-400 EU)
- But less differentiated (Five Sigma, Crawford/Turvi exist)
- Expand to EU property (same product, different buyer)
- Add EU motor convention matching as a differentiated feature

**Option C: Both simultaneously (hardest, fastest if you can execute)**
- EU motor STP for co-founder's network (Portugal/Southern EU)
- US property copilot for US market
- Converge into a single platform that handles motor (with convention intelligence) and property (with coverage AI) across both markets
- This is the "nobody does US + EU in one product" differentiator
- But requires 2x the engineering and go-to-market effort

### The honest question

Can one startup build all three? Or do you pick one and sequence?

The convention STP problem (Thesis 1) is the **most defensible** — it requires deep country-by-country convention knowledge that takes years to build. The adjuster copilot (Thesis 2) is the **biggest market** — US mid-market carriers + TPAs + MGAs. The coverage AI (Thesis 3) is the **hardest** — requires AI that can reliably interpret policy language against physical evidence.

The sequencing answer probably depends on which co-founders you have and which market you can land your first 5-10 customers in fastest.

### Sources for Sections 19-22

- [Verisk XactAI Launch](https://www.verisk.com/resources/campaigns/empowering-the-human-side-of-insurance/)
- [Verisk AI Tools Announcement Sept 2025](https://www.verisk.com/company/newsroom/verisk-introduces-new-ai-tools-to-streamline-the-property-claims-experience/)
- [Five Sigma / Starr Partnership Jan 2026](https://www.prnewswire.com/news-releases/starr-modernizes-pc-and-specialty-claims-with-five-sigmas-ai-claims-platform-and-clive-302669986.html)
- [CCC EvolutionIQ Q1 2025](https://www.investing.com/news/company-news/ccc-intelligent-solutions-q1-2025-slides-aidriven-growth-and-evolutioniq-acquisition-93CH-4106995)
- [EvolutionIQ Joins CCC](https://www.evolutioniq.com/resources/evolutioniq-joins-ccc-intelligent-solutions)
- [Shift Technology Launches Shift Claims Sept 2025](https://www.shift-technology.com/resources/news/shift-technology-launches-shift-claims-to-power-claims-transformation-with-agentic-ai)
- [Shift Technology — Microsoft Customer Story](https://www.microsoft.com/en/customers/story/23202-shift-technology-azure-ai-vision)
- [Solera/Audatex Vehicle Claims](https://www.solera.com/solutions/vehicle-claims/audatex/)
- [Solera Qapter AI](https://www.solera.com/solutions/vehicle-claims/)
- [Tractable AI](https://tractable.ai/)
- [Bdeo Visual Intelligence](https://bdeo.io/en/)
- [Bdeo — 7 of 10 Spanish Auto Insurers](https://www.santaluciaimpulsa.es/en/blog/bdeo-la-revolucion-de-la-inteligencia-visual-en-los-seguros)
- [Sprout.ai — MetLife Partnership](https://www.businesswire.com/news/home/20250624877897/en/)
- [Sprout.ai — 96% Accuracy / 3M+ Claims](https://www.insurancetimes.co.uk/news/insurance-times-awards-2025-sproutai-claims-96-accuracy-in-claims-processing/1457041.article)
- [ClaimSorted Raises €11.4M](https://www.vestbee.com/insights/articles/claim-sorted-raises-11-4-m)
- [Afori — €4M German Broker AI](https://www.eu-startups.com/2025/10/former-unicorn-team-to-launch-german-startup-afori-with-e4-million-to-bring-ai-powered-efficiency-to-insurance-brokers/)
- [Crawford Turvi Launch](https://www.crawco.com/blog/turvi-launches-elevating-the-insurtech-sector-with-advanced-saas-technology)

---

### Sources for Section 18

- [NAIC 2024 Market Share Data](https://content.naic.org/article/naic-releases-2024-market-share-data)
- [S&P Global: US P&C Insurers Exceed $1 Trillion](https://www.spglobal.com/market-intelligence/en/news-insights/articles/2025/3/in-industry-first-us-pc-insurers-exceed-1-trillion-in-direct-annual-premiums-88062276)
- [IBISWorld: P&C Insurance Businesses](https://www.ibisworld.com/united-states/number-of-businesses/property-casualty-direct-insurance/1325/)
- [IBISWorld: Insurance Brokers & Agencies](https://www.ibisworld.com/united-states/market-size/insurance-brokers-agencies/1331/)
- [Demotech: Super Regional P&C Insurers](https://www.demotech.com/demotech_news/independent-regional-and-specialty-insurers-have-addressed-availability-and-affordability-for-centuries-including-residential-property-insurance/)
- [BLS: Claims Adjusters](https://www.bls.gov/ooh/business-and-financial/claims-adjusters-appraisers-examiners-and-investigators.htm)
- [III Facts + Statistics: Auto Insurance](https://www.iii.org/fact-statistic/facts-statistics-auto-insurance)
- [III Facts + Statistics: Homeowners Insurance](https://www.iii.org/fact-statistic/facts-statistics-homeowners-and-renters-insurance)
- [III Facts + Statistics: Industry Overview](https://www.iii.org/fact-statistic/facts-statistics-industry-overview)
- [Precedence Research: Insurance TPA Market](https://www.precedenceresearch.com/insurance-third-party-administration-market)
- [Conning: US MGA Premiums 2024](https://www.prnewswire.com/news-releases/conning-us-mga-premiums-climb-16-to-114-billion-in-2024-302502760.html)
- [Vertafore: State of Independent Agencies 2024](https://www.vertafore.com/resources/ebooks-whitepapers/state-independent-insurance-agencies-2024)
- [EIOPA Insurance Statistics](https://www.eiopa.europa.eu/tools-and-data/insurance-statistics_en)
- [Insurance Europe Statistics](https://www.insuranceeurope.eu/statistics)
- [BIPAR: Insurance Intermediaries June 2025](https://www.bipar.eu/images/uploads/general/BIPAR_report-Figures_on_insurance_intermediaries-Update-June_2025.pdf)
- [Mordor Intelligence: Europe Insurance Brokerage](https://www.mordorintelligence.com/industry-reports/europe-insurance-brokerage-market)
- [MarshBerry: Insurance Brokerage in Europe](https://www.marshberry.com/eu/blog/one-continent-with-little-uniformity-insurance-brokerage-in-europe/)
- [NextMSC: Europe Insurance TPA Market](https://www.nextmsc.com/report/europe-insurance-tpa-market)
- [Howden Re: European MGA Market](https://www.reinsurancene.ws/european-mga-market-growth-is-outpacing-us-and-global-benchmarks-howden-re/)
- [Insuramore: Global MGA/MGU Sector 2024](https://www.reinsurancene.ws/global-mga-mgu-sector-surges-to-29-25bn-in-2024-insuramore-reports/)
- [Cognitive Market Research: EU Claims Management](https://www.cognitivemarketresearch.com/regional-analysis/europe-insurance-claims-management-market-report)
- [Sedgwick Enterprise Valuation](https://www.businessinsurance.com/private-equity-investment-values-sedgwick-at-13-2-billion/)
- [Crawford 2024 Results](https://ir.crawco.com/news/news-details/2025/Crawford--Company-Reports-2024-Fourth-Quarter-and-Full-Year-Results/default.aspx)
- [Ardonagh 2024 Results](https://www.ardonagh.com/announcements/2025/the-ardonagh-group-full-year-2024-financial-results/)
- [Howden 2024 Results](https://www.howdengroupholdings.com/news/howden-announces-2024-full-year-results)
- [PIB Group 2024 Results](https://www.pibgroup.co.uk/news/pib-group-surpasses-500m-revenue-milestone-in-2024)
- [Chambers: Portugal Insurance 2025](https://practiceguides.chambers.com/practice-guides/insurance-reinsurance-2025/portugal/trends-and-developments)
- [Alacrity Solutions Restructuring](https://www.transacted.io/blackrock-loses-560m-equity-in-alacrity-debt-restructuring)
- [Talli.ai: Claims Payout Statistics](https://blog.talli.ai/insurance-claims-payout-statistics/)
- [Ryan Specialty Q4 2024 Results](https://ir.ryanspecialty.com/ir-news-events/press-releases/detail/97/ryan-specialty-reports-fourth-quarter-2024-results)
- [GDV: Insurance Premiums 2023](https://www.gdv.de/gdv-en/media/insurance-premiums-up-slightly-in-2023-cautious-optimism-for-2024--165840)

---

## Sources

### TPAs
- [Sedgwick Technology](https://www.sedgwick.com/technology/)
- [Sedgwick Sidekick Agent Launch](https://www.prnewswire.com/news-releases/sedgwick-optimizes-claim-workflows-with-ai-application-sidekick-and-microsoft-integration-302440773.html)
- [Sedgwick Digital Adjust Pro](https://www.prnewswire.com/news-releases/sedgwick-unveils-a-comprehensive-claims-processing-solution-302447063.html)
- [Sedgwick Lightning App](https://www.sedgwick.com/press-release/sedgwicks-lightning-app-transforms-property-claims-inspections/)
- [Sedgwick Glassdoor](https://www.glassdoor.com/Reviews/Sedgwick-Reviews-E31568.htm)
- [Crawford Innovation](https://www.crawco.com/innovation)
- [Turvi Launch](https://www.crawco.com/blog/turvi-launches-elevating-the-insurtech-sector-with-advanced-saas-technology)
- [Crawford edjuster Acquisition](https://www.edjuster.com/news/crawford-acquires-edjuster-contents-valuation-service-and-platform/)
- [Davies Agentic AI](https://davies-group.com/knowledge/davies-unveils-new-agentic-ai-features-in-its-claimpilot-product-suite-as-it-doubles-down-on-technology-investment/)
- [Davies Vision 2030](https://davies-group.com/knowledge/davies-appoints-matt-button-as-deputy-group-ceo-as-firm-invests-for-the-future-and-unveils-its-vision-2030-strategy/)
- [ClaimPilot Features](https://claimpilot.com/features/)

### Market Data
- [Precedence Research — TPA Market](https://www.precedenceresearch.com/insurance-third-party-administration-market)
- [McKinsey Insurance Productivity 2030](https://www.mckinsey.com/industries/financial-services/our-insights/insurance-productivity-2030-reimagining-the-insurer-for-the-future)
- [EY Claims Leakage](https://www.ey.com/en_us/insights/insurance/claims-litigation)
- [Risk & Insurance — Property Claims 2025](https://riskandinsurance.com/property-claims-management-faces-major-disruptions-in-2025/)
- [Deloitte Insurance M&A 2025](https://www.deloitte.com/us/en/Industries/financial-services/articles/insurance-m-and-a-outlook.html)
- [Adjuster Salary — ZipRecruiter](https://www.ziprecruiter.com/Salaries/Property-Claims-Adjuster-Salary)

### Technology Players
- [Hover / Verisk Partnership](https://www.verisk.com/company/newsroom/hover-expands-offerings-within-verisks-xactimate-to-advance-property-claims-efficiency/)
- [Xactimate Market Share](https://uphelp.org/claim-guidance-publications/xactimate-demystified/)
- [CAPE Analytics Hail Intelligence](https://capeanalytics.com/hail-intelligence/)
- [EagleView Insurance](https://www.eagleview.com/industry/insurance/)
- [Cotality Claims Products](https://www.cotality.com/products/claims-scope)
- [Symbility vs Xactimate](https://estimate-experts.com/symbility-vs-xactimate/)
- [VCA Software](https://vcasoftware.com/tpa-claims-management-software/)
- [n2uitive AI SummaryAssist](https://www.businesswire.com/news/home/20250415387161/en/)
- [Encircle](https://www.getencircle.com/)
- [BuildArray](https://www.buildarray.com/)

### Startups
- [Assured](https://www.assured.com/)
- [Five Sigma / Clive](https://fivesigmalabs.com/clive/)
- [FurtherAI](https://www.furtherai.com/)
- [Avallon](https://www.businesswire.com/news/home/20251106838494/en/)
- [Agentech](https://www.agentech.com/)
- [Elysian](https://elysian.is/)
- [Reserv](https://insurtechdigital.com/articles/digital-native-tpa-reserv-raises-another-20m-in-funding)
- [Gradient AI](https://www.gradientai.com/)

### Market Sizing & EU Data (Sections 12-13)
- [EIOPA Insurance Statistics](https://www.eiopa.europa.eu/tools-and-data/insurance-statistics_en)
- [EIOPA Register of Insurance Undertakings](https://register.eiopa.europa.eu/registers/register-of-insurance-undertakings)
- [Insurance Europe Statistics](https://www.insuranceeurope.eu/statistics)
- [Insurance Europe — European Motor Insurance Markets](https://www.insuranceeurope.eu/publications/465/european-motor-insurance-markets/)
- [EU Claims Management Market — Cognitive Market Research](https://www.cognitivemarketresearch.com/regional-analysis/europe-insurance-claims-management-market-report)
- [Europe Insurance TPA Market — NextMSC](https://www.nextmsc.com/report/europe-insurance-tpa-market)
- [Portugal Non-Life Market — Axco](https://www.axcoinfo.com/market-place/report-store/non-life-reports/portugal-non-life-insurance-market-report/)
- [Portugal — Lloyd's Market Profile](https://www.lloyds.com/portugal)
- [Fortune Business Insights — Claims Management Market](https://www.fortunebusinessinsights.com/claims-management-market-110629)
- [Italy Average Motor Claim Cost — Statista](https://www.statista.com/statistics/1105141/average-claim-cost-for-passenger-car-insurance-in-italy/)
- [Motor Claims Paid in Europe — Statista](https://www.statista.com/statistics/437562/vehicle-insurance-claims-value-europe/)
- [Insurance Technology Spend: CIOs 3.7% to 5% of Premium — SimpleSolve](https://www.simplesolve.com/blog/why-cios-say-they-will-spend-3.7-of-premium-on-tech-in-2021)
- [McKinsey — Can European Insurtechs Live Up to the Hype?](https://www.mckinsey.com/industries/financial-services/our-insights/insurance-blog/can-european-insurtechs-live-up-to-the-hype)

### US Adjuster Workforce (Section 14)
- [Carrier Management — Claims Adjuster Among Fastest Declining Professions](https://www.carriermanagement.com/features/2025/01/22/270842.htm)
- [Claims Journal — What's Happening in The Claims Profession](https://www.claimsjournal.com/news/national/2025/10/29/333765.htm)
- [Property Insurance Coverage Law Blog — Challenges Facing Independent CAT Adjusters](https://www.propertyinsurancecoveragelaw.com/blog/challenges-facing-independent-catastrophe-adjusters/)
- [WeGoLook — Crawford On-Demand Inspections](https://www.wegolook.com/)
- [Crawford — Meeting the Growing Demand for On-Demand](https://www.crawco.com/blog/meeting-the-growing-demand-for-on-demand)
- [AdjusterPro — IA Firm Directory](https://adjusterpro.com/independent-adjusting-firm-directory/)
- [360training — Insurance Adjuster Licensing](https://www.360training.com/insurance-education/insurance-adjuster)
- [Kaplan — How to Become an Insurance Claims Adjuster](https://www.kaplanfinancial.com/resources/getting-started/how-to-become-an-insurance-claims-adjuster)
- [IA Path — Insurance Adjuster License Requirements by State](https://iapath.com/what-adjuster-license-should-i-get/)
- [Caravela Seguros — 2023 Annual Report (EN)](https://caravelaseguros.pt/wp-content/uploads/2025/01/20240412-RC-2023_vfinal_EN.pdf)
- [Yahoo Finance — Toscafund Weighs Sale of Caravela](https://finance.yahoo.com/news/toscafund-weighs-sale-portuguese-insurer-142112946.html)

---

## 23. Co-Founder Strategy Call — Transcript Analysis

*Analysis of strategy call between Jeremy and co-founder, February 2026. Full transcript available via Granola.*

### Key Decisions Made

1. **Health insurance is OUT** — Co-founder: "I will never do health. I think it's too complex." Both agreed health is too structured (ICD-10 codes, pre-authorization workflows) and already has automation from the provider side.

2. **US-first build, EU if it works** — Co-founder: "I think we should focus on US. Building a product for The US. And if it works for Europe, perfect. But if it doesn't work, let's ignore it." Jeremy pushed back with EU motor STP gap research. Resolution: EU motor is the WEDGE (design partner Caravela, convention system moat), US property is the COMPANY.

3. **Not a TPA, not making decisions** — Co-founder: "We are not a TPA. We are not a TPA. So if I'm pitching... we are not a TPA because we are not making the decisions." Human-in-the-loop is mandatory.

4. **Cars alone in Europe won't build a company** — Co-founder: "Cars in Europe, you don't need it... But it's very, very small. If you build the product for that, you don't have a company." Motor is the wedge, not the destination.

5. **Focus on P&C (property and casualty)** — Co-founder: "property and casualty, it makes a lot of sense. I would say that I would go with that one."

6. **Caravela as design partner** — Jeremy: "I want an LOI, and we say we're doing it in free beta tester. For six months." Co-founder agreed but wants to close the existing OCR contract first. Weekly syncs needed.

7. **Demo needs to be built block by block** — Co-founder: "I tried to build two demos today, and they basically... I think we need to build block by block." Both agreed: don't try to show everything at once.

### Product Positioning — What Was Confirmed

**The product is a decision engine for claims adjusters.** Not a CRM, not intake automation, not estimation.

Co-founder's clearest articulation: "I'm here to support the adjuster. To spend less amount of time on everything that doesn't require work. And when they get to the decision, I will help them with all the data that we have been collecting, and I will learn with him."

**The 6 decision sub-steps** (co-founder's framework):
1. Coverage verification
2. Policy report checking
3. Repair assessment
4. Cost analysis
5. Reserve calculation
6. Fraud detection

**SOP-driven workflows** are the core differentiator: "everything that we build needs to be really around SOP, like, what is the SOP that your insurance company or your TPA follows."

**Historical data engine** is the long-term moat: "When we come in and we use the historical data, the out-of-the-box thing, we get 60%. As soon as we start getting better data and training the models, we go to 70 or 80%."

### Features Discussed in Detail

| Feature | Source | Priority |
|---------|--------|----------|
| SOP upload → workflow generation | Co-founder | Core (Day 1) |
| Playbooks per claim type | Co-founder (citing Five Sigma: "That's very smart. Let's replicate that.") | Core |
| Email/document parsing | Co-founder | Core (prerequisite) |
| Convention matching (EU motor) | Research + co-founder | Wedge product |
| Call recording + guidance | Co-founder: "We are recording the calls... guiding you through those calls" | Phase 2 |
| Document generation per SOP | Co-founder: "we are generating all the documents for you" | Core |
| Reserve recommendation | Co-founder: "How much money you are reserving" — P&L impact framing | Core |
| Fraud signal detection | Co-founder: listed as 6th decision sub-step | Phase 2 |
| Historical data engine | Both: "the real product is based on historical data" | Long-term moat |
| Triage/complexity scoring | Co-founder: "auto triage: I have 20-30%" | Core |

### Market Sizing Discussed

Jeremy shared research numbers during the call:
- US: ~4,000 carrier entities, 2,000 in Europe
- Mid-to-small market: 600-500 in each market
- Pricing: €50K/year (smallest) to €1M+ (largest)
- ~1,000 addressable players, average €200K/year = €200M TAM

Co-founder's insight on mid-market: "I always think about insurance companies as companies that have a data science team. But I think you are right." — The mid-to-small carriers don't have tech teams and desperately need this.

### Competitive Positioning from the Call

**Five Sigma** — Co-founder: "I also care a lot about them. For me, they are still my main competitor." Jeremy: "But I think they're everywhere and nowhere at the same time."

**Assured** — Co-founder analyzed them directly: "they are focusing a lot on the initial stage." Acknowledged they're a $1B company but "that's already too big for me to think about."

**FurtherAI** — Co-founder: "they are trying to do everything... they don't focus on improving [decisions]."

**ClaimSorted** — Co-founder: "claims sorted doesn't know how to do marketing. I think their positioning is the worst."

**Avallon** — Co-founder: "they are just calling the repair guy. But that's the same for everyone."

### Critical Insight — Reserve Impact on P&L

The co-founder surfaced a selling point not prominent in our research: reserves hit the P&L immediately.

"Do you know this concept? It's not what they are paying that matters. It's how much money they are reserving. Because reserves are already recognized in the P&L right away."

This means Mysa's reserve recommendation engine has a CFO-level selling point, not just a claims VP selling point. Inaccurate reserves directly impact reported profitability.

Real example cited: Caravela lost €18M in a year because of heavy December rains and poor policy pricing — demonstrating how claims/reserve accuracy directly impacts small carrier survival.

### Blind Spots Identified

**What was NOT discussed in the call that our research flagged as important:**

1. **Verisk/XactAI** — Not mentioned by name. The co-founder said "How can we integrate with them?" about Xactimate but didn't discuss XactAI's free bundling strategy or data moat risk.

2. **Shift Technology** — Not mentioned despite being the most dangerous EU competitor. $320M raised, Shift Claims launched Sept 2025, AXA Switzerland 60% automation rate.

3. **GDPR/AI Act compliance** — Co-founder mentioned GDPR for call recording but didn't discuss AI Act high-risk classification, conformity assessments, or human oversight requirements for automated decisions.

4. **CCC/EvolutionIQ** — Mentioned briefly ("CCC is very very small" in reference to property) but the $730M EvolutionIQ acquisition and its implications for auto casualty were not discussed.

5. **Solera/Audatex** — Not discussed despite being the EU motor estimation monopoly with 4.5B+ images and Qapter AI photo-to-estimate capability.

6. **On-prem vs cloud** — Jeremy asked "Are we on-prem model for decision makers?" — this was left unresolved in the call. Agent research confirms: NOT a differentiator, 85% cloud adoption in P&C.

### Action Items from the Call

1. **Build demo block by block** — Co-founder: "Let's build the demo tomorrow. We have something to show."
2. **Get Caravela LOI** — Jeremy: "I want an LOI, free beta tester for six months."
3. **Weekly syncs with Caravela** — Jeremy: "We need to meet weekly."
4. **Pitch to Sapphire** — Co-founder: "I think we should sell this to Sapphire next week."
5. **Share research docs** — Jeremy to share README and research documents
6. **Size the EU market properly** — Both agreed more granular country-level sizing needed
7. **Define the demo scenarios** — What to show, in what order, block by block

### Contradictions vs Research

| Topic | Transcript Assumption | Research Finding | Resolution |
|-------|----------------------|-----------------|------------|
| EU motor market size | "Too small for a company" | €400-450B GWP, 55-70M claims/year | EU motor is the WEDGE, not the company. Property + US is the company. |
| TPAs in Europe | "There is only one TPA that is important" (25% market) | TPAs are minimal in EU — carriers handle claims internally | Correct — EU sell to carriers directly, not TPAs |
| CCC market share | "CCC is very very small" (about property) | CCC is 60%+ in US auto, acquired EvolutionIQ for $730M | Co-founder was right about CCC being small in property. CCC is huge in auto but not property. |
| Intake competition | "I don't care about intake" | Assured ($1B), FurtherAI ($30M), Avallon ($4.6M) all doing intake | Correct positioning — don't compete on intake, compete on decisions |
| Historical data availability | "No one ever tracked how the decisions were being made" | Adjusters generate documents, emails, call records for every decision | Data exists but is unstructured — exactly what Mysa's document AI can parse |
| Five Sigma as competitor | "They are still my main competitor" | Five Sigma is CMS + copilot, not a decision engine. $10.1M revenue. | Correct to watch but different layer — Five Sigma is broader, Mysa is deeper |
