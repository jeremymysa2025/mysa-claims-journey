# Mysa Founding Operating System (FOS) v1.0

**Date:** February 9, 2026
**Authors:** Jeremy Blehaut & Tiago Brigido
**Status:** DRAFT v1.0 — All 11 modules complete, pending founder review

---

# Part 0: Executive Summary

# Mysa — Executive Summary

**Founding Operating System | February 2026**

---

## Company

Mysa is building the **Claims Decision Engine** — a new category of AI software that sits in the gap between intake (where data arrives) and settlement (where money moves), guiding the expert judgment that determines what gets paid and why. Insurance technology has spent billions automating the front door of claims — document parsing, chatbots, fraud scoring — while leaving the actual decision-making to adjusters juggling 5-7 disconnected systems, 40-page policy PDFs, and institutional knowledge locked in their heads. Mysa is the first product built specifically to occupy the decision layer: coverage verification, liability assessment, reserve calculation, fraud flagging, and settlement recommendation — powered by carrier-specific SOPs, not generic AI. [MODULE: 1]

---

## The Problem

**The workforce is collapsing.** 25% of claims adjusters will retire within five years. The profession is the 12th fastest-declining in the US. Annual attrition runs 20% at carriers and 33% at TPAs. Each departing adjuster takes approximately six years of institutional knowledge with them. Carriers cannot hire or train fast enough to replace what they are losing. [MODULE: 1, 2]

**The decision layer is untouched.** A typical motor claim takes 2-4 hours of adjuster time. 60-70% of that time is spent getting to the decision — pulling data from disconnected systems, cross-referencing policy documents, re-keying information between platforms. The adjuster is the integration layer: a human API receiving inputs from multiple systems, processing them through memorized rules, and outputting decisions under time pressure. The result is 125 open claims per adjuster, 20+ phone calls per day, and growing backlogs of long-lasting open cases. The fully loaded cost per adjuster is approximately $110K/year, producing a cost per closed claim of $230-$370. [MODULE: 2]

**Straight-through processing is a myth for most claims.** Convention systems (standardized inter-insurer protocols for settling motor claims in the EU) handle the simplest cases automatically, but the moment a claim involves ambiguity — contested liability, policy exclusions, complex damages — an adjuster must make a judgment call with no structured support. Every existing tool (CMS, estimation software, fraud detection) addresses a piece of the workflow. None addresses the decision itself. [MODULE: 1, 2]

---

## The Solution

Mysa replaces the adjuster's fragmented, manual decision process with an AI-guided workflow that covers six expert judgment steps: coverage verification, document validation, repair assessment, cost analysis, reserve calculation, and fraud/anomaly detection. Each step that currently takes 10-30 minutes of manual work is reduced to 1-3 minutes of human review. Total decision time drops from 65-120 minutes to 10-15 minutes per claim. The adjuster always decides — Mysa recommends. [MODULE: 1, 10]

The architecture is **agent-native, not AI-bolted-on.** Business rules live as knowledge (carrier SOPs, convention system rules, enforcement patterns), not hardcoded logic. Adding a new insurer is a knowledge ingestion task (hours to days), not a development sprint (weeks). A Chrome extension overlay — designed to work alongside existing systems rather than replace them — meets adjusters where they already work. This eliminates the migration risk that kills enterprise software sales. Features are prompts, not code. [MODULE: 7]

The critical differentiator is **SOP encoding.** Mysa ingests each carrier's Standard Operating Procedures — authority levels, escalation paths, reserve rules, documentation requirements — and encodes them into the decision workflow. Different adjusters at the same carrier make the same decision on the same claim. New hires follow the same SOP-driven process as ten-year veterans from day one. This solves the consistency problem that keeps every VP of Claims awake at night. [MODULE: 1, 7]

---

## Market

The global motor and property claims market processes an estimated 80-95 million claims per year across the EU and US, backed by approximately $1.5 trillion in combined premiums. Mysa's primary target is the "Caravela tier" — mid-market carriers with EUR 100-200M in gross written premiums. These carriers are large enough to have real claims volume (30-60K claims/year) but too small to build AI in-house. They have no data science teams. They cannot compete with Tier 1 carriers for engineering talent. They need a product, not a platform to build on. [MODULE: 4]

The bottom-up math: 80-95% of carriers that write motor also write property. A Caravela-sized carrier generates EUR 100-200K/year in Mysa revenue. Property adds 60-70% revenue per carrier at zero new customer acquisition cost. The buyer (VP Claims / Chief Claims Officer) is the same persona across every market. [MODULE: 4, 9, 10]

---

## Competitive Advantage

**The decision layer has zero direct competition.** Over $1 billion in combined funding has been deployed into intake automation (Assured, FurtherAI, Avallon, Sprout.ai). $320M+ into fraud detection (Shift Technology). $35B+ in market cap sits in estimation tools (Verisk/Xactimate, CCC, Solera/Audatex). Every one of these categories addresses a piece of the claims workflow. None of them addresses the decision itself. Mysa does not compete with these companies — it sits between them, using their outputs as inputs to the judgment layer they have all avoided. [MODULE: 5]

**The data moat is decision reasoning.** CCC and Verisk own claim outcomes — what was paid. Anthropic, OpenAI, and Google own general AI capability. Carriers own their own historical data but cannot extract or learn from it. Nobody owns structured decision reasoning: why the adjuster decided, which SOP steps were followed, what comparable claims were considered, when the AI recommendation was overridden and why. This data category cannot be purchased, scraped, or inferred from historical records. It can only be captured at the moment of decision, inside a tool designed to capture it. Every claim processed through Mysa generates decision ground truth that makes the system more accurate — a flywheel that compounds over time. [MODULE: 8]

---

## Go-to-Market

Mysa follows a five-phase geographic expansion where each phase creates the precondition for the next. **Phase 1: Portugal** — smallest Southern EU market (25-30 motor writers), cleanest convention system (IDS/CIMPAS, 91% agreement rate), co-founder network, and Caravela as a live design partner (EUR 188M GWP, 57K claims/year). **Phase 2: Southern EU** — convention expertise transfers directly to Spain (CIDE), France (IRSA), and Italy (CARD); same architecture, different knowledge module. **Phase 3: Property upsell** — same carriers, same buyer, 80% workflow overlap, +60-70% revenue per account. **Phase 4: Northern/Central EU** — proven playbook on larger markets. **Phase 5: US entry** — largest TAM ($532B in combined auto + homeowners premiums), leveraging a proven product. [MODULE: 9]

---

## Business Model

Dual pricing: per-claim (EUR 2-8/claim depending on carrier size) or annual platform license (EUR 10K-2M/year depending on tier). At a Caravela-sized carrier, a EUR 100K/year platform license equals 0.05% of GWP — trivial relative to potential savings of EUR 562-750K/year from STP improvement alone. Most carriers start per-claim (low barrier, pay-as-you-go) and migrate to platform pricing as they scale. [MODULE: 10]

---

## The Team

*[PLACEHOLDER: Founder bios to be added]*

---

## The Ask

*[PLACEHOLDER: Fundraising details to be added]*

---

*Sources: All figures cited are traceable to FOS Modules 1, 2, 4, 5, 7, 8, 9, and 10. See individual modules for primary source documentation.*

---

# Part 0.5: Table of Contents, Cross-References & Glossary

# Mysa Founding Operating System — Table of Contents

**Version:** 1.0
**Date:** February 9, 2026
**Status:** Living Document

---

## Document Map

The FOS is structured as 11 interconnected modules. Each module feeds one or more external outputs:

```
                          FOUNDING OPERATING SYSTEM
                          ========================

   MODULE 1                MODULE 2              MODULE 3
   Positioning             Problem               Claims Journey
   (Identity, ICP,         (Workflow audit,       (Full lifecycle,
    value prop)             workforce crisis)      decision forks)
       |                       |                       |
       +-------+-------+-------+-------+-------+------+
               |               |               |
           MODULE 4        MODULE 5        MODULE 6
           Market          Competition     Product & Demo
           (TAM, segments, (Landscape,     (Specs, flows,
            country data)   moat)           demo scripts)
               |               |               |
       +-------+-------+-------+-------+------+
               |               |               |
           MODULE 7        MODULE 8        MODULE 9
           Technical       Data &          Go-to-Market
           (Architecture,  Flywheel        (Rollout phases,
            compliance)    (Moat, legal)    pricing, channel)
               |               |               |
       +-------+-------+-------+-------+------+
               |                               |
           MODULE 10                      MODULE 11
           Business Model                 Risk & Regulatory
           (Unit economics,               (Competitive, legal,
            fundraising)                   operational)
               |                               |
       +-------+-------+-------+-------+------+
               |               |               |
          PITCH DECK      MARKETING        SALES &
          & DATA ROOM     SITE COPY        DEMO SCRIPTS

   +-----------+-----------+-----------+-----------+
   |           |           |           |           |
   PITCH     MARKETING   DEMO        SALES       DATA
   DECK      SITE        SCRIPTS     COLLATERAL  ROOM
   +-----------+-----------+-----------+-----------+
   | Mod 1     | Mod 1     | Mod 3     | Mod 2     | Mod 4   |
   | Mod 2     | Mod 2     | Mod 6     | Mod 3     | Mod 7   |
   | Mod 4     | Mod 7     | Mod 7     | Mod 5     | Mod 8   |
   | Mod 5     | Mod 9     |           | Mod 9     | Mod 10  |
   | Mod 10    |           |           | Mod 10    | Mod 11  |
   +-----------+-----------+-----------+-----------+---------+
```

**Which modules to read for which purpose:**

| Output | Primary Modules | Supporting Modules |
|--------|----------------|-------------------|
| **Pitch Deck** | 1 (Positioning), 2 (Problem), 4 (Market), 10 (Business) | 5 (Competition), 7 (Technical), 8 (Data Moat) |
| **Marketing Site** | 1 (Positioning), 2 (Problem), 7 (Technical) | 9 (GTM) |
| **Demo Scripts** | 3 (Claims Journey), 6 (Product & Demo) | 7 (Technical) |
| **Sales Calls** | 2 (Problem), 3 (Claims Journey), 5 (Competition), 9 (GTM) | 10 (Business) |
| **Data Room / Due Diligence** | 4 (Market), 7 (Technical), 8 (Data), 10 (Business), 11 (Risk) | All others |
| **Technical Partnership** | 7 (Technical), 8 (Data) | 6 (Product) |

---

## Full Table of Contents

### Module 1: Deep Positioning & Company Identity
[MODULE_01_POSITIONING.md](MODULE_01_POSITIONING.md)

- [1.1 Category Definition](MODULE_01_POSITIONING.md#11-category-definition)
  - [The Old Categories -- And Why None of Them Fit](MODULE_01_POSITIONING.md#the-old-categories--and-why-none-of-them-fit)
  - [The New Category: Claims Decision Engine](MODULE_01_POSITIONING.md#the-new-category-claims-decision-engine)
  - [The Shift: Why Now](MODULE_01_POSITIONING.md#the-shift-why-now)
- [1.2 ICP Deep Dive](MODULE_01_POSITIONING.md#12-icp-deep-dive)
  - [Three Personas, Three Selling Motions](MODULE_01_POSITIONING.md#three-personas-three-selling-motions)
  - [By Geography: EU vs US Personas](MODULE_01_POSITIONING.md#by-geography-eu-vs-us-personas)
  - [Carrier Segmentation (Anchored to Caravela)](MODULE_01_POSITIONING.md#carrier-segmentation-anchored-to-caravela)
- [1.3 All Personas in the Ecosystem](MODULE_01_POSITIONING.md#13-all-personas-in-the-ecosystem)
- [1.4 Core Value Proposition](MODULE_01_POSITIONING.md#14-core-value-proposition)
  - [The Mad-Lib](MODULE_01_POSITIONING.md#the-mad-lib)
  - [The Value Stack](MODULE_01_POSITIONING.md#the-value-stack)
- [1.5 The Company Description](MODULE_01_POSITIONING.md#15-the-company-description)
  - [Investor Version (Pitch Deck, Data Room, Formal Communications)](MODULE_01_POSITIONING.md#investor-version-pitch-deck-data-room-formal-communications)
  - [Sales Version (First Call with VP Claims)](MODULE_01_POSITIONING.md#sales-version-first-call-with-vp-claims)
  - [Technical / Integration Version](MODULE_01_POSITIONING.md#technical--integration-version)
  - [The Blunt Version (Internal Alignment)](MODULE_01_POSITIONING.md#the-blunt-version-internal-alignment)
- [1.6 Product Now vs Product Tomorrow](MODULE_01_POSITIONING.md#16-product-now-vs-product-tomorrow)
  - [Product Now (February 2026)](MODULE_01_POSITIONING.md#product-now-february-2026)
  - [Product Tomorrow (12-18 Month Vision)](MODULE_01_POSITIONING.md#product-tomorrow-12-18-month-vision)
- [1.7 Founder-Market Fit](MODULE_01_POSITIONING.md#17-founder-market-fit)
  - [This Is a Market-Pull Story, Not a Pivot Story](MODULE_01_POSITIONING.md#this-is-a-market-pull-story-not-a-pivot-story)
  - [The Founders](MODULE_01_POSITIONING.md#the-founders)
  - [Why This Team, Specifically](MODULE_01_POSITIONING.md#why-this-team-specifically)
- [1.8 One-Liner + Elevator Pitches](MODULE_01_POSITIONING.md#18-one-liner--elevator-pitches)
  - [One-Liners (by context)](MODULE_01_POSITIONING.md#one-liners-by-context)
  - [30-Second Elevator Pitch](MODULE_01_POSITIONING.md#30-second-elevator-pitch)
  - [2-Minute Elevator Pitch](MODULE_01_POSITIONING.md#2-minute-elevator-pitch)
  - [5-Minute Pitch](MODULE_01_POSITIONING.md#5-minute-pitch)
- [Unresolved Positioning Tensions](MODULE_01_POSITIONING.md#unresolved-positioning-tensions)
- [Sources](MODULE_01_POSITIONING.md#sources)

---

### Module 2: Problem Anatomy
[MODULE_02_PROBLEM.md](MODULE_02_PROBLEM.md)

- [2.1 Workflow Audit: The Before State](MODULE_02_PROBLEM.md#21-workflow-audit-the-before-state)
  - [What an Adjuster Actually Does Today](MODULE_02_PROBLEM.md#what-an-adjuster-actually-does-today)
- [2.2 The Villain](MODULE_02_PROBLEM.md#22-the-villain)
  - [The Enemy Is Not Any One System -- It's the Gap Between All of Them](MODULE_02_PROBLEM.md#the-enemy-is-not-any-one-system--its-the-gap-between-all-of-them)
- [2.3 The Workforce Crisis](MODULE_02_PROBLEM.md#23-the-workforce-crisis)
  - [The People Who Make These Decisions Are Disappearing](MODULE_02_PROBLEM.md#the-people-who-make-these-decisions-are-disappearing)
  - [Why This Creates Urgency](MODULE_02_PROBLEM.md#why-this-creates-urgency)
- [2.4 The STP Reality Gap](MODULE_02_PROBLEM.md#24-the-stp-reality-gap)
  - [Convention Systems Promise 60-70%. They Deliver ~10%.](MODULE_02_PROBLEM.md#convention-systems-promise-60-70-they-deliver-10)
  - [Why the Gap Exists](MODULE_02_PROBLEM.md#why-the-gap-exists)
  - [STP by Region](MODULE_02_PROBLEM.md#stp-by-region)
- [2.5 The Productivity Drain](MODULE_02_PROBLEM.md#25-the-productivity-drain)
  - [30-40% Admin. 5-7 Systems. 20+ Phone Calls Per Day.](MODULE_02_PROBLEM.md#30-40-admin-5-7-systems-20-phone-calls-per-day)
  - [The Productivity Math](MODULE_02_PROBLEM.md#the-productivity-math)
- [2.6 Reserve = P&L Impact](MODULE_02_PROBLEM.md#26-reserve--pl-impact)
  - [The CFO's Problem -- And Why It Opens a Second Buyer](MODULE_02_PROBLEM.md#the-cfos-problem--and-why-it-opens-a-second-buyer)
  - [How Reserves Work (for non-insurance readers)](MODULE_02_PROBLEM.md#how-reserves-work-for-non-insurance-readers)
  - [Why This Matters for Mysa's Sales Motion](MODULE_02_PROBLEM.md#why-this-matters-for-mysas-sales-motion)
- [2.7 Garbage In, Garbage Out](MODULE_02_PROBLEM.md#27-garbage-in-garbage-out)
  - [Fixing Intake Is a Prerequisite, Not the Product](MODULE_02_PROBLEM.md#fixing-intake-is-a-prerequisite-not-the-product)
- [2.8 Why Nobody Built the Decision Layer](MODULE_02_PROBLEM.md#28-why-nobody-built-the-decision-layer)
  - [It Requires Both Deep Domain AND Modern AI -- And That Combination Barely Exists](MODULE_02_PROBLEM.md#it-requires-both-deep-domain-and-modern-ai--and-that-combination-barely-exists)
  - [The Five Structural Barriers](MODULE_02_PROBLEM.md#the-five-structural-barriers)
  - [Why It's Possible NOW](MODULE_02_PROBLEM.md#why-its-possible-now)
- [Sources](MODULE_02_PROBLEM.md#sources)

---

### Module 3: The Claims Journey
[MODULE_03_CLAIMS_JOURNEY.md](MODULE_03_CLAIMS_JOURNEY.md)

- [3.1 Motor Claims EU: Full Lifecycle (Phases 0-11)](MODULE_03_CLAIMS_JOURNEY.md#31-motor-claims-eu-full-lifecycle-phases-0-11)
  - [Phase 0: The Incident (Seconds 0-60)](MODULE_03_CLAIMS_JOURNEY.md#phase-0-the-incident-seconds-0-60)
  - [Phase 1: Scene Management (Minutes 1-30)](MODULE_03_CLAIMS_JOURNEY.md#phase-1-scene-management-minutes-1-30)
  - [Phase 2: Documentation -- The EU Advantage](MODULE_03_CLAIMS_JOURNEY.md#phase-2-documentation--the-eu-advantage)
  - [Phase 3: Claim Triggering and Reconciliation](MODULE_03_CLAIMS_JOURNEY.md#phase-3-claim-triggering-and-reconciliation)
  - [Phase 4: First Contact](MODULE_03_CLAIMS_JOURNEY.md#phase-4-first-contact)
  - [Phase 5: FNOL (First Notice of Loss)](MODULE_03_CLAIMS_JOURNEY.md#phase-5-fnol-first-notice-of-loss)
  - [Phase 6: Triage (Hours 1-48)](MODULE_03_CLAIMS_JOURNEY.md#phase-6-triage-hours-1-48)
  - [Phase 7: Investigation (Days 1-30 for PD; Weeks 1-26+ for BI)](MODULE_03_CLAIMS_JOURNEY.md#phase-7-investigation-days-1-30-for-pd-weeks-1-26-for-bi)
  - [Phase 8: Assessment (Days 3-30 for PD; Weeks 4-52+ for BI)](MODULE_03_CLAIMS_JOURNEY.md#phase-8-assessment-days-3-30-for-pd-weeks-4-52-for-bi)
  - [Phase 9: Decision](MODULE_03_CLAIMS_JOURNEY.md#phase-9-decision)
  - [Phase 10: Settlement](MODULE_03_CLAIMS_JOURNEY.md#phase-10-settlement)
  - [Phase 11: Closure](MODULE_03_CLAIMS_JOURNEY.md#phase-11-closure)
  - [EU Phases 0-11 Summary Table](MODULE_03_CLAIMS_JOURNEY.md#eu-phases-0-11-summary-table)
- [3.2 Motor Claims US: Full Lifecycle (Phases 0-11)](MODULE_03_CLAIMS_JOURNEY.md#32-motor-claims-us-full-lifecycle-phases-0-11)
  - [How the US Differs From EU -- Phase by Phase](MODULE_03_CLAIMS_JOURNEY.md#how-the-us-differs-from-eu--phase-by-phase)
- [3.3 Home/Property Claims](MODULE_03_CLAIMS_JOURNEY.md#33-homeproperty-claims)
  - [Why Property Claims Are Structurally Different](MODULE_03_CLAIMS_JOURNEY.md#why-property-claims-are-structurally-different)
  - [Home Insurance Claim Types (US Data, 2019-2023)](MODULE_03_CLAIMS_JOURNEY.md#home-insurance-claim-types-us-data-2019-2023)
  - [Why Property Claims Almost ALWAYS Need an Adjuster](MODULE_03_CLAIMS_JOURNEY.md#why-property-claims-almost-always-need-an-adjuster)
  - [Property Claims FNOL Flow](MODULE_03_CLAIMS_JOURNEY.md#property-claims-fnol-flow)
  - [Documentation Burden Is MUCH Higher Than Motor](MODULE_03_CLAIMS_JOURNEY.md#documentation-burden-is-much-higher-than-motor)
  - [What a Property Adjuster Actually Does](MODULE_03_CLAIMS_JOURNEY.md#what-a-property-adjuster-actually-does)
  - [Property Field Adjuster Time Breakdown](MODULE_03_CLAIMS_JOURNEY.md#property-field-adjuster-time-breakdown)
  - [EU vs US: No Structural Advantage for Property](MODULE_03_CLAIMS_JOURNEY.md#eu-vs-us-no-structural-advantage-for-property)
  - [The Hidden Damage Problem](MODULE_03_CLAIMS_JOURNEY.md#the-hidden-damage-problem)
  - [The Fraud Challenge Is Getting Worse](MODULE_03_CLAIMS_JOURNEY.md#the-fraud-challenge-is-getting-worse)
  - [The Realistic Automation Opportunity](MODULE_03_CLAIMS_JOURNEY.md#the-realistic-automation-opportunity)
- [3.4 The 6 Decision Sub-Steps](MODULE_03_CLAIMS_JOURNEY.md#34-the-6-decision-sub-steps)
  - [Sub-Step 1: Coverage Verification](MODULE_03_CLAIMS_JOURNEY.md#sub-step-1-coverage-verification)
  - [Sub-Step 2: Liability Determination](MODULE_03_CLAIMS_JOURNEY.md#sub-step-2-liability-determination)
  - [Sub-Step 3: Repair Assessment](MODULE_03_CLAIMS_JOURNEY.md#sub-step-3-repair-assessment)
  - [Sub-Step 4: Cost Analysis](MODULE_03_CLAIMS_JOURNEY.md#sub-step-4-cost-analysis)
  - [Sub-Step 5: Reserve Calculation](MODULE_03_CLAIMS_JOURNEY.md#sub-step-5-reserve-calculation)
  - [Sub-Step 6: Fraud Assessment](MODULE_03_CLAIMS_JOURNEY.md#sub-step-6-fraud-assessment)
  - [The 6 Sub-Steps Combined: Time Savings Opportunity](MODULE_03_CLAIMS_JOURNEY.md#the-6-sub-steps-combined-time-savings-opportunity)
- [3.5 EU vs US Comparison](MODULE_03_CLAIMS_JOURNEY.md#35-eu-vs-us-comparison)
  - [Side-by-Side Across Every Dimension](MODULE_03_CLAIMS_JOURNEY.md#side-by-side-across-every-dimension)
  - [Automation Opportunity by Market](MODULE_03_CLAIMS_JOURNEY.md#automation-opportunity-by-market)
- [3.6 All Personas and Their Roles](MODULE_03_CLAIMS_JOURNEY.md#36-all-personas-and-their-roles)
  - [Primary Personas (Direct Users of Mysa)](MODULE_03_CLAIMS_JOURNEY.md#primary-personas-direct-users-of-mysa)
  - [Secondary Personas (Interact with Mysa Indirectly)](MODULE_03_CLAIMS_JOURNEY.md#secondary-personas-interact-with-mysa-indirectly)
  - [External Personas](MODULE_03_CLAIMS_JOURNEY.md#external-personas)
  - [Major TPAs (Third-Party Administrators)](MODULE_03_CLAIMS_JOURNEY.md#major-tpas-third-party-administrators)
- [3.7 Decision Forks and Complexity Scoring](MODULE_03_CLAIMS_JOURNEY.md#37-decision-forks-and-complexity-scoring)
  - [The 8 Decision Forks](MODULE_03_CLAIMS_JOURNEY.md#the-8-decision-forks)
  - [Triage Logic: How Claims Are Routed](MODULE_03_CLAIMS_JOURNEY.md#triage-logic-how-claims-are-routed)
  - [Claim Complexity Scoring](MODULE_03_CLAIMS_JOURNEY.md#claim-complexity-scoring)
- [3.8 The "Adjuster of 2027" Vision](MODULE_03_CLAIMS_JOURNEY.md#38-the-adjuster-of-2027-vision)
  - [Today's Adjuster (2025-2026)](MODULE_03_CLAIMS_JOURNEY.md#todays-adjuster-2025-2026)
  - [The Mysa-Enabled Adjuster (2027)](MODULE_03_CLAIMS_JOURNEY.md#the-mysa-enabled-adjuster-2027)
  - [Concrete Before/After Comparison](MODULE_03_CLAIMS_JOURNEY.md#concrete-beforeafter-comparison)
  - [The Flywheel: Every Claim Makes the System Smarter](MODULE_03_CLAIMS_JOURNEY.md#the-flywheel-every-claim-makes-the-system-smarter)
  - [The 2027 Adjuster Is Not Replaced -- They Are Elevated](MODULE_03_CLAIMS_JOURNEY.md#the-2027-adjuster-is-not-replaced--they-are-elevated)
- [Sources](MODULE_03_CLAIMS_JOURNEY.md#sources)

---

### Module 4: Market Landscape
[MODULE_04_MARKET.md](MODULE_04_MARKET.md)

- [Glossary](MODULE_04_MARKET.md#glossary)
- [4.1 Global Overview](MODULE_04_MARKET.md#41-global-overview)
  - [The Opportunity at a Glance](MODULE_04_MARKET.md#the-opportunity-at-a-glance)
  - [Total Claims Volume -- Motor + Property](MODULE_04_MARKET.md#total-claims-volume--motor--property)
  - [Total Premium (GWP / DWP)](MODULE_04_MARKET.md#total-premium-gwp--dwp)
  - [Motor vs Property: Two Lines, One Market](MODULE_04_MARKET.md#motor-vs-property-two-lines-one-market)
  - [Total Carrier/Buyer Universe](MODULE_04_MARKET.md#total-carrierbuyer-universe)
- [4.2 EU Market by Country](MODULE_04_MARKET.md#42-eu-market-by-country)
  - [4.2.1 Southern EU (Convention System Countries -- The Wedge)](MODULE_04_MARKET.md#421-southern-eu-convention-system-countries--the-wedge)
  - [4.2.2 Northern/Central EU (Mixed Convention Systems -- Expansion Markets)](MODULE_04_MARKET.md#422-northerncentral-eu-mixed-convention-systems--expansion-markets)
  - [4.2.3 EU Grand Totals](MODULE_04_MARKET.md#423-eu-grand-totals)
- [4.3 US Market](MODULE_04_MARKET.md#43-us-market)
  - [US Market Structure](MODULE_04_MARKET.md#us-market-structure)
  - [US Carrier Distribution by Size](MODULE_04_MARKET.md#us-carrier-distribution-by-size)
  - [US Non-Carrier Buyers (Unique to US)](MODULE_04_MARKET.md#us-non-carrier-buyers-unique-to-us)
  - [Total US Addressable Buyers](MODULE_04_MARKET.md#total-us-addressable-buyers)
  - [US Homeowners -- Key Metrics](MODULE_04_MARKET.md#us-homeowners--key-metrics)
  - [Why Property, Not Auto, in the US](MODULE_04_MARKET.md#why-property-not-auto-in-the-us)
  - [Named US Mid-Market Carriers (Property-Strong)](MODULE_04_MARKET.md#named-us-mid-market-carriers-property-strong)
- [4.4 Why Bottom-Up: Mid/Small First, Not Enterprise](MODULE_04_MARKET.md#44-why-bottom-up-midsmall-first-not-enterprise)
  - [The Enterprise Trap](MODULE_04_MARKET.md#the-enterprise-trap)
  - [Why Mid/Small Works](MODULE_04_MARKET.md#why-midsmall-works)
  - [Bottom-Up Expansion Path](MODULE_04_MARKET.md#bottom-up-expansion-path)
- [4.5 Caravela Tier Sweet Spot](MODULE_04_MARKET.md#45-caravela-tier-sweet-spot)
  - [The Anchor: Caravela Seguros](MODULE_04_MARKET.md#the-anchor-caravela-seguros)
  - [Why EUR100-200M GWP Is Optimal](MODULE_04_MARKET.md#why-eur100-200m-gwp-is-optimal)
  - [Named Caravela-Tier Carriers by Market](MODULE_04_MARKET.md#named-caravela-tier-carriers-by-market)
- [4.6 Mid-Market vs Small: Different Needs](MODULE_04_MARKET.md#46-mid-market-vs-small-different-needs)
  - [By Carrier Size](MODULE_04_MARKET.md#by-carrier-size)
  - [By Line of Business](MODULE_04_MARKET.md#by-line-of-business)
  - [By Region](MODULE_04_MARKET.md#by-region)
- [4.7 Motor + Property Overlap](MODULE_04_MARKET.md#47-motor--property-overlap)
  - [The Same Buyers](MODULE_04_MARKET.md#the-same-buyers)
  - [The Same Workflow (~80% Identical)](MODULE_04_MARKET.md#the-same-workflow-80-identical)
  - [Revenue Uplift: +60-70% Per Carrier, Zero New Acquisition](MODULE_04_MARKET.md#revenue-uplift-60-70-per-carrier-zero-new-acquisition)
- [4.8 TAM Calculations](MODULE_04_MARKET.md#48-tam-calculations)
  - [EU Carrier Size Distribution (Full Segmentation)](MODULE_04_MARKET.md#eu-carrier-size-distribution-full-segmentation)
  - [US Carrier Distribution (For Comparison)](MODULE_04_MARKET.md#us-carrier-distribution-for-comparison)
  - [Target Segment Claims Volume](MODULE_04_MARKET.md#target-segment-claims-volume)
  - [Target as Percentage of Total Market](MODULE_04_MARKET.md#target-as-percentage-of-total-market)
  - [TAM Scenarios -- Motor Only (Bottom-Up from Validated Carrier Counts)](MODULE_04_MARKET.md#tam-scenarios--motor-only-bottom-up-from-validated-carrier-counts)
  - [TAM Scenarios -- Motor + Property Combined (Same Buyers, +60-70% Revenue)](MODULE_04_MARKET.md#tam-scenarios--motor--property-combined-same-buyers-60-70-revenue)
  - [The Honest TAM Narrative](MODULE_04_MARKET.md#the-honest-tam-narrative)
  - [The Fundraising TAM Story](MODULE_04_MARKET.md#the-fundraising-tam-story)
  - [Market Openness -- Why This TAM Is Actually Accessible](MODULE_04_MARKET.md#market-openness--why-this-tam-is-actually-accessible)
- [Sources](MODULE_04_MARKET.md#sources)

---

### Module 5: Competitive Landscape
[MODULE_05_COMPETITION.md](MODULE_05_COMPETITION.md)

- [How to Read This Module](MODULE_05_COMPETITION.md#how-to-read-this-module)
- [5.1 Where NOT to Go -- The Crowded Zones](MODULE_05_COMPETITION.md#51-where-not-to-go--the-crowded-zones)
  - [Intake Automation (~$1B+ in combined funding)](MODULE_05_COMPETITION.md#intake-automation-1b-in-combined-funding)
  - [Fraud Detection (~$320M+ in dedicated funding)](MODULE_05_COMPETITION.md#fraud-detection-320m-in-dedicated-funding)
  - [Estimation Tools (Verisk = $35B+ market cap)](MODULE_05_COMPETITION.md#estimation-tools-verisk--35b-market-cap)
  - [The Takeaway](MODULE_05_COMPETITION.md#the-takeaway)
- [5.2 Where Mysa Wins -- The Unoccupied Territory](MODULE_05_COMPETITION.md#52-where-mysa-wins--the-unoccupied-territory)
  - [Convention Systems (Zero Competition -- Confirmed)](MODULE_05_COMPETITION.md#convention-systems-zero-competition--confirmed)
  - [Coverage Determination (~99% Empty)](MODULE_05_COMPETITION.md#coverage-determination-99-empty)
  - [SOP-Driven Workflows (Nobody Does Carrier-Specific)](MODULE_05_COMPETITION.md#sop-driven-workflows-nobody-does-carrier-specific)
  - [Decision Ground Truth (New Data Category)](MODULE_05_COMPETITION.md#decision-ground-truth-new-data-category)
- [5.3 Five Sigma / Clive -- The Closest Competitor](MODULE_05_COMPETITION.md#53-five-sigma--clive--the-closest-competitor)
  - [What Five Sigma Actually Does](MODULE_05_COMPETITION.md#what-five-sigma-actually-does)
  - [Company Profile](MODULE_05_COMPETITION.md#company-profile)
  - [What Clive's Agents Do](MODULE_05_COMPETITION.md#what-clives-agents-do)
  - [How They Sell](MODULE_05_COMPETITION.md#how-they-sell)
  - [Pricing Model](MODULE_05_COMPETITION.md#pricing-model)
  - [Is Clive Actually Autonomous?](MODULE_05_COMPETITION.md#is-clive-actually-autonomous)
  - [Five Sigma's Confirmed Gaps (Mysa's Advantages)](MODULE_05_COMPETITION.md#five-sigmas-confirmed-gaps-mysas-advantages)
  - [Why Five Sigma Matters](MODULE_05_COMPETITION.md#why-five-sigma-matters)
- [5.4 Verisk / XactAI -- The Existential Long-Term Risk](MODULE_05_COMPETITION.md#54-verisk--xactai--the-existential-long-term-risk)
  - [What Verisk Actually Is](MODULE_05_COMPETITION.md#what-verisk-actually-is)
  - [What XactAI Actually Does (Launched September 2025)](MODULE_05_COMPETITION.md#what-xactai-actually-does-launched-september-2025)
  - [Why Mysa Has Time (For Now)](MODULE_05_COMPETITION.md#why-mysa-has-time-for-now)
  - [Why This Risk Is Existential](MODULE_05_COMPETITION.md#why-this-risk-is-existential)
  - [Mysa's Defensive Strategy](MODULE_05_COMPETITION.md#mysas-defensive-strategy)
- [5.5 Shift Technology -- The EU Danger](MODULE_05_COMPETITION.md#55-shift-technology--the-eu-danger)
  - [What Shift Technology Actually Is](MODULE_05_COMPETITION.md#what-shift-technology-actually-is)
  - [Company Profile](MODULE_05_COMPETITION.md#company-profile-1)
  - [Shift's Product Portfolio](MODULE_05_COMPETITION.md#shifts-product-portfolio)
  - [The "60% Automation Rate" -- What It Actually Means](MODULE_05_COMPETITION.md#the-60-automation-rate--what-it-actually-means)
  - [The Key Distinction: Workflow vs. Judgment](MODULE_05_COMPETITION.md#the-key-distinction-workflow-vs-judgment)
  - [Shift Technology's Confirmed Gaps](MODULE_05_COMPETITION.md#shift-technologys-confirmed-gaps)
  - [Why Shift Is the EU Danger](MODULE_05_COMPETITION.md#why-shift-is-the-eu-danger)
- [5.6 Wamy -- The New Entrant](MODULE_05_COMPETITION.md#56-wamy--the-new-entrant)
  - [What We Know](MODULE_05_COMPETITION.md#what-we-know)
  - [What Wamy Claims to Do](MODULE_05_COMPETITION.md#what-wamy-claims-to-do)
  - [Assessment](MODULE_05_COMPETITION.md#assessment)
- [5.7 Secondary Competitors](MODULE_05_COMPETITION.md#57-secondary-competitors)
  - [Assured (~$1B Valuation)](MODULE_05_COMPETITION.md#assured-1b-valuation)
  - [Avallon ($4.6M Seed, YC S25)](MODULE_05_COMPETITION.md#avallon-46m-seed-yc-s25)
  - [ClaimSorted (~$13.3M Raised)](MODULE_05_COMPETITION.md#claimsorted-133m-raised)
  - [FurtherAI ($30M, a16z)](MODULE_05_COMPETITION.md#furtherai-30m-a16z)
  - [omni:us (~EUR 45M Raised)](MODULE_05_COMPETITION.md#omnius-eur-45m-raised)
  - [MarvelX (EUR 5.4M, Founded 2025)](MODULE_05_COMPETITION.md#marvelx-eur-54m-founded-2025)
  - [Crawford / Turvi CoverAI](MODULE_05_COMPETITION.md#crawford--turvi-coverai)
  - [Tractable](MODULE_05_COMPETITION.md#tractable)
  - [Bdeo](MODULE_05_COMPETITION.md#bdeo)
  - [Hi Marley](MODULE_05_COMPETITION.md#hi-marley)
  - [CCC / EvolutionIQ ($730M Acquisition)](MODULE_05_COMPETITION.md#ccc--evolutioniq-730m-acquisition)
- [5.8 The Property Claims AI Gap](MODULE_05_COMPETITION.md#58-the-property-claims-ai-gap)
  - [$3B+ Invested in Physical Tools, ~$0 in Decision Tools](MODULE_05_COMPETITION.md#3b-invested-in-physical-tools-0-in-decision-tools)
  - [The Gap Stated Precisely](MODULE_05_COMPETITION.md#the-gap-stated-precisely)
  - [The Honest Competitive Map for Property](MODULE_05_COMPETITION.md#the-honest-competitive-map-for-property)
  - [Why This Gap Exists](MODULE_05_COMPETITION.md#why-this-gap-exists)
- [5.9 The Moat -- Mysa's Competitive Defenses](MODULE_05_COMPETITION.md#59-the-moat--mysas-competitive-defenses)
  - [Layer 1: Decision Ground Truth Data](MODULE_05_COMPETITION.md#layer-1-decision-ground-truth-data)
  - [Layer 2: SOP-Encoded Workflows (Carrier Lock-In)](MODULE_05_COMPETITION.md#layer-2-sop-encoded-workflows-carrier-lock-in)
  - [Layer 3: Convention System Expertise](MODULE_05_COMPETITION.md#layer-3-convention-system-expertise)
  - [Layer 4: Annotation Tools as Competitive Weapon](MODULE_05_COMPETITION.md#layer-4-annotation-tools-as-competitive-weapon)
- [5.10 Master Comparison Matrix](MODULE_05_COMPETITION.md#510-master-comparison-matrix)
  - [Multi-Dimensional Competitive Assessment](MODULE_05_COMPETITION.md#multi-dimensional-competitive-assessment)
  - [Key Risk to Mysa -- Per Competitor](MODULE_05_COMPETITION.md#key-risk-to-mysa--per-competitor)
- [The Honest Summary](MODULE_05_COMPETITION.md#the-honest-summary)
- [Sources](MODULE_05_COMPETITION.md#sources)

---

### Module 6: Product Specification & Demo
[MODULE_06_PRODUCT.md](MODULE_06_PRODUCT.md)

- [6.1 Product Flow](MODULE_06_PRODUCT.md#61-product-flow)
  - [The 7-Step Claims Pipeline](MODULE_06_PRODUCT.md#the-7-step-claims-pipeline)
  - [System Logic Summary per Step](MODULE_06_PRODUCT.md#system-logic-summary-per-step)
- [6.2 The 6 Decision Sub-Steps](MODULE_06_PRODUCT.md#62-the-6-decision-sub-steps)
  - [Detailed Breakdown](MODULE_06_PRODUCT.md#detailed-breakdown)
  - [Sub-Step 1: Coverage Verification](MODULE_06_PRODUCT.md#sub-step-1-coverage-verification)
  - [Sub-Step 2: Policy Report Checking](MODULE_06_PRODUCT.md#sub-step-2-policy-report-checking)
  - [Sub-Step 3: Repair Assessment](MODULE_06_PRODUCT.md#sub-step-3-repair-assessment)
  - [Sub-Step 4: Cost Analysis](MODULE_06_PRODUCT.md#sub-step-4-cost-analysis)
  - [Sub-Step 5: Reserve Calculation](MODULE_06_PRODUCT.md#sub-step-5-reserve-calculation)
  - [Sub-Step 6: Fraud Detection](MODULE_06_PRODUCT.md#sub-step-6-fraud-detection)
  - [Decision Sub-Steps Summary](MODULE_06_PRODUCT.md#decision-sub-steps-summary)
- [6.3 SOP-Driven Workflow Engine](MODULE_06_PRODUCT.md#63-sop-driven-workflow-engine)
  - [Why SOPs Are the Core Differentiator](MODULE_06_PRODUCT.md#why-sops-are-the-core-differentiator)
  - [How It Works](MODULE_06_PRODUCT.md#how-it-works)
  - [Three Workflow Types](MODULE_06_PRODUCT.md#three-workflow-types)
  - [Why This Creates Lock-In](MODULE_06_PRODUCT.md#why-this-creates-lock-in)
- [6.4 The Core Loop](MODULE_06_PRODUCT.md#64-the-core-loop)
  - [Trigger -> Action -> Reward -> Investment](MODULE_06_PRODUCT.md#trigger---action---reward---investment)
  - [The Flywheel Timeline](MODULE_06_PRODUCT.md#the-flywheel-timeline)
  - [Why the Loop Compounds](MODULE_06_PRODUCT.md#why-the-loop-compounds)
- [6.5 The "Clippy" Architecture](MODULE_06_PRODUCT.md#65-the-clippy-architecture)
  - [Concept: Insurance Knowledge Clippy](MODULE_06_PRODUCT.md#concept-insurance-knowledge-clippy)
  - [Why a Chrome Extension](MODULE_06_PRODUCT.md#why-a-chrome-extension)
  - [How It Works](MODULE_06_PRODUCT.md#how-it-works-1)
  - [Three Components of the Clippy Architecture](MODULE_06_PRODUCT.md#three-components-of-the-clippy-architecture)
  - [Why This Architecture Wins](MODULE_06_PRODUCT.md#why-this-architecture-wins)
  - [Limitations](MODULE_06_PRODUCT.md#limitations)
- [6.6 All Personas & How the Product Helps Each](MODULE_06_PRODUCT.md#66-all-personas--how-the-product-helps-each)
- [6.7 User Journey Maps](MODULE_06_PRODUCT.md#67-user-journey-maps)
  - [Journey 1: New Claim Intake (Desk Adjuster -- Motor PD)](MODULE_06_PRODUCT.md#journey-1-new-claim-intake-desk-adjuster--motor-pd)
  - [Journey 2: Investigation (Field Adjuster -- Complex Motor)](MODULE_06_PRODUCT.md#journey-2-investigation-field-adjuster--complex-motor)
  - [Journey 3: Decision (Desk Adjuster -- US Property Water Damage)](MODULE_06_PRODUCT.md#journey-3-decision-desk-adjuster--us-property-water-damage)
  - [Journey 4: Settlement (EU Motor -- Convention Claim)](MODULE_06_PRODUCT.md#journey-4-settlement-eu-motor--convention-claim)
- [6.8 Human-in-the-Loop: Why](MODULE_06_PRODUCT.md#68-human-in-the-loop-why)
  - [The Non-Negotiable Design Principle](MODULE_06_PRODUCT.md#the-non-negotiable-design-principle)
  - [(a) Regulatory Requirement](MODULE_06_PRODUCT.md#a-regulatory-requirement)
  - [(b) Trust: Adjusters Will Not Use Black Boxes](MODULE_06_PRODUCT.md#b-trust-adjusters-will-not-use-black-boxes)
  - [(c) Training Data: Every Correction Improves the Model](MODULE_06_PRODUCT.md#c-training-data-every-correction-improves-the-model)
  - [(d) Liability: Human Decides, AI Recommends](MODULE_06_PRODUCT.md#d-liability-human-decides-ai-recommends)
- [6.9 Demo Spec: Adjuster Portal](MODULE_06_PRODUCT.md#69-demo-spec-adjuster-portal)
  - [Design Principle: Block by Block](MODULE_06_PRODUCT.md#design-principle-block-by-block)
  - [Demo 1: EU Motor -- EAS to Settlement ("The Easy Case")](MODULE_06_PRODUCT.md#demo-1-eu-motor--eas-to-settlement-the-easy-case)
  - [Demo 2: US Property -- Water Damage ("The Hard Case")](MODULE_06_PRODUCT.md#demo-2-us-property--water-damage-the-hard-case)
  - [Demo 3: Historical Data Flywheel (If Time Permits)](MODULE_06_PRODUCT.md#demo-3-historical-data-flywheel-if-time-permits)
  - [Demo Requirements Summary](MODULE_06_PRODUCT.md#demo-requirements-summary)
- [6.10 Demo Spec: Broker Flow](MODULE_06_PRODUCT.md#610-demo-spec-broker-flow)
  - [The Broker Problem](MODULE_06_PRODUCT.md#the-broker-problem)
  - [The Mysa Broker Flow](MODULE_06_PRODUCT.md#the-mysa-broker-flow)
  - [Broker Demo Flow (Full Walkthrough)](MODULE_06_PRODUCT.md#broker-demo-flow-full-walkthrough)
- [6.11 Demo Data & Workflow Specs](MODULE_06_PRODUCT.md#611-demo-data--workflow-specs)
  - [Realistic Claim Data Examples](MODULE_06_PRODUCT.md#realistic-claim-data-examples)
  - [Example 1: EU Motor -- Portuguese Convention Claim](MODULE_06_PRODUCT.md#example-1-eu-motor--portuguese-convention-claim)
  - [Example 2: US Property -- Water Damage Claim](MODULE_06_PRODUCT.md#example-2-us-property--water-damage-claim)
  - [Triage Decision Logic (From Discovery Phases 6-8)](MODULE_06_PRODUCT.md#triage-decision-logic-from-discovery-phases-6-8)
  - [Investigation Activities Reference (Phase 7)](MODULE_06_PRODUCT.md#investigation-activities-reference-phase-7)
  - [Assessment Activities Reference (Phase 8)](MODULE_06_PRODUCT.md#assessment-activities-reference-phase-8)
  - [Settlement Activities Reference (Phases 9-10)](MODULE_06_PRODUCT.md#settlement-activities-reference-phases-9-10)
  - [Convention System Quick Reference](MODULE_06_PRODUCT.md#convention-system-quick-reference)
  - [Authority Matrix Template](MODULE_06_PRODUCT.md#authority-matrix-template)
- [Sources](MODULE_06_PRODUCT.md#sources)

---

### Module 7: Technical Architecture
[MODULE_07_TECHNICAL.md](MODULE_07_TECHNICAL.md)

- [7.1 Architecture Philosophy](MODULE_07_TECHNICAL.md#71-architecture-philosophy)
  - [Agent-Native: Why This Is Not a Feature Choice](MODULE_07_TECHNICAL.md#agent-native-why-this-is-not-a-feature-choice)
  - [Why "Add AI to Existing Software" Fails](MODULE_07_TECHNICAL.md#why-add-ai-to-existing-software-fails)
  - [The Atomic Tools Principle](MODULE_07_TECHNICAL.md#the-atomic-tools-principle)
- [7.2 Current Stack](MODULE_07_TECHNICAL.md#72-current-stack)
  - [What Exists Today: The Caravela Pilot](MODULE_07_TECHNICAL.md#what-exists-today-the-caravela-pilot)
  - [Key Metrics](MODULE_07_TECHNICAL.md#key-metrics)
  - [What This Proves](MODULE_07_TECHNICAL.md#what-this-proves)
  - [What This Does Not Do Yet](MODULE_07_TECHNICAL.md#what-this-does-not-do-yet)
- [7.3 Production Stack Vision](MODULE_07_TECHNICAL.md#73-production-stack-vision)
  - [Where This Needs to Go](MODULE_07_TECHNICAL.md#where-this-needs-to-go)
  - [Non-Negotiable Requirements](MODULE_07_TECHNICAL.md#non-negotiable-requirements)
  - [Cloud Provider Decision [FOUNDER INPUT REQUIRED]](MODULE_07_TECHNICAL.md#cloud-provider-decision-founder-input-required)
  - [Multi-Agent Architecture [FOUNDER INPUT REQUIRED]](MODULE_07_TECHNICAL.md#multi-agent-architecture-founder-input-required)
- [7.4 OCR & Document Processing](MODULE_07_TECHNICAL.md#74-ocr--document-processing)
  - [Current Performance](MODULE_07_TECHNICAL.md#current-performance)
  - [How It Works](MODULE_07_TECHNICAL.md#how-it-works)
  - [Where the 18.5% Error Gap Comes From](MODULE_07_TECHNICAL.md#where-the-185-error-gap-comes-from)
  - [Path to 90%+](MODULE_07_TECHNICAL.md#path-to-90)
  - [The Benchmark System](MODULE_07_TECHNICAL.md#the-benchmark-system)
- [7.5 Convention Matching Engine](MODULE_07_TECHNICAL.md#75-convention-matching-engine)
  - [What Convention Systems Are](MODULE_07_TECHNICAL.md#what-convention-systems-are)
  - [Convention Systems by Country](MODULE_07_TECHNICAL.md#convention-systems-by-country)
  - [How It Works Technically](MODULE_07_TECHNICAL.md#how-it-works-technically)
  - [Why This Is a Structural Moat](MODULE_07_TECHNICAL.md#why-this-is-a-structural-moat)
- [7.6 Integration Map: Open vs. Locked](MODULE_07_TECHNICAL.md#76-integration-map-open-vs-locked)
  - [Integration Accessibility Table](MODULE_07_TECHNICAL.md#integration-accessibility-table)
  - [Strategic Implications](MODULE_07_TECHNICAL.md#strategic-implications)
- [7.7 Agentic Approach for Locked Systems](MODULE_07_TECHNICAL.md#77-agentic-approach-for-locked-systems)
  - [The Problem](MODULE_07_TECHNICAL.md#the-problem)
  - [The Solution: Chrome Extension + Desktop Agent](MODULE_07_TECHNICAL.md#the-solution-chrome-extension--desktop-agent)
  - [Why This Works](MODULE_07_TECHNICAL.md#why-this-works)
  - [Limitations](MODULE_07_TECHNICAL.md#limitations-1)
  - [Build vs. Wait Decision [FOUNDER INPUT REQUIRED]](MODULE_07_TECHNICAL.md#build-vs-wait-decision-founder-input-required)
- [7.8 Data Model & Knowledge Layer](MODULE_07_TECHNICAL.md#78-data-model--knowledge-layer)
  - [Core Entities](MODULE_07_TECHNICAL.md#core-entities)
  - [Knowledge Layer Sources and Ingestion](MODULE_07_TECHNICAL.md#knowledge-layer-sources-and-ingestion)
  - [Knowledge Acquisition Phases](MODULE_07_TECHNICAL.md#knowledge-acquisition-phases)
  - [The Defensibility Stack](MODULE_07_TECHNICAL.md#the-defensibility-stack)
- [7.9 EU + US Compliance](MODULE_07_TECHNICAL.md#79-eu--us-compliance)
  - [GDPR (General Data Protection Regulation)](MODULE_07_TECHNICAL.md#gdpr-general-data-protection-regulation)
  - [EU AI Act (Regulation 2024/1689)](MODULE_07_TECHNICAL.md#eu-ai-act-regulation-20241689)
  - [US State-by-State Insurance Regulation](MODULE_07_TECHNICAL.md#us-state-by-state-insurance-regulation)
  - [Data Residency Architecture](MODULE_07_TECHNICAL.md#data-residency-architecture)
  - [Compliance Gaps Requiring Founder Decision [FOUNDER INPUT REQUIRED]](MODULE_07_TECHNICAL.md#compliance-gaps-requiring-founder-decision-founder-input-required)
- [Sources](MODULE_07_TECHNICAL.md#sources)

---

### Module 8: Data & Flywheel Strategy
[MODULE_08_DATA.md](MODULE_08_DATA.md)

- [8.1 The Data Moat Thesis](MODULE_08_DATA.md#81-the-data-moat-thesis)
  - [Three Data Owners, One Gap](MODULE_08_DATA.md#three-data-owners-one-gap)
  - [The Missing Data Category: Decision Reasoning](MODULE_08_DATA.md#the-missing-data-category-decision-reasoning)
  - [Why Nobody Else Has It](MODULE_08_DATA.md#why-nobody-else-has-it)
  - [The Thesis in One Sentence](MODULE_08_DATA.md#the-thesis-in-one-sentence)
- [8.2 Flywheel Mechanics](MODULE_08_DATA.md#82-flywheel-mechanics)
  - [The Five Stages](MODULE_08_DATA.md#the-five-stages)
  - [Stage 1: Day 1 -- SOP Workflows + Document Parsing](MODULE_08_DATA.md#stage-1-day-1--sop-workflows--document-parsing)
  - [Stage 2: Month 3 -- Historical Claims Data Ingested](MODULE_08_DATA.md#stage-2-month-3--historical-claims-data-ingested)
  - [Stage 3: Month 6 -- Decision Ground Truth Captured](MODULE_08_DATA.md#stage-3-month-6--decision-ground-truth-captured)
  - [Stage 4: Month 12 -- Predictive Models](MODULE_08_DATA.md#stage-4-month-12--predictive-models)
  - [Stage 5: Month 18+ -- Near-STP](MODULE_08_DATA.md#stage-5-month-18--near-stp)
  - [Flywheel Compounding: Why Each Stage Accelerates the Next](MODULE_08_DATA.md#flywheel-compounding-why-each-stage-accelerates-the-next)
- [8.3 Datasets: Connect vs Build](MODULE_08_DATA.md#83-datasets-connect-vs-build)
  - [Datasets to Connect (External, Available)](MODULE_08_DATA.md#datasets-to-connect-external-available)
  - [Datasets to Build (Proprietary, Defensible)](MODULE_08_DATA.md#datasets-to-build-proprietary-defensible)
  - [The Strategic Distinction](MODULE_08_DATA.md#the-strategic-distinction)
- [8.4 Annotation as Product & Strategic Asset](MODULE_08_DATA.md#84-annotation-as-product--strategic-asset)
  - [The Core Insight](MODULE_08_DATA.md#the-core-insight)
  - [(a) Solving Cold Start: Historical Data Unlocks Day 1 Value](MODULE_08_DATA.md#a-solving-cold-start-historical-data-unlocks-day-1-value)
  - [(b) Creating Switching Costs: Re-annotating from Scratch Is Prohibitive](MODULE_08_DATA.md#b-creating-switching-costs-re-annotating-from-scratch-is-prohibitive)
  - [(c) The Sales Argument: "We Give YOU Tools to Build YOUR AI on YOUR Data"](MODULE_08_DATA.md#c-the-sales-argument-we-give-you-tools-to-build-your-ai-on-your-data)
  - [(d) The Quality Flywheel: 44 Claims to Normalization Rules to Accuracy](MODULE_08_DATA.md#d-the-quality-flywheel-44-claims-to-normalization-rules-to-accuracy)
  - [(e) A New Data Category Nobody Else Has](MODULE_08_DATA.md#e-a-new-data-category-nobody-else-has)
- [8.5 Legal Framework for Data Operations](MODULE_08_DATA.md#85-legal-framework-for-data-operations)
  - [The Regulatory Landscape](MODULE_08_DATA.md#the-regulatory-landscape)
  - [Data Processing Agreements (DPAs)](MODULE_08_DATA.md#data-processing-agreements-dpas)
  - [Anonymization Strategy](MODULE_08_DATA.md#anonymization-strategy)
  - [Model Training Rights](MODULE_08_DATA.md#model-training-rights)
  - [Carrier Data Ownership](MODULE_08_DATA.md#carrier-data-ownership)
  - [EU AI Act Compliance](MODULE_08_DATA.md#eu-ai-act-compliance)
  - [GDPR Compliance for Training Data](MODULE_08_DATA.md#gdpr-compliance-for-training-data)
- [8.6 Mid-market vs Small: Different Data Needs](MODULE_08_DATA.md#86-mid-market-vs-small-different-data-needs)
  - [The Segmentation Reality](MODULE_08_DATA.md#the-segmentation-reality)
  - [By Carrier Size](MODULE_08_DATA.md#by-carrier-size)
  - [By Geography and Regulation](MODULE_08_DATA.md#by-geography-and-regulation)
  - [Concrete Example: EUR 150M French Carrier vs EUR 50M Portuguese Mutual](MODULE_08_DATA.md#concrete-example-eur-150m-french-carrier-vs-eur-50m-portuguese-mutual)
- [8.7 Network Effects & Switching Costs](MODULE_08_DATA.md#87-network-effects--switching-costs)
  - [The Four Layers of Lock-in](MODULE_08_DATA.md#the-four-layers-of-lock-in)
  - [Layer-by-Layer Time to Replicate](MODULE_08_DATA.md#layer-by-layer-time-to-replicate)
  - [Cross-Carrier Learning: The Network Effect](MODULE_08_DATA.md#cross-carrier-learning-the-network-effect)
  - [Why the Moat Compounds Over Time](MODULE_08_DATA.md#why-the-moat-compounds-over-time)
  - [The Exit Argument](MODULE_08_DATA.md#the-exit-argument)
- [Sources](MODULE_08_DATA.md#sources)

---

### Module 9: Go-to-Market
[MODULE_09_GTM.md](MODULE_09_GTM.md)

- [9.1 Why This Rollout Order](MODULE_09_GTM.md#91-why-this-rollout-order)
  - [The Logic Chain](MODULE_09_GTM.md#the-logic-chain)
- [9.2 Phase 1: Portugal (Caravela)](MODULE_09_GTM.md#92-phase-1-portugal-caravela)
  - [Why Portugal First](MODULE_09_GTM.md#why-portugal-first)
  - [The Design Partner: Caravela Seguros](MODULE_09_GTM.md#the-design-partner-caravela-seguros)
  - [The Commercial Motion](MODULE_09_GTM.md#the-commercial-motion)
  - [Adjacent Portuguese Targets](MODULE_09_GTM.md#adjacent-portuguese-targets)
  - [The ROI Case (Caravela-Specific)](MODULE_09_GTM.md#the-roi-case-caravela-specific)
- [9.3 Phase 2: Southern EU Motor](MODULE_09_GTM.md#93-phase-2-southern-eu-motor)
  - [Why Southern EU Second](MODULE_09_GTM.md#why-southern-eu-second)
  - [Country-by-Country](MODULE_09_GTM.md#country-by-country)
  - [Phase 2 Combined Targets](MODULE_09_GTM.md#phase-2-combined-targets)
- [9.4 Phase 3: Property (Same Buyers)](MODULE_09_GTM.md#94-phase-3-property-same-buyers)
  - [Why Property Before Northern EU](MODULE_09_GTM.md#why-property-before-northern-eu)
  - [The Same-Buyer Argument](MODULE_09_GTM.md#the-same-buyer-argument)
  - [What Changes for Property](MODULE_09_GTM.md#what-changes-for-property)
  - [The Revenue Math](MODULE_09_GTM.md#the-revenue-math)
  - [Property Market by Geography](MODULE_09_GTM.md#property-market-by-geography)
  - [Phase 3 Target](MODULE_09_GTM.md#phase-3-target)
- [9.5 Phase 4: Northern EU](MODULE_09_GTM.md#95-phase-4-northern-eu)
  - [Why Northern EU After Property](MODULE_09_GTM.md#why-northern-eu-after-property)
  - [The Northern EU Landscape](MODULE_09_GTM.md#the-northern-eu-landscape)
  - [Germany: The Prize](MODULE_09_GTM.md#germany-the-prize)
  - [Markets with Convention-Like Systems (Partial Wedge)](MODULE_09_GTM.md#markets-with-convention-like-systems-partial-wedge)
  - [Markets Without Convention Systems (General Decision Engine Sell)](MODULE_09_GTM.md#markets-without-convention-systems-general-decision-engine-sell)
  - [Northern EU Property Opportunity](MODULE_09_GTM.md#northern-eu-property-opportunity)
  - [Phase 4 Target](MODULE_09_GTM.md#phase-4-target)
- [9.6 Phase 5: US Mid-market](MODULE_09_GTM.md#96-phase-5-us-mid-market)
  - [Why US Last](MODULE_09_GTM.md#why-us-last)
  - [The US Challenges](MODULE_09_GTM.md#the-us-challenges)
  - [Why US Property First (Not Auto)](MODULE_09_GTM.md#why-us-property-first-not-auto)
  - [The TPA Channel](MODULE_09_GTM.md#the-tpa-channel)
  - [Named US Mid-Market Targets](MODULE_09_GTM.md#named-us-mid-market-targets)
  - [The US Sell: General Decision Engine](MODULE_09_GTM.md#the-us-sell-general-decision-engine)
  - [Phase 5 Target](MODULE_09_GTM.md#phase-5-target)
- [9.7 Why Motor + Property Together](MODULE_09_GTM.md#97-why-motor--property-together)
  - [The Structural Argument](MODULE_09_GTM.md#the-structural-argument)
  - [The Persona Argument](MODULE_09_GTM.md#the-persona-argument)
  - [The Buyer Argument](MODULE_09_GTM.md#the-buyer-argument)
- [9.8 Why EU Then US](MODULE_09_GTM.md#98-why-eu-then-us)
  - [The Convention System Wedge](MODULE_09_GTM.md#the-convention-system-wedge)
  - [The Fragmented Mid-Market](MODULE_09_GTM.md#the-fragmented-mid-market)
  - [The "Pay First, Recover Later" Architecture](MODULE_09_GTM.md#the-pay-first-recover-later-architecture)
  - [The Design Partner Advantage](MODULE_09_GTM.md#the-design-partner-advantage)
  - [EU Revenue Pays for US Entry](MODULE_09_GTM.md#eu-revenue-pays-for-us-entry)
- [9.9 Pricing & Channel](MODULE_09_GTM.md#99-pricing--channel)
  - [Pricing Philosophy](MODULE_09_GTM.md#pricing-philosophy)
  - [Pricing Tiers (Anchored to Caravela Economics)](MODULE_09_GTM.md#pricing-tiers-anchored-to-caravela-economics)
  - [US-Specific Pricing](MODULE_09_GTM.md#us-specific-pricing)
  - [Channel Strategy](MODULE_09_GTM.md#channel-strategy)
  - [Revenue Model Summary](MODULE_09_GTM.md#revenue-model-summary)
- [Sources](MODULE_09_GTM.md#sources)

---

### Module 10: Business Model & Unit Economics
[MODULE_10_BUSINESS.md](MODULE_10_BUSINESS.md)

- [10.1 Revenue Stream: Decision Engine (Primary)](MODULE_10_BUSINESS.md#101-revenue-stream-decision-engine-primary)
  - [Revenue Model: Dual Pricing](MODULE_10_BUSINESS.md#revenue-model-dual-pricing)
  - [What the Decision Engine Includes](MODULE_10_BUSINESS.md#what-the-decision-engine-includes)
- [10.2 Revenue Stream: Intake & Document Processing (Secondary)](MODULE_10_BUSINESS.md#102-revenue-stream-intake--document-processing-secondary)
  - [Why Intake Is a Revenue Stream (Not Just a Feature)](MODULE_10_BUSINESS.md#why-intake-is-a-revenue-stream-not-just-a-feature)
  - [Intake Pricing: Two Buyer Types](MODULE_10_BUSINESS.md#intake-pricing-two-buyer-types)
  - [Cost to Deliver](MODULE_10_BUSINESS.md#cost-to-deliver)
- [10.3 Unit Economics: Per Adjuster](MODULE_10_BUSINESS.md#103-unit-economics-per-adjuster)
  - [Current State (Without Mysa)](MODULE_10_BUSINESS.md#current-state-without-mysa)
  - [With Mysa: 3x Productivity](MODULE_10_BUSINESS.md#with-mysa-3x-productivity)
  - [Per-Adjuster Savings Calculation](MODULE_10_BUSINESS.md#per-adjuster-savings-calculation)
  - [For a Mid-Tier TPA (200 Adjusters)](MODULE_10_BUSINESS.md#for-a-mid-tier-tpa-200-adjusters)
- [10.4 Unit Economics: Per Carrier](MODULE_10_BUSINESS.md#104-unit-economics-per-carrier)
  - [STP (Straight-Through Processing) Improvement](MODULE_10_BUSINESS.md#stp-straight-through-processing-improvement)
  - [ACV by Carrier Tier](MODULE_10_BUSINESS.md#acv-by-carrier-tier)
  - [Combined ROI: Caravela-Tier Carrier](MODULE_10_BUSINESS.md#combined-roi-caravela-tier-carrier)
- [10.5 Pricing Tiers](MODULE_10_BUSINESS.md#105-pricing-tiers)
  - [Tier Summary](MODULE_10_BUSINESS.md#tier-summary)
  - [Design Partner Pricing](MODULE_10_BUSINESS.md#design-partner-pricing)
  - [Pricing as % of GWP](MODULE_10_BUSINESS.md#pricing-as--of-gwp)
  - [Per-Claim Pricing: When to Lead With It](MODULE_10_BUSINESS.md#per-claim-pricing-when-to-lead-with-it)
  - [Revenue Expansion: Property Upsell](MODULE_10_BUSINESS.md#revenue-expansion-property-upsell)
- [10.6 Financial Projections](MODULE_10_BUSINESS.md#106-financial-projections)
  - [[REQUIRES FOUNDER INPUT]](MODULE_10_BUSINESS.md#requires-founder-input)
- [10.7 Fundraising Plan](MODULE_10_BUSINESS.md#107-fundraising-plan)
  - [[REQUIRES FOUNDER INPUT]](MODULE_10_BUSINESS.md#requires-founder-input-1)
- [Key Numbers Summary (For Pitch Deck)](MODULE_10_BUSINESS.md#key-numbers-summary-for-pitch-deck)
- [Sources](MODULE_10_BUSINESS.md#sources)

---

### Module 11: Risk & Regulatory
[MODULE_11_RISK.md](MODULE_11_RISK.md)

- [11.1 Competitive Risks](MODULE_11_RISK.md#111-competitive-risks)
  - [Verisk / XactAI -- Existential Risk (2-3 Year Horizon)](MODULE_11_RISK.md#verisk--xactai--existential-risk-2-3-year-horizon)
  - [Shift Technology -- EU Threat (12-18 Month Horizon)](MODULE_11_RISK.md#shift-technology--eu-threat-12-18-month-horizon)
  - [Five Sigma / Clive -- Direct Competitor (Now)](MODULE_11_RISK.md#five-sigma--clive--direct-competitor-now)
  - [CCC + EvolutionIQ -- Adjacent Threat (2-3 Year Horizon)](MODULE_11_RISK.md#ccc--evolutioniq--adjacent-threat-2-3-year-horizon)
  - [Wamy -- Unknown Threat (Emerging)](MODULE_11_RISK.md#wamy--unknown-threat-emerging)
- [11.2 Technical Risks](MODULE_11_RISK.md#112-technical-risks)
  - [OCR Accuracy Ceiling](MODULE_11_RISK.md#ocr-accuracy-ceiling)
  - [Coverage Determination Reliability](MODULE_11_RISK.md#coverage-determination-reliability)
  - [Convention System Complexity Across Countries](MODULE_11_RISK.md#convention-system-complexity-across-countries)
  - [LLM Hallucination Risk in Legal/Financial Decisions](MODULE_11_RISK.md#llm-hallucination-risk-in-legalfinancial-decisions)
- [11.3 Market Risks](MODULE_11_RISK.md#113-market-risks)
  - [Mid-Market Budget Constraints](MODULE_11_RISK.md#mid-market-budget-constraints)
  - [Long Sales Cycles Even for Mid-Market](MODULE_11_RISK.md#long-sales-cycles-even-for-mid-market)
  - [Carrier Consolidation](MODULE_11_RISK.md#carrier-consolidation)
  - [Economic Downturn Reducing Claims Spend](MODULE_11_RISK.md#economic-downturn-reducing-claims-spend)
  - [Concentration Risk -- Caravela as Only Design Partner](MODULE_11_RISK.md#concentration-risk--caravela-as-only-design-partner)
- [11.4 Regulatory: EU](MODULE_11_RISK.md#114-regulatory-eu)
  - [GDPR Article 22 -- Automated Decision-Making](MODULE_11_RISK.md#gdpr-article-22--automated-decision-making)
  - [EU AI Act -- High-Risk Classification](MODULE_11_RISK.md#eu-ai-act--high-risk-classification)
  - [Per-Country Insurance Regulators](MODULE_11_RISK.md#per-country-insurance-regulators)
  - [Data Residency](MODULE_11_RISK.md#data-residency)
- [11.5 Regulatory: US](MODULE_11_RISK.md#115-regulatory-us)
  - [State-by-State Insurance Regulation](MODULE_11_RISK.md#state-by-state-insurance-regulation)
  - [Data Privacy Laws](MODULE_11_RISK.md#data-privacy-laws)
  - ["Deny Then Defend" Legal Framework](MODULE_11_RISK.md#deny-then-defend-legal-framework)
  - [How US Differs from EU Approach](MODULE_11_RISK.md#how-us-differs-from-eu-approach)
- [11.6 Operational Risks](MODULE_11_RISK.md#116-operational-risks)
  - [Key-Person Risk -- 2 Founders](MODULE_11_RISK.md#key-person-risk--2-founders)
  - [Caravela Dependency -- Design Partner Concentration](MODULE_11_RISK.md#caravela-dependency--design-partner-concentration)
  - [Talent Acquisition in EU](MODULE_11_RISK.md#talent-acquisition-in-eu)
  - [Burn Rate Management Pre-Revenue](MODULE_11_RISK.md#burn-rate-management-pre-revenue)
- [11.7 Mitigation Strategies](MODULE_11_RISK.md#117-mitigation-strategies)
  - [Competitive Risk Mitigations](MODULE_11_RISK.md#competitive-risk-mitigations)
  - [Technical Risk Mitigations](MODULE_11_RISK.md#technical-risk-mitigations)
  - [Market Risk Mitigations](MODULE_11_RISK.md#market-risk-mitigations)
  - [Regulatory Risk Mitigations (EU)](MODULE_11_RISK.md#regulatory-risk-mitigations-eu)
  - [Regulatory Risk Mitigations (US)](MODULE_11_RISK.md#regulatory-risk-mitigations-us)
  - [Operational Risk Mitigations](MODULE_11_RISK.md#operational-risk-mitigations)
- [Sources](MODULE_11_RISK.md#sources)

---

## Cross-Reference Index

Key topics and where they are discussed across the FOS:

| Topic | Modules | Key Sections |
|-------|---------|-------------|
| **Convention systems** (IDS, IRSA, CARD, CIDE) | 2, 3, 5, 7, 8, 9 | 2.4 STP Reality Gap; 3.1 Phase 3 (Claim Triggering); 5.2 Unoccupied Territory; 5.9 Layer 3 Moat; 7.5 Convention Matching Engine; 8.2 Stage 1; 9.2-9.3 Phases 1-2 |
| **STP (straight-through processing)** | 2, 3, 4, 8, 10 | 2.4 STP Reality Gap; 3.1 Phase 5; 4.8 TAM Calculations; 8.2 Stage 5 (Near-STP); 10.4 STP Improvement |
| **Chrome Extension / "Clippy"** | 1, 6, 7 | 1.6 Product Now; 6.5 The "Clippy" Architecture; 7.7 Agentic Approach for Locked Systems |
| **Decision ground truth** | 1, 5, 8 | 1.4 Core Value Proposition; 5.2 Decision Ground Truth; 5.9 Layer 1 Moat; 8.1 Data Moat Thesis; 8.4 Annotation as Product |
| **Caravela Seguros** (design partner) | 4, 7, 8, 9, 10, 11 | 4.5 Caravela Tier Sweet Spot; 7.2 Current Stack; 8.4 Quality Flywheel; 9.2 Phase 1 Portugal; 10.4 Combined ROI; 11.6 Caravela Dependency |
| **SOP workflow engine** | 1, 5, 6, 8 | 1.6 Product Now; 5.2 SOP-Driven Workflows; 6.3 SOP-Driven Workflow Engine; 8.2 Stage 1 |
| **EU AI Act** | 6, 7, 8, 11 | 6.8 Human-in-the-Loop; 7.9 EU AI Act; 8.5 EU AI Act Compliance; 11.4 High-Risk Classification |
| **Workforce crisis** | 1, 2 | 1.4 Value Stack; 2.3 The Workforce Crisis |
| **Flywheel / data compounding** | 1, 3, 6, 8 | 1.6 Product Tomorrow; 3.8 The Flywheel; 6.4 The Core Loop; 8.2 Flywheel Mechanics; 8.7 Network Effects |
| **GDPR** | 7, 8, 11 | 7.9 GDPR; 8.5 GDPR Compliance for Training Data; 11.4 GDPR Article 22 |
| **OCR / document processing** | 7, 8 | 7.4 OCR & Document Processing; 8.4(d) Quality Flywheel |
| **Human-in-the-loop** | 6, 7, 11 | 6.8 Human-in-the-Loop: Why; 7.9 EU AI Act; 11.4 GDPR Article 22 |
| **Reserve accuracy** | 2, 3, 6 | 2.6 Reserve = P&L Impact; 3.4 Sub-Step 5: Reserve Calculation; 6.2 Sub-Step 5 |
| **Property claims** | 3, 4, 5, 9 | 3.3 Home/Property Claims; 4.7 Motor + Property Overlap; 5.8 Property Claims AI Gap; 9.4 Phase 3 Property |
| **The 6 decision sub-steps** | 3, 6 | 3.4 The 6 Decision Sub-Steps; 6.2 The 6 Decision Sub-Steps |
| **Verisk / XactAI threat** | 5, 11 | 5.4 Verisk / XactAI; 11.1 Verisk Existential Risk |
| **Shift Technology threat** | 5, 11 | 5.5 Shift Technology; 11.1 Shift EU Threat |
| **Mid-market vs enterprise** | 4, 8, 9 | 4.4 Why Bottom-Up; 4.6 Mid-Market vs Small; 8.6 Different Data Needs; 9.1 Rollout Order |
| **Pricing model** | 9, 10 | 9.9 Pricing & Channel; 10.1-10.5 Revenue Streams and Pricing Tiers |
| **TAM / market sizing** | 4, 10 | 4.8 TAM Calculations; 10.7 Fundraising Plan |
| **EAS (European Accident Statement)** | 3, 6, 7 | 3.1 Phase 2 Documentation; 6.9 Demo 1 EU Motor; 7.4 OCR |
| **Personas / ICP** | 1, 3, 6 | 1.2 ICP Deep Dive; 1.3 All Personas; 3.6 All Personas and Their Roles; 6.6 All Personas |
| **Subrogation** | 3 | 3.1 Phase 6 Triage; 3.1 Phase 7 Investigation |
| **Fraud detection / SIU** | 3, 5, 6 | 3.4 Sub-Step 6; 5.1 Fraud Detection (Crowded Zone); 6.2 Sub-Step 6 |
| **Bad faith liability** | 3, 11 | 3.1 Phase 7 Investigation; 11.5 "Deny Then Defend" |
| **Data residency** | 7, 8, 11 | 7.9 Data Residency Architecture; 8.5 Legal Framework; 11.4 Data Residency |
| **Annotation / training data** | 7, 8 | 7.4 Benchmark System; 8.4 Annotation as Product & Strategic Asset |
| **Broker channel** | 3, 6, 9 | 3.1 Phase 4 First Contact; 6.10 Demo Spec: Broker Flow; 9.9 Channel Strategy |

---

## Glossary of Insurance Terms

Terms are listed alphabetically. Where an abbreviation is used throughout the FOS, the abbreviation is the primary entry.

| Term | Definition |
|------|-----------|
| **ACORD** | Association for Cooperative Operations Research and Development. US industry standard for insurance data exchange formats. No EU equivalent exists -- each EU insurer has its own intake forms and data fields. |
| **ACV (Annual Contract Value)** | The annualized revenue from a single customer contract. Used throughout the FOS to express Mysa's pricing per carrier. Not to be confused with "actual cash value" (a property claims term for replacement cost minus depreciation). |
| **Adjuster** | The insurance professional who investigates, evaluates, and settles claims. "Desk adjuster" handles claims remotely; "field adjuster" inspects damage on-site. In the EU, often called a "claims handler." |
| **ARR (Annual Recurring Revenue)** | Total annualized recurring subscription revenue. The standard SaaS growth metric. |
| **ASF** | Autoridade de Supervisao de Seguros e Fundos de Pensoes. Portugal's insurance regulator. |
| **Authority limit** | The maximum claim value an adjuster can approve without supervisor sign-off. Varies by carrier, adjuster seniority, and claim type. Claims exceeding the authority limit are escalated, adding days to cycle time. |
| **Bad faith** | A legal doctrine (primarily US) where an insurer can be sued for unreasonably denying, delaying, or undervaluing a claim. Creates significant litigation risk and is a major driver of claims process rigor. |
| **Bancassurance** | Insurance products sold through bank distribution channels. Common in Southern EU (5-8% of non-life). The policyholder may contact the bank first when filing a claim, adding an intermediary step. |
| **Bareme** | A standardized scale or table used in convention systems (especially France's IRSA) to determine fault allocation percentages based on accident circumstances. |
| **BI (Bodily Injury)** | A claim involving physical injury to a person, as opposed to property damage only. BI claims are significantly more complex, longer in duration (weeks to years vs. days), and higher in value. They often involve medical records, treatment analysis, and pain-and-suffering calculations. |
| **CARD (Convenzione tra Assicuratori per il Risarcimento Diretto)** | Italy's convention system for direct motor claims settlement. Mandatory for two-vehicle accidents involving material damage and minor bodily injury (permanent disability of 9% or less). Uses flat-rate inter-insurer reimbursement adjusted annually. |
| **Carrier** | An insurance company that underwrites policies and assumes financial risk. Distinguished from brokers (who sell policies) and TPAs (who process claims on behalf of carriers). |
| **Cat / Nat Cat (Catastrophe / Natural Catastrophe)** | Large-scale insured events such as hurricanes, floods, earthquakes, and wildfires. These events cause massive spikes in claims volume and severity, overwhelming normal claims operations. |
| **CCR (Caisse Centrale de Reassurance)** | France's state reinsurer for natural catastrophe risk under the Cat-Nat regime. |
| **CCS (Consorcio de Compensacion de Seguros)** | Spain's state reinsurer for catastrophe risk. |
| **CIDE (Convenio de Indemnizacion Directa)** | Spain's convention system for direct motor claims settlement. Also known as ASCIDE. Covers material damage only (not bodily injury). Mandatory since July 2016. Uses flat-rate inter-insurer reimbursement. |
| **CIMPAS** | Portugal's digital platform for managing convention-based motor claims under the IDS system. The electronic clearinghouse through which insurers submit, match, and settle convention claims. |
| **Claims decision engine** | Mysa's self-defined product category. Unlike a CMS (which tracks what happened) or a copilot (which assists with admin), a decision engine helps adjusters determine what to decide by applying carrier-specific rules, convention logic, and historical patterns. |
| **CMS (Claims Management System)** | The core software system carriers use to track claims -- opening files, logging activities, managing documents, and recording outcomes. Examples: Guidewire ClaimCenter, Duck Creek Claims, Five Sigma. Analogous to a CRM for sales teams. Tracks status and history but does not help with decision-making. |
| **CNIL** | Commission Nationale de l'Informatique et des Libertes. France's data protection authority, the strictest in the EU. Requires Data Protection Impact Assessments before deployment and has aggressive enforcement. |
| **CNPD** | Comissao Nacional de Protecao de Dados. Portugal's data protection authority. Less prescriptive than France's CNIL but GDPR applies equally. |
| **Colossus** | A proprietary bodily injury claims valuation tool (owned by Verisk) used by many US carriers to calculate settlement ranges for BI claims. Controversial but widely adopted. |
| **Combined ratio** | An insurer's total expenses (claims paid + operating costs) divided by premiums earned. A combined ratio below 100% means the insurer is profitable on its underwriting. |
| **Convention system** | A standardized inter-insurer protocol used in several EU countries for settling motor claims between two insurers. The policyholder's own insurer pays the claim directly (direct settlement), then recovers from the at-fault insurer's company through an inter-insurer clearinghouse at a pre-agreed flat rate (forfait). Examples: IDS (Portugal), IRSA (France), CARD (Italy), CIDE (Spain). |
| **Coverage determination** | The process of verifying whether a reported loss is covered under the policyholder's specific policy. Involves checking policy terms, exclusions, endorsements, effective dates, named drivers, and deductibles. One of Mysa's 6 decision sub-steps and a major area with almost zero AI competition. |
| **Deductible** | The amount the policyholder must pay out of pocket before insurance coverage kicks in. Called "excess" in UK/EU markets. |
| **DPA (Data Processing Agreement)** | A legally binding contract between a data controller (the carrier) and a data processor (Mysa) that specifies how personal data will be handled, stored, and protected. Required under GDPR Article 28. |
| **DWP (Direct Written Premiums)** | The US equivalent of GWP. Total premiums written directly by an insurer, excluding assumed reinsurance. The standard measure of insurer size in the US. |
| **EAS (European Accident Statement)** | A pan-EU standardized carbon-copy form filled collaboratively by both drivers at the scene of a motor accident. Contains vehicle diagrams, checkboxes for accident circumstances, a sketch, and signatures from both parties. Approximately 50% are still filled on paper. The EAS is the single most important document in European motor claims -- it serves as the primary legal statement and maps directly to convention fault tables. |
| **EU AI Act (Regulation 2024/1689)** | The European Union's comprehensive AI regulation. Insurance claims AI likely classifies as "high-risk" under Annex III, requiring conformity assessment, human oversight, technical documentation, transparency obligations, and ongoing monitoring. Full enforcement begins August 2026. |
| **FNOL (First Notice of Loss)** | The initial report a policyholder makes to their insurer that an incident occurred. Not the full claim -- it is the trigger that opens a claim file. Can arrive via phone, app, email, broker submission, or walk-in. |
| **Forfait** | A pre-agreed flat rate used in convention systems for inter-insurer reimbursement. Instead of reimbursing actual claim costs, the at-fault insurer's company pays a standardized amount through the clearinghouse. This simplifies settlement but means the paying insurer sometimes over-pays and sometimes under-pays relative to actual costs. |
| **FRISS** | A Dutch insurtech focused on real-time fraud, risk, and compliance detection for P&C insurers. Often integrated into carrier workflows alongside or in place of SIU for automated fraud scoring. |
| **GDPR (General Data Protection Regulation)** | The EU's comprehensive data privacy regulation. Article 22 specifically restricts fully automated decision-making that produces legal effects, which is why Mysa's human-in-the-loop design is both a product choice and a regulatory requirement. |
| **GWP (Gross Written Premiums)** | The total premium income an insurer writes in a period, before reinsurance deductions. The standard measure of insurer size in the EU. Mysa's target segment is carriers with EUR 100-200M GWP ("Caravela tier"). |
| **Guidewire** | The dominant enterprise claims management system vendor for large insurers. Guidewire ClaimCenter is the most widely deployed CMS globally. Integration with Guidewire requires long partnership negotiations, making it a barrier for startups. Mysa's Chrome extension strategy bypasses this barrier. |
| **ICD-10** | International Classification of Diseases, 10th Revision. A standardized coding system (~78,000 codes) used to classify medical diagnoses and procedures. Relevant in BI claims for parsing medical records and treatment costs. |
| **IDS (Indemnizacao Directa ao Segurado)** | Portugal's convention system for direct motor claims settlement. Uses flat-rate forfait reimbursement for material damage claims with clear liability. Administered through the CIMPAS digital platform. |
| **Indemnity** | The principle of restoring the policyholder to their financial position before the loss -- no more, no less. The insurer pays what is owed under the policy terms, not more (which would be unjust enrichment) and not less (which could constitute bad faith). |
| **IRSA (Indemnisation directe de l'assure et Recours entre Societes d'Assurance)** | France's convention system for direct motor claims settlement. Uses 13 standard fault scenarios with proportional fault allocation based on a bareme scale. Simpler than Portugal's IDS but serves a much larger market. |
| **IVASS** | Istituto per la Vigilanza sulle Assicurazioni. Italy's insurance regulator. Only 38 companies write RC Auto (motor liability) in Italy. |
| **Leakage** | Money lost by the insurer through overpayment, missed subrogation recovery, or process inefficiency. Industry estimates suggest 5-10% leakage on claims costs. Reducing leakage is a major ROI argument for claims technology. |
| **LLM (Large Language Model)** | The AI foundation (e.g., Google Gemini, Anthropic Claude) that powers Mysa's document understanding, reasoning, and recommendation capabilities. Mysa uses LLMs for OCR, policy parsing, and decision support -- but does not feed carrier data back to LLM providers. |
| **Loss ratio** | Claims costs (losses incurred) divided by premiums earned. A key profitability metric for insurers. A lower loss ratio means the insurer is paying out less relative to what it collects. |
| **MGA (Managing General Agent)** | An intermediary with underwriting authority granted by a carrier. MGAs increasingly handle claims administration as well. They are a potential buyer segment for Mysa, particularly in the US. |
| **NAIC (National Association of Insurance Commissioners)** | The US organization of state insurance regulators. Publishes insurer financial data, complaint ratios, and market share data used for carrier segmentation and market intelligence. |
| **OCR (Optical Character Recognition)** | Technology that converts images of text (handwritten or printed) into machine-readable data. Central to Mysa's intake pipeline -- converting paper EAS forms, invoices, and other claim documents into structured data. Mysa's Caravela OCR engine currently achieves 81.5% normalized accuracy. |
| **P&C (Property and Casualty)** | The insurance category covering motor, home/property, commercial, and liability lines. Distinguished from life insurance and health insurance. All of Mysa's target market falls within P&C. |
| **PD (Property Damage)** | Damage to physical property (vehicles, buildings, contents) as opposed to bodily injury. PD claims are generally simpler, faster, and lower-value than BI claims. In motor claims, "PD-only" means no injuries were reported. |
| **PHI (Protected Health Information)** | Medical and health data subject to special privacy protections. Relevant in BI claims that involve medical records, treatment histories, and injury assessments. Subject to GDPR Article 9 (EU) and HIPAA (US). |
| **PII (Personally Identifiable Information)** | Data that can identify an individual: names, addresses, policy numbers, license plates, phone numbers. Claims data is heavily laden with PII, making data privacy a first-order concern for any claims technology vendor. |
| **Policyholder** | The person or entity who owns the insurance policy. In motor claims, typically the vehicle owner/driver. In property claims, the homeowner. Distinguished from the claimant (who may be a third party making a claim against the policyholder's policy). |
| **Proof of loss** | A formal, sworn document submitted by the policyholder to the insurer detailing the claimed loss. Required in the US (especially for property claims) but not standard in EU motor claims, where the EAS serves a similar function. |
| **Reserve** | The amount of money an insurer sets aside (holds in reserve) to pay a specific claim. Set when a claim is opened and adjusted as new information arrives. Reserves directly impact the insurer's financial statements -- inaccurate reserves (too high or too low) distort P&L, affect regulatory capital requirements, and can trigger supervisory action. Reserve accuracy is a CFO-level concern. |
| **SaaS (Software as a Service)** | Cloud-delivered subscription software. Mysa's business model is SaaS with dual pricing: per-claim fees (landing) plus platform license (expansion). |
| **SIU (Special Investigations Unit)** | The internal department at an insurance carrier responsible for investigating suspected fraud. Claims flagged by fraud scoring systems (FRISS, Shift) or adjuster judgment are referred to SIU. Only approximately 5% of claims trigger SIU investigation. |
| **SNCU** | Small Non-Complex Undertaking. An EIOPA (European Insurance and Occupational Pensions Authority) classification for smaller insurers, typically those with under EUR 100M GWP. Approximately 13% of Solvency II entities qualify. |
| **Solvency II** | The EU's regulatory framework for insurance companies, setting capital requirements, risk management standards, and reporting obligations. All EU insurers must comply. |
| **SOP (Standard Operating Procedure)** | The carrier-specific rules, workflows, and decision guidelines that adjusters follow when processing claims. Every carrier has different SOPs, even for the same claim type. Mysa encodes these SOPs into its workflow engine, creating carrier-specific decision logic and a major source of lock-in. |
| **STP (Straight-Through Processing)** | Claims resolved near-instantly with minimal or no human review, typically via convention system automation. Convention systems promise 60-70% STP rates but deliver approximately 10% in practice because of poor input data quality. Closing this gap is a core part of Mysa's value proposition. |
| **Subrogation** | The insurer's right to recover claim payments from the party at fault (or their insurer). In convention systems, subrogation is handled automatically through forfait reimbursement. In non-convention claims, missed subrogation is a major source of leakage -- billions are lost industry-wide to missed recovery opportunities. |
| **Total loss** | When the cost to repair damaged property exceeds a threshold (typically 70-80% of the item's value), the insurer declares it a total loss and pays the full value rather than repairing it. Most common in motor claims with older or heavily damaged vehicles. |
| **TPA (Third-Party Administrator)** | A company that processes claims on behalf of insurance carriers who outsource their claims operations. TPAs are a significant buyer segment in the US, handling millions of claims annually. Major TPAs include Sedgwick, Crawford, and Gallagher Bassett. |

---

*This Table of Contents is a living document. As modules are updated, section headings and anchors should be verified.*

---

# Part 1: Deep Positioning & Company Identity

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

---

# Part 2: Problem Anatomy

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

---

# Part 3: The Claims Journey

# Module 3: The Claims Journey

**Status:** DRAFT v1.0
**Last updated:** February 9, 2026
**Feeds:** Demo narrative, product definition, domain credibility for investors, blog content, pitch deck slides 3-8, sales playbook, engineering requirements

---

> This is the largest and most domain-deep module in the Founding Operating System. It maps every phase of a motor and property insurance claim from the moment an accident happens to the day the file closes -- across both European and American markets. It documents what adjusters do, how long it takes, where the pain is, who the competitors are, and where Mysa fits. If Mysa's credibility claim is "we understand claims better than anyone," this module is the proof.

---

## 3.1 Motor Claims EU: Full Lifecycle (Phases 0-11)

European motor claims follow a convention-based system unique in global insurance. Two drivers fill out a joint accident form at the scene, and a network of pre-agreed inter-insurer rules determines fault. This creates structurally cleaner data than the US adversarial model -- but the data quality at intake remains the bottleneck blocking straight-through processing.

### Phase 0: The Incident (Seconds 0-60)

**Description:** "Pure Chaos, Not Paperwork." The driver is in shock or adrenaline mode. Nobody is filling out an accident report in the first minute. Real sequence: Am I hurt? Are my passengers hurt? Is the car in a dangerous position? [SOURCE: claims_journey_discovery.md, lines 62-78]

| Dimension | Detail |
|-----------|--------|
| **Duration** | Seconds 0-60 |
| **Adjuster involvement** | None |
| **Documents generated** | None (dashcam footage auto-records if present; telematics ping on connected car policies) |
| **Decision forks** | None |
| **EU-specific** | Emergency services via 112 |
| **Automation status** | Telematics crash notification is the only automation at this phase |

**Pain points:** Shock and adrenaline impair rational decision-making. Safety concerns override documentation concerns. No rational assessment yet. [SOURCE: claims_journey_discovery.md, lines 68-72]

---

### Phase 1: Scene Management (Minutes 1-30)

**Description:** The first critical fork. If anyone is injured, police and ambulance take over scene documentation. Otherwise, two drivers manage information exchange and documentation. [SOURCE: claims_journey_discovery.md, lines 81-133]

| Dimension | Detail |
|-----------|--------|
| **Duration** | Minutes 1-30 post-incident |
| **Adjuster involvement** | None -- still at scene |
| **Key document** | European Accident Statement (EAS) -- a pan-EU standardized carbon-copy form, filled collaboratively by both drivers, signed by both at scene |
| **EAS completion time** | 15-30 minutes post-incident |
| **EAS paper rate** | ~50% still filled on paper (remainder digital via insurer apps) |

**Decision Forks at Scene:**

| Fork | Question | Paths |
|------|----------|-------|
| **F1: Injuries?** | Is anyone injured? | YES: Police/ambulance called. Bodily injury (BI) claim path -- higher complexity, longer lifecycle, lawyers. NO: Material damage only, proceed to F2 |
| **F2: Cooperation?** | Is the other party cooperative? | B1 (Cooperative): Drivers fill EAS together, both sign. B2 (Uncooperative): No joint statement -- claim becomes much harder. Police called. B3 (Hit & Run): Other party flees. No counter-party info. Guarantee fund path |

[SOURCE: claims_journey_discovery.md, lines 83-126]

**Pain points:**
- EAS is a paper carbon-copy form, often with illegible handwriting [SOURCE: claims_journey_discovery.md, line 164]
- Diagram is often unclear or messy [SOURCE: claims_journey_discovery.md, line 165]
- Language barriers for tourists and cross-border accidents [SOURCE: claims_journey_discovery.md, line 166]
- Multi-vehicle accidents: form designed for 2 parties only [SOURCE: claims_journey_discovery.md, line 167]
- ~50% still paper, requiring manual digitization by insurer [SOURCE: claims_journey_discovery.md, line 168]

**Documents generated at scene:** Photos of damage, driver IDs exchanged, insurance cards captured, witness contact info, EAS (signed by both drivers -- each takes a copy), police report (if police called).

---

### Phase 2: Documentation -- The EU Advantage

**Description:** How accident data is captured and structured. This phase defines the entire downstream data quality. [SOURCE: claims_journey_discovery.md, lines 136-205]

| Dimension | Detail |
|-----------|--------|
| **Duration** | Minutes 30+ post-incident |
| **Adjuster involvement** | None -- still pre-claims |
| **Key mechanism** | EAS produces structurally cleaner input data than competing US narratives |
| **EAS manual digitization** | 30-60 minutes per form if paper |

**The European Accident Statement (EAS):**

The EAS is the single most important document in European motor claims. It is a pan-EU standardized form with:
- Checkboxes for circumstances (which vehicle was doing what)
- A collision diagram (hand-drawn by drivers)
- Driver and vehicle details for both parties
- Insurance information for both parties
- Signatures from both drivers

> "Despite being paper-based, [the EAS] produces structurally better data for a 'data normalization layer' platform." [SOURCE: claims_journey_discovery.md, lines 192-193]

**Product implication:** The European model, despite being paper-based, produces structurally better data than the US model. The US model requires more AI interpretation and conflict resolution. This is a key reason -- beyond licensing -- why Europe is the better starting market for Mysa. [SOURCE: claims_journey_discovery.md, lines 192-194]

---

### Phase 3: Claim Triggering and Reconciliation

**Description:** How insurers receive notice of the claim and reconcile data. This is where the EU convention system enters the picture. [SOURCE: claims_journey_discovery.md, lines 208-379]

| Dimension | Detail |
|-----------|--------|
| **Duration** | Hours to days after incident (can extend weeks if disputed) |
| **Adjuster involvement** | Limited -- claims handler may do reconciliation |
| **EU convention fault determination** | 5-10 minutes for clean EAS |
| **Convention auto-processing** | Mostly automatic for clean cases |

**EU Convention Systems:**

Convention systems are pre-agreed inter-insurer protocols that determine fault using standardized lookup tables. They are the backbone of European motor claims processing.

| Country | Convention System | How It Works |
|---------|------------------|--------------|
| **Portugal** | CIMPAS / IDS (Indemnizacao Directa ao Segurado) | Flat-rate forfait reimbursement. Material damage with clear liability only |
| **France** | IRSA (Indemnisation directe de l'assure et Recours entre Societes d'Assurance) | 13 standard fault scenarios. Proportional to fault per bareme scale |
| **Italy** | CARD (Convenzione tra Assicuratori per il Risarcimento Diretto) | Flat rate, adjusted annually. Two-vehicle accidents, material damage + minor BI (permanent disability <=9%) |
| **Spain** | CIDE / ASCIDE (Convenio de Indemnizacion Directa) | Flat rate, material damage only. Mandatory since July 2016 |
| **Germany** | No direct settlement convention | Traditional adversarial liability system. Each claim settled individually |
| **Netherlands** | Bilateral insurer agreements | Negotiated per agreement |
| **Belgium** | RDR (Reglement Direct) | Convention-based system |

[SOURCE: claims_journey_discovery.md, lines 214-219; extraction output Phases 9-11, lines 7766-7807]

**Convention flow (clean EAS path):**

```
Both drivers submit signed EAS to their own insurer
        |
Convention system matches EAS checkboxes to fault table
        |
Fault determined (e.g., 100/0, 50/50, 80/20)
        |
Each insurer pays their own policyholder (direct settlement)
        |
Inter-insurer reimbursement via clearing house at forfait rate
        |
Monthly net settlement between all member insurers
```

**When the convention path breaks down** (20-30% of claims):
- EAS incomplete or incorrectly filled
- One party refuses to sign
- Parties disagree after the fact
- Multi-vehicle accidents
- No EAS filled at scene

These fall back to police report + individual investigation -- expensive, slow, and human-intensive. [SOURCE: claims_journey_discovery.md, lines 301-320]

**The STP Reality:**
- Convention systems handle ~70-80% of claims [SOURCE: claims_journey_discovery.md, line 320]
- But actual STP is only ~10% [SOURCE: claims_journey_discovery.md, lines 320-321]
- Bottleneck: getting clean data TO the lookup, not the lookup itself

---

### Phase 4: First Contact

**Description:** The moment the policyholder contacts someone -- insurer, broker, or agent -- to report the claim. This is where the intermediary channel matters. [SOURCE: claims_journey_discovery.md, lines 384-934]

| Dimension | Detail |
|-----------|--------|
| **Duration** | Hours 0-24 after incident |
| **EU adjuster involvement** | LOW -- call center/front office handles FNOL capture |
| **EU time per claim** | 5-15 minutes |

**Three Paths to Claim Initiation:**

| Path | How It Works | Prevalence |
|------|-------------|------------|
| **Direct to insurer** | Policyholder calls hotline, app, or branch. Most common for direct-purchased policies | Growing at ~5% CAGR |
| **Through a broker** | Broker receives panic call, triages, may file FNOL on behalf. Represents CLIENT, not insurer | Common in UK (54%), Netherlands (60%), Belgium (61%) |
| **Through an agent** | Captive agents can open claims directly. Independent agents more limited | Italy 80%+, Germany 60%+, Portugal 50%+ |
| **Bancassurance (EU-specific)** | Policy sold through bank. Policyholder may call bank first, redirected to insurer | ~5-8% non-life |

[SOURCE: claims_journey_discovery.md, lines 386-463]

**EU Distribution Channel Breakdown (Non-Life Motor, 2024):**

| Channel | EU Average | Key Markets |
|---------|-----------|-------------|
| **Agents (tied + independent)** | ~55-58% | Italy 80%+, Germany 60%+, Portugal 50%+, Spain ~45% |
| **Brokers** | ~25-30% | UK 54%, Netherlands 60%, Belgium 61% |
| **Direct (online + call center)** | ~19% | Growing. Netherlands, Finland, Croatia higher |
| **Bancassurance** | ~5-8% (non-life) | Minimal for motor. Huge for life |

[SOURCE: claims_journey_discovery.md, lines 437-463]

**Adjuster Activities at First Contact (EU):**

| # | Activity | Time | Pain Point |
|---|----------|------|------------|
| 1 | Receive claim assignment | 1-2 min | May sit in queue for hours if manual |
| 2 | Review FNOL data and check EAS completeness | 3-5 min | Data often incomplete, poorly structured |
| 3 | Verify policy coverage | 2-5 min | Requires checking separate policy admin system |
| 4 | Set initial reserve (often formula-based for routine PD) | 2-5 min | Too low = reserve inadequacy; too high = unnecessary capital |
| 5 | Plan first outbound contact (only if EAS incomplete) | 2-3 min | Only ~30-40% of claims require adjuster outreach |
| 6 | Make first outbound call (if required) | 5-15 min | Voicemail, wrong numbers, language barriers |
| 7 | Log all actions in CMS | 3-5 min | Manual data entry. Some adjusters spend more time logging than investigating |

[SOURCE: claims_journey_discovery.md, lines 1555-1566]

**Key EU insight:** For clean EAS claims, the adjuster often does NOT contact the driver at all. The EAS is the statement. This is fundamentally different from the US, where the adjuster contacts the driver for a formal recorded statement on ~95% of claims.

| EU Claim Path | Insurer Contacts Driver? | % of Claims |
|---------------|-------------------------|-------------|
| Clean EAS -- both signed, matches convention | NO -- EAS is legally sufficient | ~60-70% theoretical, ~10% actual STP |
| Incomplete/unclear EAS | YES -- clarification only | ~15-20% |
| No EAS / disputed / BI / high value | YES -- formal investigation | ~10-15% |
| Suspected fraud | YES -- full SIU investigation | ~5% |

[SOURCE: claims_journey_discovery.md, lines 330-335]

---

### Phase 5: FNOL (First Notice of Loss)

**Definition:** FNOL is the initial report a policyholder makes to their insurer that an incident occurred. It is NOT the full claim -- it is the trigger that opens a claim file. [SOURCE: claims_journey_discovery.md, lines 938-1122]

| | FNOL | Formal Claim / Proof of Loss |
|---|------|------------------------------|
| **When** | Immediately after incident | Later, once fully documented |
| **Purpose** | Alert insurer, open file | Formally request payment |
| **Detail level** | Basic -- what happened, when, where | Detailed -- full documentation, sworn statement |
| **Format** | Phone call, app, email, web form | Often formal signed document |

[SOURCE: claims_journey_discovery.md, lines 944-951]

**EU FNOL Flow (Clean EAS Path):**

```
Policyholder calls insurer (or broker submits)
     |
"I had an accident. Policy number: X. I have my EAS."
     |
Front office / call center agent:
|-- Verifies policy is active
|-- Receives EAS (scan, photo, digital submission)
|-- Opens claim file
|-- Logs basic info
     |
NO CALL TO ADJUSTER for ~10% actual STP
     |
EAS goes to claims handler who:
|-- Matches EAS to convention fault tables
|-- If clean match -> straight-through processing
|-- If unclear -> THEN contact driver for clarification
```

[SOURCE: claims_journey_discovery.md, lines 1031-1050]

**EU Adjuster Activities at FNOL:**

| # | Activity | Time | Pain Point |
|---|----------|------|------------|
| 1 | Validate FNOL completeness | 3-5 min | 30-50% of FNOLs incomplete |
| 2 | Process EAS / intake documents (OCR paper EAS, interpret handwriting, re-key data) | 5-15 min | Paper EAS is #1 bottleneck. Handwriting illegibility, torn forms |
| 3 | Request missing documents | 5-10 min | Response time unpredictable. Claim stalls until docs arrive |
| 4 | Enter/validate data in CMS | 5-15 min | Manual data entry. Average 15+ clicks per FNOL in legacy systems |
| 5 | Set/update reserves | 2-5 min | Over-reserving ties up capital; under-reserving triggers regulatory flags |
| 6 | Create claim diary/task list | 2-3 min | Easy to forget with 100+ open claims |

[SOURCE: claims_journey_discovery.md, lines 1613-1626]

**Total EU FNOL time:** 5-10 min (clean EAS); 20-40 min (incomplete EAS)

**No EU equivalent to ACORD:** Each EU insurer has their own FNOL intake forms, claims management systems, and data fields. The EAS standardizes scene documentation but not the FNOL itself. This creates a product opportunity for a data normalization layer that takes any input (EAS scan, email, phone transcript) and outputs structured data for any insurer's system. [SOURCE: claims_journey_discovery.md, lines 1003-1019]

---

### Phase 6: Triage (Hours 1-48)

**Description:** Evaluate claim complexity, confirm or adjust routing, set investigation plan. Often concurrent with FNOL processing. [SOURCE: claims_journey_discovery.md, lines 1663-1734]

| Dimension | Detail |
|-----------|--------|
| **Duration** | Hours 1-48 after FNOL |
| **EU adjuster involvement** | LOW for routine (rules/convention auto-triage); HIGH for complex |
| **Time per claim** | 5-15 min (routine); 30-60 min (complex requiring supervisor) |

**Adjuster Activities at Triage:**

| # | Activity | Time | Pain Point |
|---|----------|------|------------|
| 1 | Review triage classification | 2-3 min | Auto-triage often wrong. 20-30% override rate |
| 2 | Assess claim complexity (simple PD, complex PD, BI, total loss, multi-party, litigated?) | 3-5 min | Complexity is spectrum, not binary |
| 3 | Check for coverage issues | 3-5 min | Coverage denials contentious, must document |
| 4 | Identify subrogation potential | 2-3 min | Convention may flag automatically. Billions lost industry-wide to missed opportunities |
| 5 | Assess fraud indicators (review Shift/FRISS scores) | 2-5 min | False positives waste SIU resources |
| 6 | Set investigation plan | 3-5 min | "Orchestrator" moment -- plans downstream workflow |
| 7 | Request vendor services (if vehicle needs inspection) | 5-10 min | Manual phone/portal-based scheduling |
| 8 | Diary management | 2-3 min | With 100+ claims, critical to avoid stale claims |

[SOURCE: claims_journey_discovery.md, lines 1674-1685]

**The "Adjuster as Orchestrator" -- triage is where it starts.** At triage, the adjuster becomes a project manager, deciding WHO does WHAT and WHEN:
- Who inspects vehicle? Self (field), DRP body shop, independent appraiser, virtual (Snapsheet/Tractable)
- Who handles rental car? Enterprise/Hertz partnership, direct pay, reimburse policyholder
- Who determines liability? Self, supervisor, convention system
- Who handles BI? Self (if dual-licensed), transfer to BI unit, outside counsel
- Who investigates fraud? Self (basic verification) or SIU (formal investigation)

[SOURCE: claims_journey_discovery.md, lines 1687-1697]

**Triage Automation (Current State):**

| Automation | Adoption | Impact |
|-----------|----------|--------|
| Rules-based auto-triage (severity, type, location) | ~60% of mid-large insurers | Eliminates supervisor manual routing for 70-80% |
| AI/ML complexity scoring | ~15-20% (growing fast) | More accurate; predicts litigation, severity, fraud |
| Automated fraud scoring at triage (Shift, FRISS) | ~30% | Real-time fraud flags before adjuster touches |
| Auto-reserve setting | ~20% | Formula-based eliminates manual estimation |
| Automated subrogation identification (CCC, CLARA) | ~15% | AI identifies recovery at FNOL/triage, not weeks later |

[SOURCE: claims_journey_discovery.md, lines 1699-1707]

**Handoff Points:**

| From | To | When | Why |
|------|-----|------|-----|
| Auto-triage | PD desk adjuster | Simple, clear-fault PD claim | Routine handling path |
| Auto-triage | BI specialist | Injuries reported | Requires medical knowledge |
| Auto-triage | Total loss desk | Vehicle likely totaled | Specialized workflow |
| Auto-triage | SIU | High fraud score (>70) | Formal investigation |
| Auto-triage | Litigation handler | Attorney letter received | Different rules and timelines |
| PD adjuster | Catastrophe team | CAT event declared | Surge protocols, field deployment |
| Auto-triage | STP engine | Clean, low-complexity, no fraud flags | Straight-through processing |

[SOURCE: claims_journey_discovery.md, lines 1722-1732]

---

### Phase 7: Investigation (Days 1-30 for PD; Weeks 1-26+ for BI)

**Description:** The core of what adjusters DO. Gather evidence, determine liability, identify all parties, coordinate vendor activities. [SOURCE: claims_journey_discovery.md, lines 1736-1821]

| Dimension | Detail |
|-----------|--------|
| **Adjuster involvement** | HIGH -- this is the core adjuster phase |
| **Simple PD duration** | 1-3 hours total |
| **Complex PD duration** | 5-15 hours |
| **BI duration** | 20-100+ hours over months |

**Adjuster Activities at Investigation (13 tasks):**

| # | Activity | Time | EU Handler | Pain Point |
|---|----------|------|------------|------------|
| 1 | **Take recorded statements** | 15-30 min per party | Rare for routine PD (EAS serves as statement). Common for disputes, BI | Phone tag: avg 2.7 attempts per party. Can consume 30-40% of investigation time |
| 2 | **Review police report** | 10-20 min | If available (~20-30% of claims) | Quality varies wildly |
| 3 | **Analyze scene photos/video** | 10-30 min | Review policyholder photos, compare to EAS diagram | Poor quality, wrong angles, insufficient coverage |
| 4 | **Match to convention scenario** | 5-10 min | Core EU handler activity. Match EAS checkboxes to IRSA/IDA/IDS fault table | ~40% need human interpretation beyond lookup |
| 5 | **Determine liability** | 15-60 min | For non-convention cases: review all evidence, assign fault % | Most contentious step |
| 6 | **Coverage analysis** | 10-30 min | For edge cases (excluded drivers, lapsed coverage, commercial use) | Denials trigger complaints, lawsuits, bad faith |
| 7 | **Contact witnesses** | 10-20 min per witness | Rare for routine PD | Hard to reach and reluctant |
| 8 | **Order/review medical records (BI)** | 30-60 min per cycle | Review medical reports from treating doctors | Most time-consuming document type |
| 9 | **Coordinate with legal (litigated)** | 15-30 min per interaction | If attorney involved | All communication through counsel |
| 10 | **Cross-reference databases** | 5-10 min | Check internal history | Multiple systems to check |
| 11 | **Request additional evidence** | 5-15 min per request | Supplemental photos, repair shop reports, telematics | Each request = wait cycle |
| 12 | **Document EVERYTHING** | Ongoing (3-5 min per entry) | Log every action, call, finding | Per 10 min investigation, 5-10 min documentation |
| 13 | **Supervisor review / authority escalation** | 10-20 min | If reserve exceeds authority | Delays claims by days |

[SOURCE: claims_journey_discovery.md, lines 1747-1763]

**The Orchestration View:**

```
                         ADJUSTER (Orchestrator)
                               |
       +-----------+-----------+-----------+-----------+
       |           |           |           |           |
   Body Shop   Appraiser   Medical    Attorney    SIU
   (estimate)  (inspection) (records)  (legal)   (fraud)
       |           |           |           |           |
   Rental Car   Tow Company  Pharmacy   Court      Police
   (logistics)  (salvage)    (bills)    (filing)   (report)
```

The adjuster's VALUE is in knowing what to ask for, when, from whom, and how to interpret what comes back. The adjuster's PAIN is that coordinating all these parties is manual, phone/email-based, and asynchronous. [SOURCE: claims_journey_discovery.md, lines 1765-1781]

**Investigation Automation (Current State):**

| Automation | Adoption | Impact |
|-----------|----------|--------|
| AI fraud detection (real-time scoring) | ~30% of insurers | Shift: >99% accuracy |
| Automated statement transcription | ~5-10% (emerging) | Accuracy issues remain |
| Digital evidence collection (photo upload) | ~30-40% | Policyholder submits via app |
| Automated police report retrieval | ~20% | LexisNexis, Verisk pull electronically |
| AI-assisted liability determination | ~5% (very emerging) | Tools suggest liability; adjuster confirms |
| Telematics data integration | ~10% of policies | Speed, braking, impact severity data |

[SOURCE: claims_journey_discovery.md, lines 1783-1792]

---

### Phase 8: Assessment (Days 3-30 for PD; Weeks 4-52+ for BI)

**Description:** Review damage estimates, determine repair vs total loss, validate medical expenses (BI), set final reserves. [SOURCE: claims_journey_discovery.md, lines 1825-1922]

| Dimension | Detail |
|-----------|--------|
| **Adjuster involvement** | HIGH -- reviews and validates vendor/tool assessments |
| **Simple PD duration** | 30-60 min |
| **Complex PD duration** | 2-5 hours |
| **Total loss duration** | 1-3 hours |
| **BI duration** | 10-40+ hours over months |

**Adjuster Activities at Assessment (12 tasks):**

| # | Activity | Time | Pain Point |
|---|----------|------|------------|
| 1 | Review repair estimate (body shop, appraiser, or AI tool) | 15-30 min | May include inflated labor, miss hidden damage |
| 2 | Negotiate estimate with body shop | 15-30 min per supplement | Supplements (additional damage during repair) avg 1.3 per claim |
| 3 | Determine repair vs total loss | 10-20 min | Threshold varies by country |
| 4 | Calculate Actual Cash Value (ACV) for total loss | 30-60 min | Finding accurate comparables hard for older/rare vehicles |
| 5 | Review medical records/bills (BI) | 30-120 min per cycle | Records arrive in batches over months |
| 6 | Calculate BI damages | 30-60 min | Internal guidelines, severity tables |
| 7 | Assess diminished value (where applicable) | 15-30 min | Less common in EU |
| 8 | Calculate loss of use / rental | 10-15 min | Rental costs escalate when repairs delayed |
| 9 | Review salvage value (total loss) | 10-15 min | Salvage market fluctuates |
| 10 | Set/update final reserves | 5-15 min | Reserve accuracy is KPI |
| 11 | Request Independent Medical Exam (BI disputes) | 15-30 min to arrange | Scheduling takes weeks |
| 12 | Document assessment rationale | 10-20 min | Every number must be defensible |

[SOURCE: claims_journey_discovery.md, lines 1836-1851]

**Repair vs Total Loss Decision:**

```
DAMAGE ESTIMATE RECEIVED
        |
COMPARE: Repair Cost vs ACV
        |
+-- Repair Cost < Threshold --> REPAIRABLE
|   +-- Authorize repair
|   +-- Monitor supplements
|   +-- Manage rental duration
|
+-- Repair Cost >= Threshold --> TOTAL LOSS
|   +-- Calculate ACV (comparables, condition adjustments)
|   +-- Deduct salvage value
|   +-- Present offer to policyholder
|   +-- Process title transfer, salvage disposition
|
+-- BORDERLINE --> Adjuster judgment
    +-- Consider: age, mileage, safety (structural damage?)
    +-- Customer preference
    +-- Escalate to supervisor if uncertain

EU: Typically 60-70% of vehicle value threshold (varies by country/insurer)
```

[SOURCE: claims_journey_discovery.md, lines 1853-1885]

**Assessment Automation (Current State):**

| Automation | Adoption | Impact |
|-----------|----------|--------|
| AI photo-based estimates (CCC, Tractable, Audatex) | ~20-30% of eligible claims | Generates line-level estimates in seconds |
| Automated total loss valuation (CCC Valuescope, Mitchell) | ~60% of total loss claims | ACV calculation automated; adjuster reviews |
| AI-assisted BI valuation (Colossus, Claims Outcome Advisor) | ~70% of US insurers | Constrains settlement range |
| Digital supplement workflow | ~30-40% of DRP claims | Auto-approval for under-threshold items |
| Salvage auction integration (Copart, IAA) | ~50-60% of total loss | Direct feed for salvage valuation |

[SOURCE: claims_journey_discovery.md, lines 1887-1895]

---

### Phase 9: Decision

**Description:** The pivotal phase where coverage and liability determinations are converted into actions -- approve, deny, or settle. The output determines whether the claim flows to settlement (Phase 10) or closure without payment (Phase 11). [SOURCE: claims_journey_discovery.md, lines ~2019-2025]

**11 Core Adjuster Decision Activities:**

1. Coverage validation -- confirm policy applies
2. Liability determination -- fault allocation (EU convention or adversarial)
3. Damage valuation -- translate estimate to reserve
4. Reserve setting -- appropriate to phase and peril
5. Negotiation authority check -- within limits?
6. Authority escalation (if needed) -- route to supervisor
7. Decision -- approve, deny, escalate to litigation
8. Recommendation documentation -- file notes with reasoning
9. STP routing (if eligible) -- claims that can auto-approve
10. Complex claim routing -- litigation, attorney, multi-party
11. Denial reasoning (if denying) -- policy justification

[SOURCE: extraction output Phases 9-11, lines 19-30]

This phase is covered in full detail in Section 3.4: The 6 Decision Sub-Steps.

---

### Phase 10: Settlement

**Description:** The execution phase where approved decisions are converted into actual payments. [SOURCE: claims_journey_discovery.md, lines 7507-7516]

**Key finding:** In the EU convention-based system, settlement for material damages can be near-automatic once the decision phase completes. [SOURCE: extraction output Phases 9-11, line 41]

**EU Settlement Sub-Phases:**

1. **Offer generation** -- calculate settlement amount from decision outputs
2. **Offer communication** -- present to policyholder
3. **Negotiation** (minimal for convention material damage -- convention bareme determines amounts)
4. **Authorization** -- payment approved within authority matrix
5. **Payment execution** -- SEPA transfer (1 business day; SEPA Instant: 10 seconds)
6. **Documentation** -- settlement recorded
7. **Convention reimbursement** -- inter-insurer clearing house processes forfait

[SOURCE: claims_journey_discovery.md, lines 7519-7526]

**EU Convention Settlement Flow (e.g., CARD/Italy):**

```
1. Policyholder claims to own insurer (Insurer A)
2. Insurer A settles with policyholder (30 days with EAS, 60 without; 15 days to pay)
3. Insurer A sends reimbursement claim to CONSAP clearing house
4. CONSAP calculates monthly net positions across all member insurers
5. Monthly batch settlement between insurers at forfait rate
```

[SOURCE: extraction output Phases 9-11, lines 303-309]

**Regulatory Settlement Timelines (EU):**

| Country | Make Offer/Decision | Pay After Agreement |
|---------|--------------------|--------------------|
| **Italy** (with EAS) | 30 days | 15 days |
| **Italy** (no EAS) | 60 days | 15 days |
| **Italy** (BI) | 90 days | 15 days |
| **France** | 3 months (BI: 8 months from accident) | 1 month |
| **Spain** | 3 months (material) | Immediate upon acceptance |
| **Germany** | Reasonable time (no statutory deadline) | Prompt |

[SOURCE: extraction output Phases 9-11, lines 361-374]

**EU Convention Forfait Dynamic:**

The convention forfait system means the insurer who paid the claimant may NOT recover the actual amount paid -- they recover a standardized flat rate. If actual claim cost exceeds the forfait, the insurer absorbs the difference. If the actual cost is below the forfait, the insurer profits on that claim. Understanding this dynamic is critical for any platform operating in EU motor claims. [SOURCE: extraction output Phases 9-11, lines 944-945]

---

### Phase 11: Closure

**Description:** The final administrative phase. All payments finalized, reserves zeroed, file closed. In practice, closure is rarely clean. [SOURCE: claims_journey_discovery.md, lines 8500-8519]

**The Closure Sequence:**

1. All indemnity and expense payments finalized
2. All recovery actions completed or assigned (subrogation, salvage)
3. Settlement agreement signed (if applicable)
4. Reserves reduced to zero (or to expected recovery amount)
5. All litigation resolved or transferred
6. SIU investigation cleared (if referred)
7. Convention settlement completed via clearing house
8. Reinsurance notification sent (if above treaty threshold)
9. Quality documentation check -- file completeness verified
10. Financial reconciliation -- paid vs reserved variance captured
11. File status changed to "Closed" in CMS
12. Post-closure triggers: regulatory reporting, underwriting feedback, NPS survey, audit queue

[SOURCE: extraction output Phases 9-11, lines 716-729]

**EU-Specific Closure:**
- Convention settlement confirmation via IDA/IRSA/CIDE/CIMPAS
- Green Card bureau notification if cross-border claim
- EU Motor Insurance Directive: reasoned offer within 3 months of claim presentation
- GDPR data retention: typically 5-10 years post-closure depending on jurisdiction

[SOURCE: extraction output Phases 9-11, lines 773-777]

**Closure Metrics (Industry Benchmarks):**

| Metric | Industry Average | Best-in-Class |
|--------|-----------------|---------------|
| Average cycle time FNOL to closure (PD) | 30-45 days | 15-25 days |
| Average cycle time FNOL to closure (BI) | 180-365 days | 90-180 days |
| Reopening rate | 5-12% overall | <5% |
| Reserve accuracy (within 10% of final paid) | 60-70% | >80% |
| Claims leakage rate | 5-10% | <3% |
| Quality audit score | 75-85/100 | >90/100 |
| NPS at closure | 23-35 | >60 |
| Cost per claim (closure admin) | $150-300 | <$100 |

[SOURCE: extraction output Phases 9-11, lines 1069-1083]

---

### EU Phases 0-11 Summary Table

| Phase | Duration | Adjuster Role | Adjuster Time | STP Possible? | Key Pain Points |
|-------|----------|---------------|---------------|---------------|-----------------|
| 0: Incident | Seconds 0-60 | None | -- | -- | Shock, no documentation |
| 1: Scene Management | Minutes 1-30 | None | -- | EAS filled (50% paper) | Paper EAS messy; language barriers |
| 2: Documentation | Minutes 30+ | None | -- | Standardized EAS | EU: handwriting illegibility |
| 3: Reconciliation | Hours-Days | Passive | -- | Convention lookup | 10% STP actual vs 60-70% theoretical |
| 4: First Contact | Hours 0-24 | LOW | 5-15 min | Yes if clean EAS | Phone tag; incomplete FNOL |
| 5: FNOL | Hours 0-48 | MODERATE | 5-40 min | ~10% if clean EAS | Paper EAS; missing docs |
| 6: Triage | Hours 1-48 | LOW-HIGH | 5-60 min | Auto-triage | 20-30% override rate |
| 7: Investigation | Days 1-30 (PD) | HIGH | 1-15 hrs | No | Phone tag; documentation burden |
| 8: Assessment | Days 3-30 (PD) | HIGH | 0.5-5 hrs | Partial | Estimate negotiation; supplements |
| 9: Decision | Overlaps 7-8 | HIGH | Varies | STP for clean claims | Authority escalation delays |
| 10: Settlement | Days-Weeks | MODERATE | Varies | Convention near-automatic | Forfait mismatch; payment timing |
| 11: Closure | Days post-settlement | LOW | Administrative | Automated for clean | Zombie claims; reopening rate |

[SOURCE: Compiled from claims_journey_discovery.md phases 0-11; extraction outputs Phases 0-5, 6-8, 9-11]

---

## 3.2 Motor Claims US: Full Lifecycle (Phases 0-11)

US motor claims follow a fundamentally different model. There is no joint accident form, no convention system, and fault is determined through adversarial investigation. Every claim requires more human investigation time than the EU equivalent.

### How the US Differs From EU -- Phase by Phase

**Phase 0-1: Incident and Scene**

The scene management phase diverges immediately:

| Dimension | EU | US |
|-----------|----|----|
| **Joint form** | YES -- EAS filled by both drivers | NO -- each driver independent |
| **Police involvement** | Only if injuries, dispute, or driver requests | Much more frequent -- legally required above $500-$1,000 threshold (varies by state) |
| **Who documents** | Two drivers collaboratively fill EAS | Police officer files crash report; drivers file separately |
| **Data source** | Single agreed document signed by both | Two separate (potentially conflicting) accounts + police report |
| **Emergency services** | 112 | 911 |

[SOURCE: claims_journey_discovery.md, lines 180-204]

**Phase 2: Documentation -- Competing Narratives**

The US produces "two separate, potentially conflicting accounts" rather than a single agreed document. This creates fundamentally different downstream challenges. [SOURCE: claims_journey_discovery.md, lines 178, 193-194]

| Dimension | EU | US |
|-----------|----|----|
| **Standardized joint form** | YES -- EAS, pan-EU standardized | NO -- no equivalent |
| **Structured data** | YES -- checkboxes, standard fields | NO -- mostly narrative text in police reports |
| **Source of truth** | Single agreed document | Two separate accounts + police report |
| **Data flow** | One form to each insurer | Police report + Driver A account to Insurer A; Driver B account to Insurer B |

[SOURCE: claims_journey_discovery.md, lines 180-189]

**Phase 3: Claim Triggering -- The US Adversarial Model**

There is NO convention system. Instead:

| Choice | How It Works | Tradeoff |
|--------|-------------|----------|
| **First-party claim** (file with own insurer) | Faster. Customer relationship. Pay deductible upfront (recover later through subrogation) | Policyholder pays deductible |
| **Third-party claim** (file with other driver's insurer) | No deductible. But much slower -- insurer has zero obligation to rush | Very slow |
| **Both simultaneously** | Smart drivers file both -- fast service from own + establish claim with at-fault | Most thorough |

[SOURCE: claims_journey_discovery.md, lines 225-240]

**Critical Fork F6: No-Fault vs At-Fault States**

| System | States | How It Works |
|--------|--------|-------------|
| **No-Fault** (~12 states) | Michigan, Florida, New York, New Jersey, Pennsylvania, etc. | Each driver files with OWN insurer for medical/injury (PIP coverage). Fault barely matters for medical piece. Property damage still follows fault. Litigation only for serious injuries above threshold |
| **At-Fault** (majority) | Texas, California, Georgia, Ohio, etc. | At-fault driver's insurer pays everything. Fault determination is the entire game. Litigation much more common |

[SOURCE: claims_journey_discovery.md, lines 241-256]

**US Liability Investigation Steps:**
1. Gather all data (police crash report, driver A recorded statement, driver B recorded statement, photos, dashcam, witnesses, telematics)
2. Reconstruct what happened (physical evidence, contradictions, cross-references)
3. Liability determination (fault percentage -- not binary, can be 80/20, 70/30, 50/50)
   - Comparative negligence (most states): Both drivers share fault, payout adjusts proportionally
   - Contributory negligence (few states: VA, MD, NC, DC, AL): If found even 1% at fault, recover NOTHING
4. Inter-company arbitration if insurers disagree (via Arbitration Forums, Inc. -- binding decision)

[SOURCE: claims_journey_discovery.md, lines 261-288]

**Phase 4-5: First Contact and FNOL -- The Adjuster-Heavy Model**

US FNOL Flow:

```
Policyholder calls insurer (or broker submits basic info)
     |
Call center agent collects:
|-- Policy number
|-- Basic incident info (date, time, location)
|-- Other party info
|-- Police report number
     |
Claim file opened
     |
THEN adjuster calls back (often same day or next)
     |
Adjuster conducts RECORDED STATEMENT (15-30 min):
|-- Walk me through what happened
|-- What were you doing before the accident?
|-- What did you see?
|-- Where exactly were you hit?
|-- Who said what?
|-- Any witnesses?
|-- Any injuries?
     |
Adjuster ALSO calls OTHER driver for their statement
     |
Adjuster reconstructs incident from competing accounts
```

[SOURCE: claims_journey_discovery.md, lines 1052-1079]

**Up to 4 recorded statements for a single fender bender:**

| Step | What Happens | Time |
|------|-------------|------|
| Insurer A calls Driver A | Formal recorded statement | 15-30 min |
| Insurer A attempts to reach Driver B | Get other party's version | 15-30 min (if cooperative) |
| Insurer B calls Driver B | Their own recorded statement | 15-30 min |
| Insurer B attempts to reach Driver A | Get other party's version | 15-30 min (if cooperative) |

[SOURCE: claims_journey_discovery.md, line 350]

**US Adjuster Activities at FNOL (9 tasks):**

| # | Activity | Time | Pain Point |
|---|----------|------|------------|
| 1 | Validate FNOL completeness | 3-5 min | 30-50% incomplete |
| 2 | Conduct recorded statement (insured) | 15-30 min | Most time-consuming per-claim activity. Phone tag adds 2-3 attempts |
| 3 | Contact other party for recorded statement | 15-30 min | Other party has no obligation. May take days/weeks |
| 4 | Request missing documents | 5-10 min | Claim stalls until docs arrive |
| 5 | Retrieve police report | 5-10 min | ~60-70% of claims. Costs $5-$15, takes 5-14 days |
| 6 | Enter/validate data in CMS | 5-15 min | 15+ clicks per FNOL in legacy systems |
| 7 | Set/update reserves | 2-5 min | Authority limits apply ($5K-$25K for new adjusters) |
| 8 | Create claim diary | 2-3 min | Critical with 100+ open claims |
| 9 | Request additional evidence (photos, dashcam, telematics) | 5-15 min | Each request = wait cycle |

[SOURCE: claims_journey_discovery.md, lines 1613-1626]

**Total US FNOL time:** 30-60 min (includes recorded statement)

**Phase 6-8: Triage, Investigation, Assessment**

US triage, investigation, and assessment follow the same structure as EU (see Phase 6-8 in Section 3.1) but with consistently higher adjuster time investment:

**Human Time Per Routine Claim -- The Cost Gap:**

| | EU (clean EAS path) | US (standard path) |
|---|---------------------|-------------------|
| Driver contacted post-incident? | Often NO | Almost always YES |
| Form of contact | Clarification call/email if needed | Formal recorded statement (15-30 min) |
| Adjuster time per claim | Minutes (review EAS, match to convention) | 30-60+ minutes per driver per insurer |
| Human hours for routine claim | Low | High even for simple claims |

[SOURCE: claims_journey_discovery.md, lines 352-360]

**Phase 9: Decision**

US decisions carry more complexity because:
- Comparative negligence systems require percentage-based fault allocation (not binary)
- State-by-state rules create 50+ regulatory frameworks
- No convention lookup tables -- liability is human judgment
- Authority matrices are typically more layered (see Section 3.7)

**Phase 10: Settlement -- The Adversarial System**

US settlement absorbs 62% of total claims lifecycle time due to negotiation cycles. [SOURCE: extraction output Phases 9-11, line 41]

| Settlement Type | Negotiation Likelihood | Duration |
|----------------|----------------------|----------|
| First-party material (simple) | Low (10-20%) | 1-2 rounds, 1-2 weeks |
| First-party material (total loss) | Medium (30-40%) | 2-4 rounds, 2-4 weeks |
| Third-party material | Medium (30-40%) | 2-5 rounds, 2-8 weeks |
| Bodily injury | High (80-90%) | 3-8 rounds, 3-18 months |
| Subrogation (inter-insurer) | Medium (30%) | 1-3 rounds, 1-6 months |

[SOURCE: extraction output Phases 9-11, lines 500-508]

**US BI Negotiation Cycle:**
1. Attorney sends demand letter (high anchor -- typically 3-5x expected settlement)
2. Insurer counteroffer at 20-40% of demand
3. Attorney provides additional documentation
4. Insurer revises offer upward (10-30% increase)
5. Back-and-forth narrows gap over 3-8 rounds
6. Agreement typically reached at 50-70% of initial demand
7. If no agreement: mediation, arbitration, or litigation

[SOURCE: extraction output Phases 9-11, lines 513-519]

**US Regulatory Settlement Timelines:**

| State | Acknowledge Claim | Accept/Reject | Pay After Agreement |
|-------|------------------|---------------|---------------------|
| California | 15 days | 40 days | 30 days |
| Texas | 15 days | 30 days | 5 business days |
| North Carolina | 30 days | 30 days | 10 days |
| Florida | 14 days | 90 days (total) | 20 days |
| New York | 15 days | 30 days | 5 business days |

[SOURCE: extraction output Phases 9-11, lines 361-374]

**US Authority Matrix:**

| Role | Material Damage | BI Authority | Total Loss |
|------|----------------|--------------|------------|
| Junior Adjuster | Up to $5,000 | Up to $5,000 | N/A (refer up) |
| Experienced Adjuster | Up to $15,000-$25,000 | Up to $15,000 | Up to $15,000 |
| Senior Adjuster | Up to $50,000 | Up to $50,000 | Up to $50,000 |
| Supervisor | Up to $100,000 | Up to $100,000 | Up to $100,000 |
| Claims Manager | Up to $250,000 | Up to $250,000 | Up to $250,000 |
| Regional VP of Claims | Up to $500,000 | Up to $500,000 | Up to $500,000 |
| Claims Committee | Above $500,000 | Above $500,000 | Above $500,000 |

[SOURCE: extraction output Phases 9-11, lines 536-545]

**US Total Loss Thresholds (by state):**
- 75% of ACV: Most common (CO, CT, FL, GA, IL, IN, KY, etc.)
- 70% of ACV: AL, DC, MD, SC
- 80% of ACV: NV, NM, OK
- 100% of ACV / Total Loss Formula: CA, HI, KS, MI, OH, TX, WV, etc.
- No statutory threshold: a few states leave to insurer discretion

[SOURCE: claims_journey_discovery.md, lines 1853-1885]

**Phase 11: Closure**

US closure includes:
- Release of all claims form is standard -- near-universal, especially for BI
- State-specific closing requirements (e.g., California requires written notice of claim closure)
- Unfair Claims Settlement Practices Act compliance check
- 1099 tax form for BI settlements exceeding $600
- Medicare reporting (Section 111) for BI claims involving Medicare beneficiaries
- Subrogation recovery continues after policyholder considers claim "done"
- Reopening rate higher than EU: early settlement pressure leads to premature closure

[SOURCE: extraction output Phases 9-11, lines 749-782]

**US Payment Methods:**

| Method | Speed | Usage | Trend |
|--------|-------|-------|-------|
| Paper Check | 5-10 business days | ~30% (declining) | Federal mandate to move to EFT |
| ACH/EFT | 1-3 business days | ~40% | Growing rapidly |
| Wire Transfer | Same day | Large/urgent only | Stable |
| Virtual Credit Card | Instant | Growing for shop payments | Growing |
| Push-to-Debit | Instant (30 min) | Emerging | Lemonade, Hippo use this |
| Direct-to-Repair-Shop | N/A | ~40% of repairable | Stable |

[SOURCE: extraction output Phases 9-11, lines 473-483]

---

## 3.3 Home/Property Claims

Home and property claims are structurally different from motor -- no counterparty, no EAS, no convention system. Coverage determination is the core challenge. As the source document notes, "water damage is the fender bender of property."

### Why Property Claims Are Structurally Different

| Dimension | Motor Insurance | Home/Property Insurance |
|-----------|----------------|------------------------|
| **Counterparty?** | YES -- another driver, another insurer | Usually NO -- it's you vs. the peril |
| **Agreed document?** | EU: EAS -- both parties sign | NONE -- only your claim, your photos |
| **Fault question?** | WHO caused the accident? | WAS the peril covered? |
| **Convention/lookup system?** | EU: Yes -- IRSA/IDA fault tables | NONE -- coverage is policy interpretation |
| **STP possible?** | EU: ~10% actual, 60-70% theoretical | Very rare -- almost always needs inspection |
| **Adjuster involvement** | EU: Often NO for clean EAS path | Almost ALWAYS for non-trivial claims |

[SOURCE: claims_journey_discovery.md, lines 2349-2356]

### Home Insurance Claim Types (US Data, 2019-2023)

| Peril | % of Claims | Avg Claim Amount | Notes |
|-------|------------|-----------------|-------|
| **Wind and hail** | 42.5% | Varies by severity | ~1 in 36 insured homes per year |
| **Water damage and freezing** | 29.4% | ~$15,400 | Second most common. Often invisible (behind walls) |
| **Fire and lightning** | ~5% | Highest (often total loss) | Most severe |
| **Theft** | 0.7% | ~$5,524 | Least common |
| **Other (liability, etc.)** | ~22% | Varies | Includes personal liability |

[SOURCE: claims_journey_discovery.md, lines 2360-2366]

### Why Property Claims Almost ALWAYS Need an Adjuster

Motor (EU clean path): EAS says what happened, convention says who is at fault, damage is to a standardized asset, repair cost is estimable from photos and make/model.

Property: NO agreed document. Burden of proof is on the policyholder to show damage occurred, it was caused by a covered peril (not excluded), and the scope of loss matches the claim. Every home is unique. Contents are unknown. Hidden damage is common (water behind walls, mold, structural). [SOURCE: claims_journey_discovery.md, lines 2370-2386]

**Result:** ~100% of non-trivial home claims require adjuster inspection vs. ~10% STP for EU motor.

### Property Claims FNOL Flow

```
INCIDENT (water leak, fire, theft, storm)
         |
IMMEDIATE ACTIONS
|-- Mitigate further damage (turn off water, board up)
|-- Document BEFORE cleanup (photos, video)
|-- Police report (if theft/vandalism)
         |
FNOL to insurer (phone / app / web portal)
|-- Policy number, date, description
|-- NOT an agreed document -- just your report
         |
ADJUSTER ASSIGNED (almost always)
|-- Inspection scheduled (usually within 1 week)
|-- 1-2 hours on-site
|-- Documents everything, estimates costs
         |
PROOF OF LOSS
|-- Formal sworn statement
|-- Inventory of damaged/stolen items
|-- Supporting documentation (receipts, photos)
         |
COVERAGE DETERMINATION
|-- Was this peril covered?
|-- Any exclusions apply?
|-- Policy limits?
         |
SETTLEMENT
|-- May get partial payment upfront
|-- Replacement cost = two payments (ACV now, depreciation later)
|-- Complex claims (fire rebuild) can take MONTHS to YEARS
```

[SOURCE: claims_journey_discovery.md, lines 2394-2428]

### Documentation Burden Is MUCH Higher Than Motor

| Motor | Property |
|-------|----------|
| EAS + photos + police report (if applicable) | Photos/video of damage from multiple angles |
| | Inventory of damaged/stolen items with brand names, model numbers, original receipts, age and condition |
| | Police report (mandatory for theft) |
| | Proof of ownership for valuable items |
| | "Proof of loss" form (formal sworn statement) |

The inventory problem is brutal. After a fire or burglary, people have to remember and prove everything they owned. [SOURCE: claims_journey_discovery.md, lines 2441-2453]

### What a Property Adjuster Actually Does

**Part 1: Investigation -- Establishing the Facts**
- Inspect the damage (what happened, how bad is it)
- Determine causation (what caused it -- covered peril or not?)
- Document everything (photos, measurements, notes)
- Interview the policyholder and witnesses
- Review police reports (theft/vandalism)
- Detect fraud indicators

**Part 2: Valuation -- Estimating the Cost**
- Measure damaged areas
- Calculate repair/replacement costs using Xactimate (industry standard, 75-80% of adjusters)
- Assess repair vs replace
- Account for depreciation (ACV vs replacement cost)
- Review contractor estimates
- Negotiate settlement amounts

[SOURCE: claims_journey_discovery.md, lines 2461-2475]

### Property Field Adjuster Time Breakdown

| Activity | % of Time | Automation Potential |
|----------|----------|---------------------|
| **Travel to/from properties** | ~25-30% | HIGH -- eliminate with virtual inspection |
| **Documentation and data entry** | ~20-25% | HIGH -- auto-capture, voice-to-text, photo AI |
| **On-site inspection** | ~15-20% | MEDIUM -- remote video, 3D scanning |
| **Report writing** | ~10-15% | HIGH -- AI draft generation |
| **Xactimate/estimate creation** | ~10-15% | MEDIUM -- AI-assisted, but review needed |
| **Communication (calls, emails)** | ~10-15% | MEDIUM -- automated updates |
| **Collaboration/escalation** | ~5-10% | LOW -- human judgment needed |

[SOURCE: claims_journey_discovery.md, lines 2588-2596]

**Key finding:** "When a claim is assigned to an adjuster who needs help from a colleague, handling time nearly TRIPLES." [SOURCE: claims_journey_discovery.md, line 2598]

### EU vs US: No Structural Advantage for Property

Unlike motor, where EU convention systems create a structural advantage, property claims are effectively the same in both markets:
- No EAS equivalent
- No convention system
- No fault lookup tables
- The claim is between policyholder and insurer about whether a peril is covered
- **The 3x productivity opportunity applies equally to EU and US**

[SOURCE: claims_journey_discovery.md, lines 2575-2580]

| Aspect | US | EU |
|--------|----|----|
| **Insurer's inspector** | Claims Adjuster | Loss Adjuster |
| **Policyholder's advocate** | Public Adjuster | Loss Assessor |
| **Licensing** | State-specific, complex | More standardized within countries |
| **TPA usage** | Very common, especially for CAT | Common in UK, growing in continental EU |
| **Major TPAs** | Crawford, Sedgwick, Engle Martin | Crawford, Sedgwick, McLarens, Davies, Charles Taylor |
| **Estimating tool** | Xactimate (Verisk) -- 75-80% | Xactimate + country-specific tools |

[SOURCE: claims_journey_discovery.md, lines 2540-2555]

### The Hidden Damage Problem

Water damage (29.4% of claims) is often invisible:
- Mold growing behind walls
- Structural damage to joists
- Electrical damage from water infiltration

Photos do not show what is behind the drywall. This is why property claims resist full automation more than motor. [SOURCE: claims_journey_discovery.md, lines 2677-2682]

### The Fraud Challenge Is Getting Worse

> "Fraudsters can create fabricated property losses, complete with repair invoices, photos, estimates, and hotel bills using AI." -- Gen Re, January 2026 [SOURCE: claims_journey_discovery.md, line 2671]

### The Realistic Automation Opportunity

| | Can Automate | Can Augment | Still Needs Human |
|---|-------------|-------------|-------------------|
| FNOL intake | Yes | -- | -- |
| Document processing | Yes | -- | -- |
| Photo damage detection | Yes (visible) | -- | Hidden damage |
| Measurement/3D modeling | Yes | -- | -- |
| Repair cost estimation | -- | Draft for review | Final approval |
| Coverage determination | -- | Flag exclusions | Complex interpretation |
| Causation determination | -- | Suggest likely cause | Disputed/unclear |
| Fraud detection | -- | Flag for review | Investigation |
| Settlement negotiation | -- | -- | Human required |
| Large/complex claims | -- | Reduce adjuster time | Inspection needed |

[SOURCE: claims_journey_discovery.md, lines 2686-2698]

**The opportunity is not "replace the adjuster" -- it is "make the adjuster 3x more productive" and "eliminate field visits for claims that don't need them."** [SOURCE: claims_journey_discovery.md, line 2699]

---

## 3.4 The 6 Decision Sub-Steps

The decision phase is the highest-value, least-automated part of the claims process. It comprises 6 distinct expert judgment steps that together consume 60-70% of adjuster time. This is the layer that Mysa targets -- the space between intake (where data arrives) and settlement (where money moves).

### Sub-Step 1: Coverage Verification

**Question:** Does the policy cover this loss?

| Activity | Detail |
|----------|--------|
| Read policy document (often 40+ pages) | Check effective dates, named insured, covered perils, exclusions, endorsements |
| Verify policy was active at time of loss | Cross-reference policy admin system |
| Check for exclusions | Common: excluded drivers, commercial use, lapsed coverage, intentional acts |
| Confirm deductible | Which deductible applies (may vary by peril type in property) |
| Document coverage determination | Must be defensible -- coverage denials trigger complaints, lawsuits, bad faith allegations |

**EU:** Coverage verification is simpler for convention-eligible motor claims -- the convention handles inter-insurer settlement, and the policyholder's own insurer pays them. Coverage issues arise for edge cases.

**US:** More complex due to state-specific rules, endorsements, stacking (when multiple policies may apply). Coverage denials are a top source of bad faith litigation.

**Time:** 15-30 minutes for standard claims; longer for edge cases requiring underwriting consultation [SOURCE: MODULE_02_PROBLEM.md, step 3]

**Automation status:** ~40% of insurers have policy verification auto-check. LLMs can now read policies and flag exclusions -- this was impossible 3 years ago. [SOURCE: extraction output Phases 0-5, lines 431-436]

---

### Sub-Step 2: Liability Determination

**Question:** Who was at fault, and what percentage?

**EU (Convention):**
- Match EAS checkboxes to IRSA/IDA/IDS/CARD/CIDE fault table
- Clear matches: minutes. Ambiguous: human judgment needed (~40% need interpretation)
- Convention handles ~70-80% of motor claims
- For non-convention cases: review all evidence, assign fault %

**US (Adversarial):**
- Analyze recorded statements from both parties
- Review police report, photos, dashcam footage
- Physical evidence reconstruction
- Fault percentage -- not binary (can be 80/20, 70/30, 50/50)
- Comparative negligence (most states): both share fault proportionally
- Contributory negligence (VA, MD, NC, DC, AL): 1% at fault = recover nothing
- Inter-company arbitration via Arbitration Forums, Inc. if insurers disagree

**Time:** 5-10 minutes (EU convention match); 15-60 minutes (non-convention / US) [SOURCE: extraction output Phases 6-8, activity #4-5]

**Automation status:** ~5% of insurers use AI-assisted liability determination. Shift Technology claims 90% liability prediction accuracy. Five Sigma's Clive uses expert analysis and contextual reasoning. ZERO competitors automate EU convention matching. [SOURCE: extraction output Phases 6-8, lines 127-132]

---

### Sub-Step 3: Repair Assessment

**Question:** What does the damage cost to repair? Is it repairable, or is the vehicle/property a total loss?

| Activity | Motor | Property |
|----------|-------|----------|
| Review repair estimate | From body shop, independent appraiser, or AI tool (CCC/Tractable/Audatex) | Xactimate estimate from field/desk adjuster |
| Negotiate estimate | Challenge line items, approve supplements (avg 1.3 supplements per auto claim) | Review contractor estimates vs Xactimate |
| Repair vs total loss | Compare repair cost to ACV using state/country threshold | Compare repair cost to coverage limit |
| Hidden damage management | Supplement cycle: 50-90% of repairable auto claims have at least one | Water behind walls, mold, structural damage |

**Time:** 15-30 min per estimate review; 30-60 min for total loss ACV calculation [SOURCE: extraction output Phases 6-8, activities #1-4]

**The Supplement Cycle (Auto):**

The supplement cycle is the single largest source of settlement rework in auto claims. [SOURCE: extraction output Phases 9-11, lines 642-706]

- **Frequency:** 50-90% of repairable claims require at least one supplement
- **Average supplements per claim:** 1.5-2.5
- **Average supplement amount:** $800-$2,500 per supplement
- **DRP trusted shop approval:** Same day
- **Non-DRP shop approval:** 5-14 days (requires re-inspection)

**Automation status:** AI photo-based estimates at 20-30% adoption. Tractable generates repair-vs-total-loss decisions from photos alone. CCC generates line-level estimates in seconds. [SOURCE: extraction output Phases 6-8, lines 224-231]

---

### Sub-Step 4: Cost Analysis

**Question:** What is the total financial exposure?

This sub-step aggregates all cost components:
- Repair/replacement cost (from Sub-Step 3)
- Rental car / loss of use
- Medical costs (BI claims)
- Legal costs (if litigated)
- Salvage value deduction (total loss)
- Diminished value (where applicable)
- Subrogation potential (expected recovery from at-fault party)

**BI Valuation Methods:**
- **Multiplier method:** Total medical bills x multiplier (1.5-5.0 based on severity). Example: $20,000 medical bills x 3.0 = $60,000 demand
- **Per diem method:** Daily rate for pain/suffering x number of days affected
- **Software-based:** Colossus (Verisk): 750 injury codes, 10,720 value drivers. Used by 70%+ of US insurers. Claims Outcome Advisor (Mitchell)

[SOURCE: extraction output Phases 9-11, lines 438-442]

**Colossus -- The Dominant BI Tool (and Its Problems):**

Colossus has been the standard BI valuation tool since the late 1980s. It constrains adjuster negotiation authority to a settlement range. But:
- $1B+ class action for systematic undervaluation
- CSC executive testified system can be "tuned" to achieve target savings (e.g., 15% reduction)
- Designed for predictable BI patterns; nuclear verdicts ($10M+) grew 52% in 2024
- "Thermonuclear" verdicts ($100M+) increased 35%
- Social inflation has fundamentally altered the distribution

[SOURCE: claims_journey_discovery.md, lines 9903-9944]

**Time:** 10-30 minutes for standard cost aggregation; hours for complex BI [SOURCE: extraction output Phases 6-8, activities #6-8]

---

### Sub-Step 5: Reserve Calculation

**Question:** How much money should we set aside for this claim?

Reserves are money set aside for expected future claim payments. They hit the P&L immediately. [SOURCE: MODULE_01_POSITIONING.md, lines 118-120]

| Reserve Scenario | Financial Impact |
|-----------------|-----------------|
| Closed at reserve (ideal) | No P&L impact |
| Over-reserved (common) | Favorable development -- releases income. But if systematic, premiums were too high |
| Under-reserved (dangerous) | Adverse development -- hits current period P&L. Potential solvency concern |
| Staircase pattern (red flag) | Reserve increased incrementally throughout life. Masks true liability |

[SOURCE: extraction output Phases 9-11, lines 811-818]

**Industry data:**
- Average reserve accuracy within 10% of final paid: ~60-70%
- Claims where reserve was increased 3+ times: ~15-20% (staircase pattern)
- Over-reserving is more common than under-reserving (conservative incentive)
- Impact of 10% over-reserving across a book: reduces reported profit, inflates loss ratios, increases premiums, hurts competitive positioning

[SOURCE: extraction output Phases 9-11, lines 819-824]

**Time:** 2-15 minutes depending on complexity; often done in Excel or CMS reserve module [SOURCE: MODULE_02_PROBLEM.md, step 9]

**Automation status:** ~20% of insurers use auto-reserve setting. Five Sigma's Clive provides automated reserve setting and exposure calculation. [SOURCE: extraction output Phases 6-8, line 46]

---

### Sub-Step 6: Fraud Assessment

**Question:** Is this claim legitimate?

Fraud detection runs throughout the claim lifecycle, but it crystallizes at decision time as a formal go/no-go:

| Indicator Type | Examples |
|---------------|----------|
| **Red flags at FNOL** | Multiple prior claims, late reporting, inconsistent story, known fraud ring address |
| **Document fraud** | Fabricated invoices, altered photos, fake medical records. AI-generated fraud is growing |
| **Pattern fraud** | Staged accidents, phantom passengers, inflated medical treatment |
| **Provider fraud** | Billing for services not rendered, unnecessary procedures, kickback schemes |

**Industry scale:**
- US insurance fraud costs $80B+/year (FBI estimates)
- SIU referral rate: ~5-10% of claims
- SIU confirmation rate: ~20-30% of referred claims result in confirmed fraud or denial
- Average time SIU investigation adds: 30-90 days

[SOURCE: extraction output Phases 9-11, lines 886-891]

**Automation status:** Fraud detection is the most automated of the 6 sub-steps. Shift Technology claims >99% accuracy. FRISS provides real-time scoring. ~30% of insurers use AI fraud scoring at triage. But the investigation itself remains human. [SOURCE: extraction output Phases 6-8, lines 44, 123]

---

### The 6 Sub-Steps Combined: Time Savings Opportunity

| Sub-Step | Manual Time | With Mysa (Target) | Savings |
|----------|-------------|---------------------|---------|
| Coverage verification | 15-30 min | 2-5 min (AI reads policy, flags exclusions) | 80-85% |
| Liability determination | 5-60 min | 1-5 min (convention matching; evidence synthesis) | 80-90% (EU convention); 50-70% (US) |
| Repair assessment | 15-30 min | 5-10 min (AI pre-fills from estimation tools) | 50-70% |
| Cost analysis | 10-30 min | 2-5 min (auto-aggregation from structured data) | 70-80% |
| Reserve calculation | 2-15 min | 1-3 min (AI-calculated with confidence interval) | 50-80% |
| Fraud assessment | 2-5 min (scoring) | 1-2 min (AI pre-scored, adjuster confirms) | 50-70% |
| **Total decision time** | **65-120 min** | **10-15 min** | **4-8x improvement** |

[SOURCE: MODULE_01_POSITIONING.md, lines 92, 210; mysa_product_strategy.md, Part 1]

---

## 3.5 EU vs US Comparison

### Side-by-Side Across Every Dimension

| Dimension | EU Motor | US Motor |
|-----------|---------|---------|
| **Legal framework** | Convention-based direct settlement (each insurer pays own policyholder) | Adversarial (at-fault party's insurer pays, or first-party with subrogation) |
| **Guiding principle** | "Pay first, recover later" | "Deny then defend" (perceived by plaintiffs) |
| **Scene documentation** | EAS -- joint form filled by both drivers, signed by both | No joint form. Police crash report + separate accounts |
| **Fault determination** | Convention bareme -- standardized lookup tables | Individual adjuster assessment, negotiated. Comparative vs contributory negligence |
| **Inter-insurer settlement** | Clearing house, forfait flat-rate, monthly batch | Bilateral subrogation. Arbitration Forums if disputed ($17.6B/yr, 869K disputes) |
| **STP potential** | 60-70% theoretical, ~10% actual | Very low for complex claims |
| **STP bottleneck** | Data quality at intake (paper EAS, messy handwriting) | Everything is manual -- no STP mechanism |
| **Convention systems** | IRSA (France), CARD (Italy), CIDE (Spain), IDS (Portugal), RDR (Belgium) | None |
| **Adjuster time per routine claim** | 5-15 min (clean EAS path) | 30-60+ min (recorded statements required) |
| **Recorded statements** | Rare for routine PD | Near-universal. 2-4 per claim |
| **Police involvement** | Only if injuries/dispute/request | Legally required above $500-$1,000 threshold |
| **Phone tag** | Minimal for clean EAS | 2.7 attempts to reach each party. 30-40% of investigation time |
| **Call recording** | Rarely -- GDPR makes phone recording complex | Standard practice -- all calls recorded |
| **State/country variation** | Country-by-country convention rules + regulators | 50 states with different rules on everything |
| **No-fault / at-fault split** | Not applicable (convention handles) | ~12 no-fault states; majority at-fault |
| **BI settlement** | Often outside convention (traditional liability process) | Adversarial demand/counteroffer. 3-8 rounds. Colossus/Claims Outcome Advisor |
| **Attorney involvement** | Rare for material damage (~5%) | Common for BI (~35-40%), growing for property |
| **Settlement timeline (material)** | IT: 30/60 days to offer + 15 to pay. FR: 3 months | 30-45 days typical acknowledgment + 5-30 days payment |
| **Release of liability** | Not always required for convention material damage | Standard practice -- near-universal |
| **Subrogation** | Convention forfait handles most recovery automatically | Manual bilateral process. $15B+/year left on table |
| **Total loss threshold** | Typically 60-70% of vehicle value | State-by-state: 70-100% of ACV |
| **Salvage market** | Less standardized | Copart and IAA dominate. Highly standardized |
| **Statute of limitations** | France 10 yr, Germany 3 yr, Spain 1 yr (PI: 5 yr) | 1-6 years. Most states 2-3 yr PI, 2-6 yr PD |
| **Data retention** | GDPR: 5-10 years with right to request deletion | State-specific. Generally 5-7 years. No federal GDPR equivalent |
| **Regulatory reporting** | Solvency II Pillar III. ~55 reporting templates | NAIC Annual Statement Schedule P. State DOI market conduct exams |
| **Estimation tools** | Audatex/Qapter (Solera) -- EU-focused | CCC Intelligent Solutions (dominant), Mitchell |
| **CMS landscape** | Legacy systems, some Guidewire/Duck Creek. Many mid-market on homegrown | More standardized on Guidewire, Duck Creek, Salesforce |

[SOURCE: claims_journey_discovery.md -- EU vs US comparison sections across all phases; MODULE_01_POSITIONING.md, lines 131-140; extraction output Phases 9-11, lines 349-358, 974-985]

### Automation Opportunity by Market

| Opportunity | EU | US |
|------------|----|----|
| **Biggest time sink** | Paper EAS digitization (50% still paper) | Recorded statements (30-60 min per party) |
| **Biggest automation gap** | Getting clean data TO the convention lookup | Everything is manual from the start |
| **Product entry point** | Document track: EAS extraction + convention matching | Voice track: call transcription + SOP coaching |
| **Competitive moat** | Convention engine -- ZERO competitors | Real-time voice assist during calls -- ZERO competitors |
| **Shared opportunity** | Messy claims (disputes, incomplete data, BI) are expensive everywhere |

[SOURCE: claims_journey_discovery.md, lines 361-370; claims_journey_discovery.md, lines 11859-11893]

---

## 3.6 All Personas and Their Roles

The claims adjuster does not work alone. Every claim involves a network of professionals, each with distinct roles and distinct pain points. This section maps the full ecosystem.

### Primary Personas (Direct Users of Mysa)

| Persona | What They Do | Daily Reality | Caseload | How Mysa Helps |
|---------|-------------|---------------|----------|----------------|
| **Desk Adjuster** | Handles straightforward claims from office. Reviews documentation, makes coverage/reserve decisions. Highest volume | 5-7 systems, 20+ calls/day, 30-40% admin. Relies on photos, virtual appraisal, field adjuster reports | PD: 80-150 claims. BI: 40-80 | Primary user. AI pre-fills 6 decision sub-steps. 65-120 min to 10-15 min per claim |
| **Field Adjuster** | Investigates complex/high-value claims on-site. Inspects damage, interviews witnesses, collects evidence | 25-30% of time is travel. Hands-on vehicle/property inspection. Lower volume, higher complexity | PD: 60-100 claims | Investigation scoping, documentation generation, evidence checklist per SOP |
| **BI Adjuster** | Specializes in bodily injury claims. Reviews medical records, calculates injury costs | 30-120 min per medical record review cycle. Colossus input. Long-tail claims spanning months-years | BI: 25-50 claims | Medical record parsing, comparable injury analysis, reserve calculation |
| **SIU Investigator** | Handles suspected fraud referred from triage or investigation | Formal investigation. Recorded statements, cross-referencing, surveillance | 15-30 active investigations | Fraud signal agent. Risk scoring and pattern matching. Referral recommendations |
| **Supervisor / Team Lead** | Reviews decisions above authority limits. Manages team workload and quality | Reviews 50+ decisions/day. Quality bottleneck | Oversight of 10-20 adjusters | Dashboard: decision audit trail, SOP compliance, workload distribution |

[SOURCE: MODULE_01_POSITIONING.md, lines 70-79, 170-189; claims_journey_discovery.md, lines 1466-1530]

### Secondary Personas (Interact with Mysa Indirectly)

| Persona | Role in Claims | Pain Point | Mysa Interaction |
|---------|---------------|------------|------------------|
| **Appraiser** | Estimates physical damage value (may be internal, independent, or body shop) | Multiple re-inspections for supplements. ACV disputes | Data exchange: claim photos, repair scopes, estimates |
| **Medical Case Manager** | Manages ongoing medical treatment claims. Coordinates with healthcare providers | Complex medical terminology. Treatment appropriateness evaluation | Treatment timeline tracking, medical cost analysis |
| **Broker / Agent** | Submits claims on behalf of policyholders. First point of contact. EU: 55-58% agents, 25-30% brokers | "Claims visibility black hole" -- no real-time status. Manual FNOL submission | White-labeled FNOL forms. Email-to-claim creation |
| **TPA (Third-Party Administrator)** | Processes claims on behalf of carriers who outsource. Must follow carrier-specific SOPs | Authority cap referrals create delays. Data handoff friction. Inconsistent practices | Same product as carrier -- SOPs come from client carrier. Per-claim pricing |
| **Legal / Compliance** | Reviews for regulatory compliance. Handles litigation, bad faith allegations | 50 states or country-by-country regulation. Audit readiness | Audit trail: AI recommendation + adjuster decision + SOP compliance |
| **Underwriter** | Sets policy terms and pricing. Doesn't process claims but claims data informs pricing | Claims-to-underwriting feedback loop is quarterly/annual, not real-time | Downstream: aggregated claims decision data feeds underwriting models |

[SOURCE: MODULE_01_POSITIONING.md, lines 170-189; claims_journey_discovery.md, lines 2500-2530]

### External Personas

| Persona | Role | Key Data |
|---------|------|----------|
| **Policyholder / Claimant** | Files claim, receives settlement. End beneficiary | 45% don't understand how settlement was calculated. 60% cite slow settlement as primary frustration |
| **Repair Network** | Body shops, contractors who perform repairs | Supplement approval delays 3-5 business days. Payment lag 15-30 days post-invoice |
| **Salvage / Recovery** | Handles total-loss vehicles, damaged goods disposal | Copart and IAA dominate US. Less standardized in EU |
| **Arbitration / Convention Body** | Resolves inter-insurer disputes. EU: IRSA/CARD/CIDE clearing houses. US: Arbitration Forums Inc. | AF resolved 869,000 disputes worth $17.6B in 2021 |
| **Public Adjuster / Loss Assessor** | Works for the POLICYHOLDER, not insurer. Advocates for higher settlement | US: regulated, 10-15% fee. UK: loss assessors established. Less common continental EU |

[SOURCE: extraction output Phases 9-11, lines 601-635; claims_journey_discovery.md, lines 2500-2555]

### Major TPAs (Third-Party Administrators)

| TPA | Scale | Notes |
|-----|-------|-------|
| **Crawford and Company** | 10,000+ employees, 50,000+ field resources, 70 countries | Largest in the world |
| **Sedgwick** | Largest adjuster network globally, 25 yr avg experience | End-to-end TPA. Strong DRP network |
| **Gallagher Bassett** | Global TPA | Strong commercial focus |
| **Broadspire** | US-focused | |
| **McLarens** | 100+ personnel in Europe | Strong EU presence, specialty/complex |
| **Davies Group** | Revenue ~$1.4B, 9,500+ across 22 countries | UK/EU focus. Owns Kuarterback AI |
| **Charles Taylor** | Global | Technical adjusting |
| **Engle Martin** | Delegated authority specialist | Low-touch to CAT claims |

[SOURCE: claims_journey_discovery.md, lines 2511-2521; extraction output Phases 9-11, lines 270-275]

**TPAs handle 25-35% of motor claims and are a key distribution channel for Mysa.** If Mysa can make their adjusters more productive, it directly impacts their unit economics. Per-claim pricing is a natural fit. [SOURCE: claims_journey_discovery.md, line 2532]

---

## 3.7 Decision Forks and Complexity Scoring

Claims are not linear. At multiple points, the claim can fork into entirely different processing paths -- each with different timelines, costs, and complexity. This section documents 8 documented decision forks and the triage logic that routes claims.

### The 8 Decision Forks

| Fork | Question | Paths | Impact |
|------|----------|-------|--------|
| **F1: Injuries?** | Is anyone injured? | YES: BI claim path (higher complexity, longer lifecycle, lawyers, BI specialist). NO: Material damage only | BI claims are 10-50x more expensive than PD. Average BI settlement: $20K-$25K (minor) to $100K+ (severe) |
| **F2: Cooperation?** | Is the other party cooperative? (EU) | Cooperative: EAS filled jointly. Uncooperative: no joint statement, much harder. Hit and Run: no counter-party, guarantee fund path | Non-cooperative claims require full investigation. Adds weeks to months |
| **F3: EU vs US Market** | Which legal framework? | EU: EAS-based, convention-based settlement. US: Competing narratives, adversarial settlement | Fundamentally different workflows, tools, and automation opportunities |
| **F4: Channel** | How does the claim arrive? | Direct to insurer / through broker / through agent / bancassurance | Broker adds data handoff step. Agent may file directly in insurer system |
| **F5: STP Eligibility** | Does this claim qualify for straight-through processing? | YES: Auto-process with minimal review. NO: Route to adjuster | Only ~10% actual STP despite 60-70% theoretical (EU). Data quality is bottleneck |
| **F6: No-Fault vs At-Fault** (US) | Which state legal framework? | No-Fault (~12 states): PIP covers medical regardless of fault. At-Fault (majority): fault determines everything | Completely different investigation and settlement workflows |
| **F7: Repair vs Total Loss** | Does repair cost exceed threshold? | Repairable: authorize repair, manage supplements. Total Loss: ACV calculation, salvage, title transfer | Total loss is specialized workflow. 20% of auto claims (rising) |
| **F8: Authority Limit** | Does the decision amount exceed the adjuster's authority? | Within authority: adjuster decides. Exceeds: escalate to supervisor/committee | 20-30% of claims require supervisor approval, adding 1-3 days each |

[SOURCE: claims_journey_discovery.md, lines 83-126 (F1-F2), 138-189 (F3), 386-413 (F4), 320-321 (F5), 241-256 (F6), 1853-1885 (F7); extraction output Phases 9-11, lines 536-545 (F8)]

### Triage Logic: How Claims Are Routed

```
FNOL RECEIVED
     |
AUTO-TRIAGE (rules-based at ~60% of mid-large insurers)
     |
+-- SIMPLE PD + CLEAN DATA + LOW FRAUD SCORE
|   --> STP Engine (if eligible) or PD Desk Adjuster
|
+-- MODERATE COMPLEXITY
|   --> PD Desk Adjuster (standard queue)
|
+-- INJURIES REPORTED
|   --> BI Specialist Adjuster
|
+-- VEHICLE LIKELY TOTALED
|   --> Total Loss Desk
|
+-- HIGH FRAUD SCORE (>70)
|   --> SIU (formal investigation before proceeding)
|
+-- ATTORNEY LETTER OF REPRESENTATION
|   --> Litigation Handler
|
+-- CAT EVENT DECLARED
    --> Catastrophe Team (surge protocols)
```

**Auto-triage override rate:** 20-30%. This means the automated routing is wrong for roughly 1 in 4-5 claims. AI/ML complexity scoring (at ~15-20% adoption) is more accurate. [SOURCE: extraction output Phases 6-8, lines 21, 43]

### Claim Complexity Scoring

Claims exist on a spectrum of complexity, not in binary categories. Scoring factors include:

| Factor | Low Complexity | High Complexity |
|--------|---------------|-----------------|
| **Parties** | 2 drivers, clear | 3+ vehicles, pedestrians, commercial |
| **Injuries** | None | Multiple, severe, ongoing treatment |
| **Liability** | Clear (EAS/convention match or admission) | Disputed, multi-party, comparative negligence |
| **Coverage** | Standard, no questions | Exclusion questions, stacking, multi-policy |
| **Attorney** | None | Letter of representation received |
| **Fraud indicators** | None | Multiple flags, SIU referral |
| **Value** | Under adjuster authority | Exceeds authority, requires committee |
| **Jurisdiction** | Favorable for insurer | High-litigation jurisdiction, nuclear verdict risk |

**Five Sigma's Clive** uses dynamic complexity rating (Low/Medium/High) analyzing liability, severity, legal involvement, and regulatory factors. **Shift Technology** classifies by urgency and decides STP vs human routing with a reported 60% automation rate. **Tractable** determines repair vs total loss from photos at FNOL, flagging severity before the adjuster touches the claim. [SOURCE: extraction output Phases 6-8, lines 50-57]

---

## 3.8 The "Adjuster of 2027" Vision

### Today's Adjuster (2025-2026)

| Metric | Current State |
|--------|--------------|
| **Caseload** | ~125 open claims, 300-480 closed per year |
| **Time per routine decision** | 65-120 minutes (the 6 decision sub-steps) |
| **Admin time** | 30-40% of total day |
| **Systems used** | 5-7 per claim (CMS, policy system, estimation tool, convention platform, phone, email, reporting) |
| **Phone calls** | 20+ per day |
| **Context switching** | Constant -- loses context when jumping between systems and claims |
| **Supervisor bottleneck** | 20-30% of decisions require supervisor approval (1-3 day delay each) |
| **STP rate** | ~10% (EU), near-zero (US complex) |
| **Knowledge transfer** | 6 years to develop full expertise. Knowledge walks out the door at retirement |
| **Reserve accuracy** | 60-70% within 10% of final paid |

[SOURCE: MODULE_01_POSITIONING.md, lines 75-85; MODULE_02_PROBLEM.md, lines 15-47; extraction output Phases 6-8, lines 262-282]

**A day in the life of today's adjuster:**

```
8:00  Log into CMS. 15 new assignments overnight. 125 open claims.
8:15  Start processing. Open first claim. Pull up policy PDF. Ctrl-F for coverage clauses.
8:30  Switch to estimation tool. Compare repair estimate against market rates.
8:45  Call policyholder for clarification. Voicemail. Note in CMS: "Attempted contact."
8:50  Call claimant. Reached. 15-minute recorded statement.
9:10  Enter statement notes into CMS. Copy data from phone notes.
9:25  Switch to convention platform (EU). Re-key EAS data. Wait for match.
9:35  Convention matches to scenario. Back to CMS. Update liability.
9:40  Calculate reserve in Excel. Enter in CMS.
9:50  Write coverage determination letter. 15 minutes.
10:05 Submit to supervisor for review. Claim #1 paused.
10:10 Start claim #2. Repeat.
...
4:30  End of day. Processed 8-12 claims. 15 still waiting from this morning.
      50+ remain untouched. Diary items backed up.
```

### The Mysa-Enabled Adjuster (2027)

| Metric | Target State |
|--------|-------------|
| **Caseload** | 200+ claims managed (2-3x increase with same headcount) |
| **Time per routine decision** | 10-15 minutes (AI pre-fills all 6 sub-steps; adjuster reviews) |
| **Admin time** | <10% (AI handles documentation, data entry, context surfacing) |
| **Systems used** | 1 interface (Mysa sits on top of existing systems, pushes with one click) |
| **Phone calls** | AI transcribes live, extracts entities, auto-fills CMS. Post-call summary in seconds |
| **Context switching** | Near-zero -- Mysa surfaces all relevant context per claim |
| **Supervisor bottleneck** | Batch review of AI-recommended decisions. Supervisor reviews 10x faster |
| **STP rate** | 30-50% of simple PD motor claims (Month 18-24) |
| **Knowledge transfer** | New adjusters follow SOP-driven workflows from Day 1. Same process as 10-year veteran |
| **Reserve accuracy** | >80% (AI-calculated with confidence intervals from comparable claims) |

**A day in the life of the Mysa-enabled adjuster:**

```
8:00  Log into Mysa. 15 new assignments. AI has pre-processed 10 of them.
8:05  Claim #1: Mysa read the EAS (OCR), matched convention scenario (IRSA #4),
      confirmed coverage (policy active, no exclusions), set reserve ($3,200 based
      on 47 similar claims), scored fraud (LOW). One-click: Approve.
      Total time: 3 minutes.
8:08  Claim #2: Same. One-click approve. 2 minutes.
8:10  Claim #3: Mysa flags uncertainty. "Convention match confidence: 62%.
      Diagram ambiguous -- vehicles may have been merging or turning."
      Adjuster reviews photos, makes judgment call. Overrides to Scenario 7.
      Total time: 12 minutes. Mysa logs the override as training data.
8:22  Claim #4: Complex. BI claim. Attorney involved. Mysa surfaced medical records,
      extracted injury codes, compared to 12 similar claims in this jurisdiction.
      "Recommended reserve: $45,000. Range: $32,000-$68,000. Confidence: 71%."
      Adjuster reviews, adjusts to $52,000, writes reasoning in 2 sentences.
      Total time: 20 minutes.
8:42  Claims #5-10: US claims. Adjuster makes outbound call. Mysa transcribes live.
      Entities extracted in real-time. SOP prompts in sidebar: "Ask about witnesses."
      "Confirm injury status." "Get rental details." Call ends. Summary auto-generated.
      One-click push to CMS. 15 minutes per call instead of 35.
...
4:30  End of day. Processed 25-30 claims. All diary items current.
      Backlog shrinking. Going home on time.
```

### Concrete Before/After Comparison

| Activity | Before (Manual) | After (Mysa) | Time Saved |
|----------|----------------|--------------|------------|
| **Read EAS / intake documents** | 5-15 min (manual read, re-key) | 30 sec (OCR extraction) | 90-95% |
| **Convention matching** | 5-15 min (re-key into convention platform) | 5 sec (auto-match with confidence score) | 95%+ |
| **Coverage verification** | 15-30 min (Ctrl-F through 40-page PDF) | 2-5 min (AI reads policy, flags exclusions) | 80-85% |
| **Recorded statement** (US) | 15-30 min + 15 min notes entry | Same call time + 1 min (auto-transcription, auto-fill) | 50% of total time |
| **Reserve calculation** | 10-15 min (Excel, gut feel) | 1-3 min (AI with confidence interval, comparable claims) | 75-85% |
| **Document generation** | 15-25 min (manual from template) | 2-5 min (AI draft with decision reasoning trail) | 80-85% |
| **Supervisor review** | 10-20 min per decision + 0-48 hr wait | 2-5 min (AI pre-validates; supervisor batch reviews) | 75-90% |
| **CMS data entry** | 5-15 min (manual across 5-7 systems) | 30 sec (one-click push) | 95% |

### The Flywheel: Every Claim Makes the System Smarter

The critical difference between Mysa and every competitor: decision capture.

```
Adjuster processes claim through Mysa
     |
     v
INVISIBLE DATA CAPTURE (Block 5):
|-- What evidence was reviewed?
|-- What did the AI recommend?
|-- What did the adjuster actually decide?
|-- WHY did they override the AI (if they did)?
|-- How long did each step take?
     |
     v
After 1,000 claims: Recommendations start
After 10,000 claims: Recommendations are accurate
After 100,000 claims: Near-STP for routine claims
```

Every competitor trains on OUTCOMES -- what was paid. Mysa trains on REASONING -- why it was paid. Outcomes inherit errors in historical data. Reasoning captures expert judgment. This is the dataset that does not exist anywhere else in the industry. [SOURCE: claims_journey_discovery.md, lines 11624-11631; MODULE_01_POSITIONING.md, lines 40-44]

### The 2027 Adjuster Is Not Replaced -- They Are Elevated

The adjuster of 2027 handles 2-3x more claims but spends MORE of their time on the highest-value work -- complex judgment calls, negotiation, fraud investigation -- and LESS on the low-value work that drains them today. The profession becomes more sustainable, more attractive to younger talent, and more resilient to the workforce crisis.

> "The product is proactive on every single step... not only removing manual work but empowering the decision-making process."
> -- Jeremy Blehaut [TRANSCRIPT: Feb 9, 2026]

[SOURCE: MODULE_01_POSITIONING.md, lines 242-243]

---

## Sources

| Source | Type | Sections Used |
|--------|------|--------------|
| `claims_journey_discovery.md` (736KB, 11,968 lines) | Primary -- all phase data, EU vs US comparisons, persona mapping, property claims, competitor analysis | 3.1-3.8 |
| Extraction output: Phases 0-5 (`af38eab.output`) | Derived -- structured extraction from discovery doc | 3.1, 3.2 |
| Extraction output: Phases 6-8 (`adde4a9.output`) | Derived -- structured extraction from discovery doc | 3.1, 3.2, 3.4 |
| Extraction output: Phases 9-11 (`a625e30.output`) | Derived -- structured extraction from discovery doc | 3.1, 3.2, 3.5, 3.6, 3.7 |
| `MODULE_01_POSITIONING.md` | Prior FOS module -- positioning, personas, value stack | 3.4, 3.6, 3.8 |
| `MODULE_02_PROBLEM.md` | Prior FOS module -- workflow audit, workforce crisis, STP gap | 3.4, 3.8 |
| `mysa_product_strategy.md` Parts 1-2 | Primary -- product strategy, market sizing, decision sub-steps | 3.4, 3.8 |
| Feb 7, 2026 Granola call | Transcript (summary) | 3.8 |
| Feb 9, 2026 Granola call | Transcript (summary) | 3.8 |

---

# Part 4: Market Landscape

# Module 4: Market Landscape

**Status:** DRAFT v1.0
**Last updated:** February 9, 2026
**Feeds:** Pitch deck slides 3-6 (market), fundraising data room, sales territory planning, board TAM narratives
**Depends on:** Module 1 (Positioning & ICP), Module 2 (Problem)

---

## Glossary

| Term | Definition |
|------|-----------|
| **GWP** | Gross Written Premiums — the total premium income an insurer writes in a period, before reinsurance deductions. The standard measure of insurer size in the EU. |
| **DWP** | Direct Written Premiums — the US equivalent of GWP. Total premiums written directly by an insurer, excluding assumed reinsurance. |
| **STP** | Straight-Through Processing — claims resolved near-instantly with minimal human review, typically via convention system automation. |
| **Convention System** | Standardized inter-insurer protocol for settling motor claims between two insurers (e.g., IDS in Portugal, IRSA in France, CARD in Italy, CIDE in Spain). Defines deterministic rules for fault allocation. |
| **TPA** | Third-Party Administrator — a company that processes claims on behalf of insurance carriers who outsource their claims operations. |
| **MGA** | Managing General Agent — an intermediary with underwriting authority from a carrier, increasingly also handling claims. |
| **ACV** | Annual Contract Value — the annualized revenue from a single customer contract. |
| **Caravela tier** | Mysa's term for the primary target segment: carriers with €100-200M GWP (or $100-500M DWP in the US). Named after design partner Caravela Seguros (€188M GWP). |
| **P&C** | Property and Casualty — the insurance category covering motor, home/property, commercial, and liability. |
| **Cat / Nat Cat** | Catastrophe / Natural Catastrophe — large-scale insured events (floods, earthquakes, wildfires). Drives spikes in claims volume and cost. |
| **CCS** | Consorcio de Compensacion de Seguros — Spain's state reinsurer for catastrophe risk. |
| **CCR** | Caisse Centrale de Reassurance — France's state reinsurer for natural catastrophe risk (Cat-Nat regime). |
| **KGV** | Kantonale Gebaudeversicherung — Swiss cantonal building insurance monopolies (19 of 26 cantons), limiting the private property insurance market. |

---

## 4.1 Global Overview

### The Opportunity at a Glance

The global motor and property claims market processes an estimated **80-95 million claims per year** across the EU and US alone, backed by approximately **$1.5 trillion in combined premiums** (using approximate EUR/USD parity for simplicity). This is the universe in which Mysa operates. [SOURCE: market_landscape_overview.md, Section 1]

### Total Claims Volume — Motor + Property

| Market | Motor Claims/Year | Property Claims/Year | **Combined** |
|--------|------------------|--------------------------|-------------|
| **EU (16 countries)** | ~25-35M | ~16-20M | **~41-55M** |
| **US** | ~35M | ~4.4-4.5M | **~39.5M** |
| **Global total** | **~60-70M** | **~20-25M** | **~80-95M** |

[SOURCE: market_landscape_overview.md, Section 1 — "Total Claims Volume"]

### Total Premium (GWP / DWP)

| Market | Motor GWP/DWP | Property GWP/DWP | **Combined** |
|--------|----------|-------------------|-------------|
| **EU Southern (PT, ES, FR, IT)** | €57.9B | ~€24-28B | **~€82-86B** |
| **EU Northern/Central (12 countries)** | €70-78B | ~€30-33B | **~€100-111B** |
| **EU Total (16 countries)** | **~€128-136B** | **~€54-61B** | **~€182-197B** |
| **US** | ~$359B (auto) | $172.7B (homeowners) | **~$532B** |
| **Global combined** | | | **~€700B+** |

[SOURCE: market_landscape_overview.md, Section 1 — "Total Premium (GWP/DWP)"]

### Motor vs Property: Two Lines, One Market

Motor insurance is the larger line by premium volume, but property is the faster-growing opportunity — particularly in the EU, where mandatory nat cat schemes are expanding coverage and increasing claims volumes. The critical structural insight is that **80-95% of carriers that write motor also write property** — the buyer list is essentially the same. [SOURCE: market_landscape_overview.md, Section 3]

| Dimension | Motor | Property |
|-----------|-------|----------|
| **EU GWP** | ~€128-136B | ~€54-61B |
| **US DWP** | ~$359B | $172.7B |
| **EU claims/year** | ~25-35M | ~16-20M |
| **US claims/year** | ~35M | ~4.4-4.5M |
| **Convention system?** | YES (EU only) — IRSA, CARD, CIDE, IDS | **NONE — anywhere** |
| **Core decision** | WHO caused it? (fault %) | WAS it covered? (policy interpretation) |
| **Estimation monopoly** | Audatex/Solera (EU), CCC/Mitchell (US auto) | Xactimate (US, ~80%), fragmented in EU |
| **AI competition for decisions** | Some (Shift, Five Sigma) | **Almost none** (Crawford CoverAI failed, Wamy pre-traction) |
| **Avg claim size** | ~€1,500-3,000 (EU), ~$5,000 (US) | ~€3,000-8,000 (EU), **$17,059 (US — 3.4x auto)** |
| **Dominant peril** | Collision | **Water damage (38-44% EU), wind/hail (US)** |

[SOURCE: market_landscape_overview.md, Section 3 — "Motor vs Home — Side by Side, Same Carriers"]

### Total Carrier/Buyer Universe

| Market | Total Carriers | TPAs | MGAs | **Total Potential Buyers** |
|--------|---------------|------|------|--------------------------|
| **EU** | ~2,141+ undertakings | ~200-300 | 650+ (€18B GWP, 23% CAGR) | **~3,000+** |
| **US** | ~4,116 P&C entities | ~500-800 | ~330-550 | **~5,000-5,500** |
| **Global** | | | | **~8,000+** |

[SOURCE: market_landscape_overview.md, Section 1 — "Total Carrier/Buyer Universe"]

---

## 4.2 EU Market by Country

This section covers all 16 validated EU markets, split into Southern EU (countries with established motor convention systems — the initial wedge) and Northern/Central EU (mixed or no convention systems — expansion markets).

All data sourced from validated regulatory filings and industry bodies: ASF (Portugal), DGSFP/ICEA (Spain), ACPR/France Assureurs (France), IVASS/ANIA (Italy), BaFin (Germany), DNB (Netherlands), FSMA/Assuralia (Belgium), FMA/VVO (Austria), FINMA/SVV (Switzerland), Central Bank of Ireland, FI Sweden/Svensk Forsakring, FSA Denmark, FIN-FSA Finland, Finanstilsynet Norway, KNF/PIU (Poland), CNB/XPRIMM (Czech Republic), EIOPA, NAIC, AM Best. [SOURCE: mysa_product_strategy.md, Part 9a — full regulatory source list]

---

### 4.2.1 Southern EU (Convention System Countries — The Wedge)

These four countries have established motor convention systems that create a technical wedge for Mysa: deterministic fault rules encoded into inter-insurer settlement protocols. Convention expertise is hard to replicate and creates immediate value for carriers struggling with data quality at convention intake.

#### Motor Insurance

| Country | Convention System | Motor GWP | Registered Vehicles | Total Insurers | Motor Writers | Caravela-Tier Carriers (€100-200M) | Small Carriers (€50-100M) | Convention Detail |
|---------|-------------------|-----------|---------------------|----------------|---------------|-------------------------------------|---------------------------|-------------------|
| **Portugal** | IDS/CIMPAS | **€1.8B** (2023) | ~5.8M light (7.3M total) | ~47 active non-life (63 domestic) | ~25-30 | **6-8** | ~8-12 | 1.94 day avg processing, 91% agreement rate |
| **Spain** | CIDE/ASCIDE/CICOS | **€13.2B** (2024, +8.9%) | **34M** | ~176 operating (187 RAEA) | ~80-100 (31 groups in motor) | **8-10** | ~25-35 | 2.5M claims/year processed through convention |
| **France** | IRSA | **€28.1B** (2024, +7.3%) | **45.5M** | **660** ACPR-supervised (246 FFA, 324 mutuelles, 302 insurance code, 34 social security code) | ~100-120 | **30-60** | ~100+ | 13 cases, deterministic rules |
| **Italy** | CARD | **~€14.8B** (2023) | **~40M** | ~85 national (IVASS) | **38** write RC Auto | **10-15** | ~8-12 | Mandatory for 2-vehicle collisions |
| **Southern EU Total** | **All have convention** | **€57.9B** | **~125M** | | | **54-93** | **141-159+** | |

[SOURCE: mysa_product_strategy.md, Part 3c — country-level data; Part 9a — convention details and regulatory sources]

> [WEB SOURCE: Portugal — ECO/ASF rankings, top 10 = 92% of market. Spain — DGSFP sector report, 176 operating entities. France — ACPR data, 660 organizations. ACPR 1st quartile cutoff = €82M. Italy — IVASS, only 38 companies write RC Auto. EIOPA — ~300 of ~2,300 Solvency II entities qualify as SNCU (<€100M GWP, ~13%)]
> [SOURCE: mysa_product_strategy.md, Part 3c]

**Key observations:**

- **France is the largest motor market in the EU** at €28.1B, and has the most mid-market targets (30-60 Caravela-tier carriers, 100+ small carriers). The French mutuelle system creates a deeply fragmented market with hundreds of autonomous, multi-line carriers — many with motor books in the €82-200M range. [SOURCE: mysa_product_strategy.md, Part 3c]
- **Spain is the fastest-growing motor market** at +8.9% YoY. Its convention system (CIDE) processes 2.5M claims per year. [SOURCE: mysa_product_strategy.md, Part 9a]
- **Portugal is the smallest market but the best proving ground** — tightest feedback loop, highest convention agreement rate (91%), and Caravela as design partner. [SOURCE: mysa_product_strategy.md, Part 3c]
- **Italy has the fewest motor writers** (only 38 write RC Auto per IVASS) but mandatory CARD convention for two-vehicle collisions. Italy's pending mandatory nat cat insurance for businesses (effective October 2025) will drive massive property claims growth. [SOURCE: mysa_product_strategy.md, Part 3c; Part 3f]

#### Property Insurance

| Country | Property GWP | Claims/Year | Penetration | Dominant Peril | Catastrophe Scheme |
|---------|-------------|------------|-------------|---------------|-------------------|
| **Portugal** | ~€0.44B (Multirriscos) | ~200-300K est. | ~55% | Wildfires, storms | None |
| **Spain** | **€6.1B** (Hogar, 61.4% of €9.99B multirriesgos) | **~4M+** (UNESPA) | ~74% | **Water damage (38.2%)** | **CCS** (state reinsurer; DANA 2024 = €3.5B) |
| **France** | **€13.8B** (MRH, 2024, +7.5%) | **4.6M** (France Assureurs) | **~96%** (mandatory for tenants) | **Water damage (44%)** | **CCR/Cat-Nat** (surcharge increasing 12% to 20%) |
| **Italy** | ~€3.5-4.0B (Fire + Property) | ~1-2M | ~50% (lowest in Southern EU) | Earthquakes, floods | **Mandatory nat cat for businesses from Oct 2025** |
| **Southern EU Total** | **~€24-28B** | **~10-12M** | | | |

[SOURCE: mysa_product_strategy.md, Part 3f — Southern EU Home/Property Market; market_landscape_overview.md, Section 5]

> [WEB SOURCE: France Assureurs 2024, ICEA 2024, UNESPA, ASF, ANIA/IVASS, DLA Piper Italy nat cat law]
> [SOURCE: mysa_product_strategy.md, Part 3f]

**Key observations:**

- **Water damage is the "fender bender" of property claims** — 38-44% of all home claims in Spain and France. Highly repetitive, highly standardizable, and perfect for AI-assisted decision-making. [SOURCE: mysa_product_strategy.md, Part 3f]
- **Italy is a massive growth story**: mandatory nat cat insurance for all businesses (effective October 2025) will add an estimated €2-3B in new premiums. Residential mandatory coverage is under discussion. 2023 was a record cat year (€6B insured losses). Claims volumes will surge, and carriers will need tech to handle it. [SOURCE: mysa_product_strategy.md, Part 3f]
- **France has near-universal penetration** (~96%) because tenants insurance is mandatory, making it the largest EU property claims market by volume (4.6M claims/year). [SOURCE: mysa_product_strategy.md, Part 3f]

---

### 4.2.2 Northern/Central EU (Mixed Convention Systems — Expansion Markets)

These 12 countries represent a larger premium pool than Southern EU (€70-78B motor vs €57.9B) but with fewer mid-market carriers in the Caravela tier. Convention systems are mixed — some countries have partial or emerging convention-like systems, others have none. The wedge is weaker here, but the market size justifies expansion once Southern EU is proven.

#### Motor Insurance

| Country | Motor GWP | Convention-Like System? | Total Insurers | Caravela-Tier (€100-200M) | Small (€50-100M) |
|---------|----------|------------------------|----------------|--------------------------|-------------------|
| **Germany** | **~€30B** | Teilungsabkommen (bilateral only, not universal) | ~522 BaFin + 534 state-supervised | **15-25** | 20-35 |
| **Netherlands** | **~€5.9-6.2B** | DSA (new, launched 2024) | ~60-70 | **3-5** | 5-8 |
| **Belgium** | **~€4.3-4.5B** | RDR (Convention Reglement Direct) | ~82-90 | **5-8** | 8-12 |
| **Austria** | **~€4.3B** | None formal | ~30-35 | **2-4** | 3-5 |
| **Switzerland** | **~€7.2-8.2B** | None formal | ~117 | **3-5** | 5-8 |
| **Ireland** | **~€1.3B** | None | ~40-50 | **2-4** | 3-5 |
| **Sweden** | **~€2.6-2.9B** | Trafikskadenamden (injury board) | ~50-60 | **3-4** | 4-6 |
| **Denmark** | **~€2.0-2.4B** | None formal | ~40-50 | **2-3** | 3-5 |
| **Finland** | **~€1.2-1.4B** | Traffic Insurance Centre | ~40-49 | **2-3** | 2-3 |
| **Norway** | **~€2.7-2.8B** | None formal | ~30-40 | **2-3** | 3-4 |
| **Poland** | **~€6.5B** | UFG coordination | ~29 | **3-5** | 4-6 |
| **Czech Republic** | **~€2.1-2.3B** | None formal | ~24-30 | **2-3** | 3-4 |
| **Northern/Central EU Total** | **~€70-78B** | **Mixed** | | **~42-72** | **~63-101** |

[SOURCE: mysa_product_strategy.md, Part 9a — Northern/Central EU table; validated via BaFin, DNB, FSMA, FMA, FINMA, FI Sweden, FSA Denmark, FIN-FSA, Finanstilsynet Norway, KNF Poland, CNB Czech Republic]

**Key observations:**

- **Germany (~€30B) is the single largest EU motor market** but more concentrated than Southern EU — fewer mid-market targets proportionally. Still, 15-25 Caravela-tier carriers is the largest Northern segment. [SOURCE: mysa_product_strategy.md, Part 9a]
- **Belgium (RDR convention), Netherlands (DSA — new 2024), and Sweden (Trafikskadenamden)** have convention-like systems, providing a partial wedge opportunity. [SOURCE: mysa_product_strategy.md, Part 3d]
- **Poland (€6.5B)** is a significant market with only ~29 insurers — more concentrated but growing. [SOURCE: mysa_product_strategy.md, Part 9a]
- **Austria, Switzerland, Ireland, Denmark, Norway, Finland, Czech Republic** have no formal convention systems — the sell here is the general decision engine capability, not convention expertise. [SOURCE: mysa_product_strategy.md, Part 3d]

#### Property Insurance

| Country | Property GWP | Penetration | Key Dynamic | Motor/Property Carrier Overlap |
|---------|-------------|-------------|------------|-------------------------------|
| **Germany** | **~€15.5-17B** | ~94% building insurance | Profitable only 4x since 2002. Water damage >€4.5B/yr. €8.2B 2021 floods. | Very high (except HUK-Coburg motor-only) |
| **Netherlands** | ~€4.5-5.5B | ~90%+ | Property is LARGEST non-life line. Flood risk rising; EIOPA new 0.17% flood factor. | Very high |
| **Belgium** | ~€2.4-2.5B | ~95% | Nat cat mandatory in fire policies. 2021 Wallonia floods. | Very high |
| **Austria** | ~€2.0-2.5B | ~80-85% | >€1B weather damages 2023 | Very high |
| **Switzerland** | ~€2.5-3.5B | ~95-100% | **KGV monopoly in 19 cantons limits private market to ~80% of country** | High (limited by KGV) |
| **Ireland** | ~€1.8-2.0B | ~85-90% | Windstorm + flood exposure | Very high |
| **Sweden** | ~€3.5-4.0B | ~95% | Near-universal coverage. Forest fires increasing. | Very high |
| **Denmark** | ~€3.0-3.5B | ~90%+ | Stormradet mandatory storm scheme | Very high |
| **Finland** | ~€1.5-2.0B | ~80-85% | Flood gap >90% (worst Nordic coverage gap) | Very high |
| **Norway** | ~€2.5-3.0B | ~90%+ | **Naturskadepool mandatory; $218M deficit 2023** | Very high |
| **Poland** | ~€1.5-2.0B | **~49%** | **Major growth market — lowest penetration in EU-16** | Very high |
| **Czech Republic** | ~€1.3-1.5B | ~60-70% | Below Western EU average penetration | Very high |
| **Northern/Central EU Total** | **~€30-33B** | | | |

[SOURCE: mysa_product_strategy.md, Part 3f — Northern/Central EU table; market_landscape_overview.md, Section 5]

> [WEB SOURCE: GDV, Verbond van Verzekeraars, FSMA/Assuralia, VVO, VKG/SVV, Central Bank of Ireland, Svensk Forsakring, Finanstilsynet, Finanssiala, Naturskade.no, PIU, XPRIMM/CNB]
> [SOURCE: mysa_product_strategy.md, Part 3f]

**Key observations:**

- **Germany is the EU's largest property market** (~€15.5-17B) but is structurally unprofitable — only profitable 4 times since 2002. Water damage alone costs >€4.5B/year. Carriers here need decision efficiency the most. [SOURCE: mysa_product_strategy.md, Part 3f]
- **Poland (~49% penetration) is the EU's biggest growth market for property** — as penetration catches up to Western EU norms, claims volumes will multiply. [SOURCE: market_landscape_overview.md, Section 5]
- **Motor/property carrier overlap is "very high" in every Northern/Central EU country** — confirming the upsell thesis. [SOURCE: mysa_product_strategy.md, Part 3f]

---

### 4.2.3 EU Grand Totals

| Metric | Southern EU (4 countries) | Northern/Central EU (12 countries) | **All 16 EU Countries** |
|--------|--------------------------|-----------------------------------|------------------------|
| **Motor GWP** | €57.9B | ~€70-78B | **~€128-136B** |
| **Property GWP** | ~€24-28B | ~€30-33B | **~€54-61B** |
| **Combined GWP** | ~€82-86B | ~€100-111B | **~€182-197B** |
| **Caravela-tier carriers (€100-200M)** | 54-93 | 42-72 | **~96-165** |
| **Small carriers (€50-100M)** | 141-159+ | 63-101 | **~204-260+** |
| **Enterprise (>€1B — builds in-house)** | 16-19 | ~20-30 | **~36-49** |
| **Large (€200M-€1B)** | 30-47 | ~30-50 | **~60-97** |
| **Micro (<€50M)** | 243-372+ | 200-400+ | **~443-772+** |
| **Motor claims/year** | — | — | **~25-35M** |
| **Property claims/year** | — | — | **~16-20M** |

[SOURCE: mysa_product_strategy.md, Part 9a — "Full EU Totals" table; market_landscape_overview.md, Sections 4-5]

> The Northern EU market is LARGER in premium terms than Southern EU (€70-78B vs €57.9B) but has FEWER mid-market carriers in the Caravela tier. Germany alone is €30B but concentrated in large players. Southern EU has more fragmented markets = more mid-market targets. Convention systems in Southern EU provide the wedge, but Germany/Benelux/Nordics are the expansion that makes this a real company.
> [SOURCE: mysa_product_strategy.md, Part 9a — CLAUDE ANALYSIS]

---

## 4.3 US Market

The US is the largest single insurance market globally. Its structure differs fundamentally from the EU: no convention systems, a large TPA/MGA ecosystem, and much higher concentration in auto (but less in property). This section maps the US opportunity as an expansion market.

### US Market Structure

| Segment | Count | Premium/Revenue | Concentration |
|---------|-------|----------------|--------------|
| **Total P&C carriers** | ~4,116 entities | $1.06T DWP | Top 10 = 51.4%, Top 100 = ~90% |
| **Auto insurance** | — | **$359B** | **Top 5 = 63.6%** (extremely concentrated) |
| **Homeowners** | — | **$172.7B** (+13.7% YoY, 2024) | Top 25 = 78% (less concentrated) |
| **Commercial multi-peril** | — | $87B | More fragmented |
| **Workers' comp** | — | $65B | Fragmented |

[SOURCE: mysa_product_strategy.md, Part 9a — US Market comparison; validated via NAIC 2024 Market Share, AM Best, Conning, IBIS World]

### US Carrier Distribution by Size

| Tier (DWP) | Carrier Count | Profile | Mysa Fit |
|-----------|--------------|---------|---------|
| **>$5B** (top 25-30 groups) | ~25-30 | Build in-house — State Farm, GEICO, Progressive, Allstate, Liberty Mutual | **NO** |
| **$1B-$5B** | ~50-80 | Mix of build/buy — Cincinnati Financial, Hanover, Erie | Possible — longer cycles |
| **$100M-$500M** (Caravela-comparable) | **~200-350** | **Buy-not-build — can't afford data science teams** | **YES — primary** |
| **$50M-$100M** | ~150-250 | Lean operations, budget-conscious | YES — entry-level |
| **<$50M** | ~3,000+ | Micro carriers, regional, many inactive/run-off | Long-tail only |

[SOURCE: mysa_product_strategy.md, Part 9a — US Carrier Distribution table]

### US Non-Carrier Buyers (Unique to US)

The US has a large ecosystem of non-carrier buyers that does not exist at comparable scale in the EU. These entities process claims on behalf of carriers and represent a significant additional buyer pool.

| Buyer Type | Count (Material Size) | Why They Buy | Market Size |
|-----------|----------------------|-------------|------------|
| **TPAs** (P&C-focused) | ~500-800 | Process claims for carriers. Adjuster shortage + leakage pressure. Need efficiency tools. | ~$115B managed |
| **MGAs with claims authority** | ~330-550 | Fastest-growing segment (16% CAGR). Increasingly handle claims in addition to underwriting. | ~$114B managed premium |
| **Independent adjusting firms** | ~53,000 businesses | Workforce IS their product. Augmentation = survival. | $11.7B market |

[SOURCE: market_landscape_overview.md, Section 2 — US Non-Carrier Buyers; mysa_product_strategy.md, Part 9a]

> "Mid-tier TPAs buy rather than build. They have budget pressure (adjuster shortage, leakage, turnover)."
> [SOURCE: mysa_product_strategy.md, Part 3d — referencing RESEARCH Section 6]

### Total US Addressable Buyers

**~1,030-1,700** entities (carriers in $100M-$500M tier + material-size TPAs + MGAs with claims authority). [SOURCE: mysa_product_strategy.md, Part 9a]

### US Homeowners — Key Metrics

| Metric | Value | Source |
|--------|-------|--------|
| Total DWP | **$172.7B** (2024, +13.7% YoY) | NAIC |
| Claims/year | **~4.4-4.5M** (5.3% frequency on ~84M insured homes) | III/ISO |
| Total carriers writing homeowners | **~496** | IBISWorld |
| $100-500M tier (Caravela-comparable) | **~60-80 carriers** | NAIC/AM Best |
| Top 5 market share | **45.7%** (LESS concentrated than auto = 63.6%) | NAIC |
| Average claim size | **$17,059** (3.4x larger than auto's ~$5,000) | III |
| Xactimate usage | **~80% of property claims** | Verisk |

[SOURCE: mysa_product_strategy.md, Part 3f — US Homeowners Market table; market_landscape_overview.md, Section 5]

### Why Property, Not Auto, in the US

US auto is dangerously concentrated — the top 5 carriers (State Farm, GEICO, Progressive, Allstate, USAA) control 63.6% of the market. Mid-market carriers in auto are being squeezed. US homeowners, by contrast, is less concentrated (top 5 = 45.7%), with more of the market sitting in mid-market and regional carriers. **For Mysa, US entry should target homeowners/property mid-market carriers + TPAs, not US auto.** [SOURCE: mysa_product_strategy.md, Part 9a — CLAUDE ANALYSIS; Part 3d]

### Named US Mid-Market Carriers (Property-Strong)

Erie ($3.3B, tech-forward — invested in AI startups), Cincinnati Financial ($1.6B), Amica ($1.2B, "AI Trailblazer" — partnered with ZestyAI), NJM Insurance, Donegal Insurance Group, Secura, Shelter Insurance, Westfield Insurance, state farm bureaus (KY, NC, TX). Plus insurtechs: Hippo, Kin, SageSure. [SOURCE: mysa_product_strategy.md, Part 3f]

---

## 4.4 Why Bottom-Up: Mid/Small First, Not Enterprise

### The Enterprise Trap

> "For big carriers, it will be 'don't touch this. It's my turf. It's my logic. Build our own.'"
> — Jeremy Blehaut [TRANSCRIPT: Feb 7, 2026]

> "I always think about insurance companies as companies that have a data science team. But I think you are right." — Co-founder, after realizing mid-market carriers don't have dev teams [TRANSCRIPT: Feb 7, 2026]

Enterprise carriers (>€1B GWP / >$5B DWP) — Allianz, AXA, Generali, UnipolSai, Covea, State Farm, GEICO, Progressive — exhibit a consistent pattern:

**They build in-house. Badly.**

- Allianz launched "Insurance Copilot" in Austria in 2024. Key insight: they built it in-house for themselves, not as a product for other insurers. [SOURCE: mysa_product_strategy.md, Part 3a — referencing competitive_landscape_reality_check.md]
- BCP (Portugal's largest bank) has an in-house Copilot. Direct observation from co-founder's girlfriend who works there: "It's very bad." [TRANSCRIPT: Feb 7, 2026]

Even when enterprise builds are bad, the institutional bias is still "my turf, my logic." Selling to enterprise means:

| Enterprise Characteristic | Impact on Mysa |
|--------------------------|---------------|
| 12-month procurement cycles | Burns cash with no revenue during sales cycle |
| Enterprise procurement committees | 8-15 stakeholders instead of 1-2 decision-makers |
| RFP processes | Commoditizes Mysa's unique value into a feature checklist |
| Internal build bias | Carrier believes they can do it themselves (even when they can't) |
| Existing vendor lock-in | Guidewire, Duck Creek, CCC already entrenched — adding another vendor feels risky |
| Customization demands | "We're different" — enterprise expects bespoke, not product |

[SOURCE: mysa_product_strategy.md, Part 3a — enterprise vs mid-market analysis; CLAUDE ANALYSIS]

### Why Mid/Small Works

> "For the mid-market ones like Caravela, they want us."
> — Jeremy Blehaut [TRANSCRIPT: Feb 7, 2026]

Mid-market carriers (€100-200M GWP, ~100-200 employees) are the opposite of enterprise on every dimension that matters for an early-stage company:

| Mid-Market Characteristic | Why It Matters |
|--------------------------|---------------|
| **Can't build it** | No data science team. No AI/ML engineers. 100-200 total employees — they don't have the talent to build claims AI. |
| **Want to buy it** | Growing fast (Caravela grew 10x in 10 years). Need tools to scale without proportional headcount growth. |
| **Fast decisions** | 1-2 decision-makers (VP Claims + CEO/COO). No procurement committee. No 12-month RFP process. |
| **No procurement bureaucracy** | Call, demo, pilot, contract. 3-6 month sales cycle vs 12-18 months for enterprise. |
| **Budget exists** | €50K-200K/year is 0.03-0.2% of GWP — trivial if it improves STP or reserve accuracy. |
| **Pain is acute** | Growing claims volume with flat headcount. Adjusters drowning. Institutional knowledge walking out the door. |
| **Reference customers** | Happy mid-market customers create peer pressure in tight insurance communities. Word of mouth in a market of 300-500 carriers. |

[SOURCE: mysa_product_strategy.md, Part 3a — "Why Caravela tier is the sweet spot"; market_landscape_overview.md, Section 2]

### Bottom-Up Expansion Path

The strategy is not "stay mid-market forever." It is:

1. **Win mid-market** (€100-200M, Caravela tier) — prove product-market fit, build data moat
2. **Expand to small** (€50-100M) — entry-level pricing, same product
3. **Move up to large** (€200M-€1B) — with customer proof points and data, large carriers become "better than what you built internally"
4. **Eventually serve enterprise** — but only from a position of strength, with a proven product and hundreds of mid-market deployments

> Even the large carriers that build in-house are building BAD copilots. The co-founder's direct observation: internal tools are document retrieval, not decision support. Mysa could eventually sell to large carriers as "better than what you built internally" — but that's Phase 3, not Phase 1.
> [SOURCE: mysa_product_strategy.md, Part 3a — CLAUDE ANALYSIS]

---

## 4.5 Caravela Tier Sweet Spot

### The Anchor: Caravela Seguros

| Metric | Value |
|--------|-------|
| GWP (2024) | €188M |
| Employees | 149 |
| Total claims/year | ~57K (42K motor + ~15K property) |
| Ranking | 7th in Portuguese non-life |
| Growth | 10x in 10 years |
| Property growth | +31% (fastest-growing line) |
| Data science team | **None** |

[SOURCE: market_landscape_overview.md, Section 6 — Anchor: Caravela Seguros; WEB: Caravela 2024 Annual Report, ECO rankings, ASF data]

Caravela is the archetype of the target customer: a mid-market carrier with real claims volume (57K/year), rapid growth (10x in a decade), zero in-house AI capability (149 employees, no data science team), and acute operational pressure (growing claims with flat headcount). It is also Mysa's design partner.

### Why €100-200M GWP Is Optimal

1. **Real claims volume** (~30K-60K claims/year) justifies the technology investment. A carrier processing 5K claims/year doesn't need a decision engine. One processing 40K does. [SOURCE: mysa_product_strategy.md, Part 3a]

2. **No data science team** — at 100-200 employees, there is no room for ML engineers, data scientists, or AI specialists. They must buy, not build. [SOURCE: mysa_product_strategy.md, Part 3a]

3. **Growth pressure** — many Caravela-tier carriers are growing fast (Caravela: 10x in 10 years, UNA motor +26%). They need tools to scale without hiring proportionally. [SOURCE: market_landscape_overview.md, Section 6]

4. **Budget exists** — €50K-200K/year is 0.03-0.2% of GWP. Trivial if it improves STP rates or reserve accuracy. Compare to a single adjuster's fully loaded cost (~$110K/year). [SOURCE: mysa_product_strategy.md, Part 3a]

5. **Fast decision-making** — 1-2 decision-makers (not a procurement committee). 3-6 month sales cycle. [SOURCE: mysa_product_strategy.md, Part 3a]

### Named Caravela-Tier Carriers by Market

| Country | Carrier | Estimated GWP | Notes |
|---------|---------|---------------|-------|
| **Portugal** | **Caravela** | €188M (2024) | Design partner. 7th non-life. 42K motor claims. |
| Portugal | CA Seguros | ~€200-210M | 8th, displaced by Caravela |
| Portugal | Mapfre PT | ~€190-210M | 9th, surge with Bankinter partnership |
| Portugal | Aegon Santander | ~€170-190M | 10th, health +37.5% |
| Portugal | Victoria | ~€130-150M | 11th, strong in health |
| Portugal | UNA | ~€120-140M | 12th, health +53%, motor +26% |
| **Spain** | Pelayo | ~€375M (mutua) | 844K auto policies, 2.42% motor share |
| Spain | Admiral/Balumba | ~€100-150M motor | UK-owned direct writer, +13.4% |
| Spain | Patria Hispana | ~€100-130M | Centennial company, +12.9% |
| Spain | Mutua Tinerfena | ~€80-120M | Regional Canary Islands mutual |
| **France** | Thelem Assurances | €453M total (~€150-200M motor) | 1.15M contracts. **Closest French analog to Caravela.** |
| France | L'Olivier Assurance | ~€220-260M | Online auto pure-play. Similar growth profile to Caravela. |
| France | Direct Assurance (AXA sub) | ~€300-400M | Slightly larger than Caravela tier |
| France | ~30-60 small mutuelles | €82-200M each | ACPR 2nd quartile. Many are autonomous, multi-line with motor books. |
| **Italy** | HDI Assicurazioni | €716M non-life, ~€160-200M motor | R.C. Auto = 22.8% of non-life. **Closest Italian analog to Caravela.** |
| Italy | ~10-12 smaller carriers | €50-200M motor | Regional companies, online insurers (Prima, Quixa, Verti, Linear) |

[SOURCE: mysa_product_strategy.md, Part 3c — Caravela-Tier Deep Dive; market_landscape_overview.md, Section 6]

> [WEB SOURCE: Caravela 2024 Annual Report; ASF; ECO Sapo rankings; MAPFRE Economics; France Assureurs; IVASS/ANIA]
> [SOURCE: mysa_product_strategy.md, Part 3c]

---

## 4.6 Mid-Market vs Small: Different Needs

Carriers in the €100-200M range (Caravela tier) and carriers in the €50-100M range (small tier) share the core problem — they can't build AI in-house — but their buying behavior, data maturity, and budget constraints differ meaningfully.

### By Carrier Size

| Dimension | Caravela Tier (€100-200M) | Small Tier (€50-100M) |
|-----------|--------------------------|----------------------|
| **Employees** | ~100-200 | <100 |
| **Claims/year** | ~30K-60K | ~15K-30K |
| **Data infrastructure** | Basic CMS (often legacy or homegrown). Some have Guidewire/Duck Creek. Digital records exist but may be inconsistent. | Minimal. May still use paper-heavy processes. Some have no CMS at all — spreadsheets and email. |
| **Decision-maker** | VP Claims or CCO (dedicated role) | CEO or COO wearing multiple hats. Claims may report to a general operations head. |
| **Budget for claims tech** | €50K-200K/year | €10K-100K/year |
| **Pricing sensitivity** | Moderate — ROI-driven. Will pay if value is demonstrated. | High — tight budgets, every euro scrutinized. Per-claim pricing preferred over platform fees. |
| **Sales cycle** | 3-6 months | 1-3 months (simpler decision, lower stakes) |
| **Onboarding complexity** | Medium — need to ingest SOPs, connect to existing CMS, configure workflows. Historical data may be available. | Low — simpler SOPs (or no formal SOPs), fewer integrations, less historical data. |
| **Strategic value to Mysa** | High — reference customers, meaningful data volume, case studies | Moderate — volume play, proves broad applicability, lower ACV |

[SOURCE: mysa_product_strategy.md, Part 3a — carrier segmentation; Part 3e — pricing model; market_landscape_overview.md, Section 2]

### By Line of Business

| Dimension | Motor | Property |
|-----------|-------|----------|
| **EU mid-market data maturity** | Higher — convention systems create structured data standards (EAS forms, convention codes). Carriers have been digitizing motor for years. | Lower — no convention systems, less standardized data. Property claims often documented in free-text reports, photos, and vendor estimates. |
| **US mid-market data maturity** | Higher — CCC/Mitchell integration widespread. Structured auto claims data. | Mixed — Xactimate used by ~80% for estimation, but coverage determination and causation remain largely unstructured. |
| **Pricing sensitivity (EU)** | Lower — motor is the bread-and-butter line. Carriers understand the ROI of motor claims efficiency. | Higher — property is often a secondary line for motor-primary carriers. Budget may be tighter for property-specific tools. |
| **Pricing sensitivity (US)** | Higher — auto mid-market is being squeezed by top 5 carriers. Less room for new tools. | Lower — property is growing rapidly (+13.7% YoY). Carriers have acute pressure from cat losses and need tech solutions. |

[SOURCE: mysa_product_strategy.md, Part 3f — motor vs property comparison; market_landscape_overview.md, Section 3]

### By Region

| Dimension | EU Mid-Market | US Mid-Market |
|-----------|--------------|--------------|
| **Primary buyer type** | Carriers (direct) | Carriers + TPAs + MGAs (three buyer types) |
| **TPA ecosystem** | Small — most carriers handle claims in-house | Large — ~500-800 material TPAs, many handling claims for multiple carriers |
| **Convention system value** | High — differentiator in Southern EU, partial in Northern EU | None — no convention systems in the US |
| **Regulatory complexity** | Per-country regulation (16 different frameworks), GDPR, EU AI Act | Per-state regulation (50 states + DC), more litigious environment |
| **Sales motion** | Relationship-driven, conference-based, language/cultural barriers per market | More standardized, English-only, larger conference ecosystem (ITC, RIMS) |
| **Competitive density** | Low (90-95% of mid-market has no claims AI) | Moderate (75-85% open, but more competitors active — Five Sigma, Hi Marley) |

[SOURCE: mysa_product_strategy.md, Parts 3a, 3d, 9a — market openness by segment]

---

## 4.7 Motor + Property Overlap

### The Same Buyers

**80-95% of carriers that write motor also write property.** This is validated across all 16 EU countries and the US. [SOURCE: market_landscape_overview.md, Section 3; mysa_product_strategy.md, Part 3f]

Caravela itself illustrates the overlap: €188M total GWP, of which motor is the primary line (42K motor claims) but property is the fastest-growing (+31%), with approximately 15K property claims per year. The same VP Claims manages both lines. The same adjusters often handle both (though specialization increases with carrier size). [SOURCE: market_landscape_overview.md, Section 6]

The Northern/Central EU data confirms this universally:

| Country | Motor/Property Carrier Overlap |
|---------|-------------------------------|
| Germany | Very high (except HUK-Coburg motor-only) |
| Netherlands | Very high |
| Belgium | Very high |
| Austria | Very high |
| Switzerland | High (limited by KGV cantonal monopolies) |
| Ireland | Very high |
| Sweden | Very high |
| Denmark | Very high |
| Finland | Very high |
| Norway | Very high |
| Poland | Very high |
| Czech Republic | Very high |

[SOURCE: mysa_product_strategy.md, Part 3f — Northern/Central EU property table, carrier overlap column]

### The Same Workflow (~80% Identical)

The adjusting process for property is nearly identical to motor — the same 6 decision sub-steps apply:

| Decision Sub-Step | Motor | Property | Overlap |
|-------------------|-------|----------|---------|
| **Coverage verification** | "Is this accident covered under the policy?" | "Is this water damage / fire / storm covered under the policy?" | ~90% identical |
| **Policy check** | Check policy terms, exclusions, deductibles | Check policy terms, exclusions, deductibles, named vs open perils | ~80% identical (property adds causation) |
| **Repair assessment** | Damage assessment via photos, inspection | Damage assessment via photos, inspection, contractor scopes | ~85% identical |
| **Cost analysis** | Audatex/CCC estimates, parts pricing | Xactimate estimates, material pricing, contractor bids | ~70% identical (different estimation tools) |
| **Reserve calculation** | Historical comparison, severity bands | Historical comparison, severity bands, cat exposure | ~85% identical |
| **Fraud detection** | Pattern matching, staged accident indicators | Pattern matching, inflated claims indicators, pre-existing damage | ~80% identical |

[SOURCE: mysa_product_strategy.md, Part 3f — "the adjusting process for property is nearly identical to motor — the same 6 decision sub-steps"]

The key difference is in the **decision itself**: motor asks "WHO caused it?" (fault allocation, often determined by convention systems). Property asks "WAS it covered?" (policy interpretation, causation analysis — sudden vs gradual for water damage, named peril vs open peril). This means the AI modules are different, but the workflow architecture, data model, and user experience are ~80% shared. [SOURCE: market_landscape_overview.md, Section 3]

### Revenue Uplift: +60-70% Per Carrier, Zero New Acquisition

| Scenario | Motor-Only TAM | Motor + Property TAM | Uplift |
|----------|---------------|---------------------|--------|
| EU mid-market only | €50-100M | **€80-170M** | **+60-70%** |
| EU + US mid-market | €100-250M | **€160-425M** | **+60-70%** |
| Full addressable | €200-650M | **€320M-1.1B** | **+60-70%** |

[SOURCE: mysa_product_strategy.md, Part 3f — "Revenue impact of adding property to motor"]

> Adding property doesn't require new buyers — it requires new AI modules (coverage determination, causation analysis) applied to the **same carrier relationships**. The carrier overlap is 80-95% across all 16 EU countries and the US.
> [SOURCE: mysa_product_strategy.md, Part 3f]

Caravela reference: at €188M GWP, 57K total claims/year = 42K motor (74%) + ~15K property (26%). French carriers are closer to 50/50 motor/property. Average across the EU: property claims = ~30-50% of motor per multi-line carrier. [SOURCE: mysa_product_strategy.md, Part 3f]

---

## 4.8 TAM Calculations

All TAM calculations are built bottom-up from validated carrier counts, anchored to Caravela's actual economics (€188M GWP, 57K claims/year, 149 employees). No top-down percentages of "total insurance market." Every number maps to a countable set of carriers.

### EU Carrier Size Distribution (Full Segmentation)

| Size Tier | GWP Range | EU Count (16 countries) | Tech Approach | Mysa Addressable? |
|-----------|----------|------------------------|---------------|-------------------|
| **Enterprise** | >€1B | ~36-49 groups | Build in-house (Allianz, AXA, Generali, UnipolSai, Covea all building own) | NO — Phase 3+ |
| **Large** | €200M-€1B | ~60-97 | Buy best-of-breed or outsource to TPA | YES — longer cycles |
| **Caravela tier** | €100-200M | **~96-165** | **Need it, can't build it. ~100-200 employees.** | **PRIMARY TARGET** |
| **Small** | €50-100M | **~204-260+** | Want tech, tight budget, <100 employees | YES — entry pricing |
| **Micro** | <€50M | ~443-772+ | Manual processes, minimal tech, <50 staff | LONG-TAIL only |

[SOURCE: mysa_product_strategy.md, Part 9a — Full EU Totals; market_landscape_overview.md, Section 2]

### US Carrier Distribution (For Comparison)

| Size Tier | DWP Range | US Count | Mysa Fit |
|-----------|----------|---------|---------|
| **Top 25-30** | >$5B | ~25-30 | NO — build in-house |
| **Large** | $1B-$5B | ~50-80 | Possible — longer cycles |
| **Caravela-comparable** | $100-$500M | **~200-350** | **YES — buy-not-build** |
| **Small** | $50-$100M | ~150-250 | YES — budget-conscious |
| **Micro** | <$50M | ~3,000+ | Mixed — many mono-line or inactive |

[SOURCE: mysa_product_strategy.md, Part 9a — US Carrier Distribution]

### Target Segment Claims Volume

| Segment | Carriers | Motor Claims | Property Claims | **Combined Claims** |
|---------|---------|-------------|----------------|-------------------|
| **Caravela tier (€100-200M) — EU** | 96-165 | 2.9-7.4M | 1.2-4.1M | **4.1-11.5M** |
| **Small tier (€50-100M) — EU** | 204-260 | 2.4-6.5M | 1.0-3.1M | **3.4-9.6M** |
| **US mid-market ($100-500M) + TPAs** | 60-80 carriers + 500-800 TPAs | ~3-5M | ~1-2M | **~4-7M** |
| **TOTAL TARGET** | **360-505 carriers + TPAs** | **~8-19M** | **~3-9M** | **~11-28M claims/year** |

[SOURCE: market_landscape_overview.md, Section 6 — Target Segment Claims Volume; mysa_product_strategy.md, Part 3f]

### Target as Percentage of Total Market

| | Motor | Property | Combined |
|--|-------|----------|---------|
| **Target segment** | ~8-19M | ~3-9M | **~11-28M** |
| **Total market** | ~60-70M | ~20-25M | ~80-95M |
| **Target as %** | ~15-27% | ~15-36% | **~14-29%** |

[SOURCE: market_landscape_overview.md, Section 6 — "Target as % of Total Market"]

This is the right size for a focused startup: **large enough to build a $100M+ ARR business, small enough that enterprise competitors (Shift, CCC, Guidewire) aren't competing for the same buyers.** [SOURCE: mysa_product_strategy.md, Part 3f — CLAUDE ANALYSIS]

### TAM Scenarios — Motor Only (Bottom-Up from Validated Carrier Counts)

| Scenario | EU Carriers | US Buyers | Total Buyers | ACV Range | **Revenue Range** |
|----------|------------|-----------|-------------|-----------|-------------------|
| **Conservative** — Southern EU Caravela tier only | 54-93 | — | 54-93 | €50-200K | **€2.7-€18.6M** |
| **Base** — All EU €50-200M carriers | 300-425 | — | 300-425 | €30-200K | **€25-55M** |
| **EU + large tier** — Add €200M-1B | 360-520 | — | 360-520 | €30-500K | **€50-100M** |
| **EU + US mid-market** — Add US $100-500M carriers + TPAs + MGAs | 360-520 | 1,030-1,700 | 1,530-2,400 | €10K-2M | **€200-650M** |

[SOURCE: mysa_product_strategy.md, Part 9b — Motor TAM table]

### TAM Scenarios — Motor + Property Combined (Same Buyers, +60-70% Revenue)

| Scenario | Motor TAM | + Property TAM | **Combined TAM** |
|----------|----------|---------------|-----------------|
| **Conservative** — Southern EU Caravela tier | €2.7-€18.6M | +€1.6-€13M | **€4.3-€31.6M** |
| **Base** — All EU €50-200M | €25-55M | +€15-38M | **€40-93M** |
| **EU + large** | €50-100M | +€30-70M | **€80-170M** |
| **EU + US mid-market** | €100-250M | +€60-175M | **€160-425M** |
| **Full addressable** | €200-650M | +€120-455M | **€320M-1.1B** |

[SOURCE: mysa_product_strategy.md, Part 9b — Motor + Property TAM table]

### The Honest TAM Narrative

> [TRANSCRIPT — Jeremy]: "It's like 700 mid-market players in Europe. That makes less than 500 million of... insurance, like Caravela style."
> [SOURCE: mysa_product_strategy.md, Part 3c]

The Southern EU motor market alone is **NOT a venture-scale TAM**. At base case (~€15-25M), it is a healthy SaaS business but not a $1B+ outcome. The venture story requires:

1. Expanding to all of EU including Northern markets
2. Expanding to the US
3. Expanding from motor to property
4. Moving up-market over time

EU motor is the **wedge**, not the company. [SOURCE: mysa_product_strategy.md, Part 3c — CLAUDE ANALYSIS]

**But as a wedge, it is perfect:**
- 54-93 carriers in the primary tier = reachable with 2-3 sales reps
- Caravela as design partner proves the product in a live environment
- Convention system expertise creates a defensible moat
- Every carrier added builds the historical data flywheel
- Technology transfers directly to property and US markets

[SOURCE: mysa_product_strategy.md, Part 3c]

### The Fundraising TAM Story

| Stage | TAM | What It Represents |
|-------|-----|-------------------|
| **Wedge TAM** (EU motor, Caravela tier) | €2.7-€18.6M | Proves the product works. Not venture-scale alone. |
| **Year 2-3 TAM** (all EU mid-market motor + property) | €80-170M | Real SaaS business. |
| **Year 3-5 TAM** (EU + US mid-market, both lines) | €160-425M | Venture-scale. |
| **Vision TAM** (full addressable + expansion) | €320M-1.1B | IPO-scale. |

[SOURCE: mysa_product_strategy.md, Part 9b — "The honest TAM story for fundraising"]

> "We start with EU motor — the convention system wedge that nobody else has. Within 6 months, the same carrier pays us for property too (same AI, bigger problem, same buyer). By year 3, we're in the US with the same product. The market is ~11-28M claims/year in our target segment alone, 80-95M globally. And 90%+ of mid-market carriers have ZERO AI claims tools today."
> [SOURCE: mysa_product_strategy.md, Part 9b]

### Market Openness — Why This TAM Is Actually Accessible

| Segment | Total Entities | Using Claims AI | % Open | Mysa Opportunity |
|---------|---------------|----------------|--------|-----------------|
| **All carriers globally (EU + US)** | ~6,300+ | ~400-600 (~7%) | **~93% open** | Massive whitespace |
| **EU mid-market (€50-200M)** | ~300-425 | <30 (Shift = large carriers, Bdeo = visual only) | **~90-95% open** | **Primary target — virtually untouched** |
| **US mid-market ($100-500M)** | ~200-350 | ~30-50 (Five Sigma + Hi Marley customers) | **~75-85% open** | Strong — but competitors more active |
| **TPAs globally** | ~500-800+ | ~50-80 (Shift, ClaimSorted) | **~85-90% open** | Good expansion target |
| **MGAs with claims authority** | ~330-550 | <20 | **~95% open** | Emerging segment, growing fast |

[SOURCE: mysa_product_strategy.md, Part 9a — "Competitor Adoption — How Open Is the Market?"]

> Only 4% of insurers have SCALED AI in claims. Most "adoption" is pilots, POCs, or single-feature tools (Bdeo = photos only, Hi Marley = texting only). Nobody has deployed an AI decision engine at scale. [WEB: McKinsey 2025 insurance survey]
> [SOURCE: mysa_product_strategy.md, Part 9a]

---

## Sources

| Source | Type | Sections Used |
|--------|------|--------------|
| `market_landscape_overview.md` | Primary — validated market data compilation | 4.1, 4.2, 4.3, 4.5, 4.7, 4.8 |
| `mysa_product_strategy.md` Part 3a | Primary — segmentation, enterprise vs mid-market | 4.4, 4.5, 4.6, 4.8 |
| `mysa_product_strategy.md` Part 3b-3c | Primary — total market sizing, country-level data | 4.2, 4.3, 4.8 |
| `mysa_product_strategy.md` Part 3d | Primary — expansion markets, US entry strategy | 4.2, 4.3, 4.6 |
| `mysa_product_strategy.md` Part 3e | Primary — pricing model | 4.6 |
| `mysa_product_strategy.md` Part 3f | Primary — property market, overlap analysis, revenue uplift | 4.2, 4.7, 4.8 |
| `mysa_product_strategy.md` Part 9a | Primary — fundraising narrative, full EU country-by-country, US comparison, market openness | 4.2, 4.3, 4.8 |
| `mysa_product_strategy.md` Part 9b | Primary — revised TAM calculations | 4.8 |
| Feb 7 Granola call — Mid-market strategy | Transcript | 4.4 (enterprise vs mid-market quotes) |
| MODULE_01_POSITIONING.md | Reference — ICP segmentation, carrier table | 4.4, 4.5 (cross-reference) |
| EIOPA, BaFin, ACPR, IVASS, ASF, DGSFP, DNB, FSMA, FMA, FINMA, Central Bank of Ireland, FI Sweden, FSA Denmark, FIN-FSA, Finanstilsynet, KNF, CNB | Regulatory sources (via agent research) | 4.2 |
| NAIC 2024 Market Share, AM Best, Conning, IBIS World | US market sources (via agent research) | 4.3, 4.8 |
| France Assureurs 2024, ICEA 2024, UNESPA, ANIA, GDV | Industry body sources (via agent research) | 4.2 |
| McKinsey 2025 insurance survey | Web source — AI adoption rate | 4.8 |
| Caravela 2024 Annual Report, ECO Sapo rankings | Web sources — anchor carrier data | 4.5 |

---

# Part 5: Competitive Landscape

# Module 5: Competitive Landscape

**Status:** DRAFT v1.0
**Last updated:** February 9, 2026
**Feeds:** Pitch deck competition slides, investor Q&A preparation, sales battle cards, product roadmap prioritization, co-founder strategic alignment

---

## How to Read This Module

This is not a marketing document. It is an investor-grade competitive analysis designed to be honest about where Mysa wins, where it loses, and where the risks are existential. Every claim is sourced. Where data is thin, that is stated. The goal is to arm the founders with the truth -- not to sell a story.

For readers new to insurance technology: each competitor section explains what the company actually does in plain language before analyzing its relevance to Mysa.

---

## 5.1 Where NOT to Go -- The Crowded Zones

Three areas of claims AI have attracted massive capital. Mysa should not compete here directly. These are well-funded, well-defended, and increasingly commoditized.

### Intake Automation (~$1B+ in combined funding)

Intake automation means digitizing the "front door" of claims -- the moment a policyholder reports a loss. It covers FNOL (First Notice of Loss), document parsing, chatbots, data extraction, and initial triage.

**Who is here:**
- **Assured** -- reported $1B valuation (March 2025, ICONIQ Capital + Kleiner Perkins), AI agent "Emma" handles 70% of interactions autonomously, 50M+ customer interactions for the largest US insurers [SOURCE: home_property_competitive_deep_dive.md, Section 4]
- **FurtherAI** -- $30M raised (a16z), "AI workforce for insurance," claims 30x faster intake and 95% accuracy [SOURCE: mysa_product_strategy.md, Part 4d]
- **Avallon** -- $4.6M seed (YC S25), AI agents for calls, emails, document triage, 10x revenue growth during YC [SOURCE: home_property_competitive_deep_dive.md, Section 5]
- **Sprout.ai** -- ~$38M raised, document AI with 98% accuracy, 100+ languages, Zurich UK and AdvanceCare as customers [SOURCE: Sprout_ai_vs_Omnius_Deep_Research.md]
- **Strada** -- YC-backed, voice AI agents for FNOL [SOURCE: competitive_landscape_reality_check.md]

**Why to avoid:** Over $1B in combined funding is chasing the same admin automation layer. These companies are fighting for the same buyer (VP Claims) with the same pitch ("faster document processing"). The category is getting crowded fast, and differentiation is collapsing toward commodity features. [SOURCE: competitive_landscape_reality_check.md; home_property_competitive_deep_dive.md, Section 16]

> "Everyone is fighting over intake and admin. Assured, FurtherAI, Avallon, Sprout.ai, Strada -- all competing to automate FNOL, document processing, and data entry."
> [SOURCE: home_property_competitive_deep_dive.md, Section 19]

### Fraud Detection (~$320M+ in dedicated funding)

Fraud detection uses ML and pattern matching to identify suspicious claims -- fake invoices, staged accidents, organized fraud rings.

**Who is here:**
- **Shift Technology** -- $320M raised, $1B+ valuation, 100+ insurers, 25+ countries, nearly 2 billion claims analyzed. Fraud detection is their DNA (10+ years). Insurance Data Network (IDN) enables cross-carrier fraud data sharing. [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md]
- **FRISS** -- Established EU fraud detection vendor
- **SAS** -- Enterprise analytics vendor with insurance fraud modules

**Why to avoid:** Shift has a 10-year head start, 2 billion claims of training data, and the Insurance Data Network (a cross-carrier data sharing platform where 4 of the top 5 US P&C insurers are members). Fraud detection has genuine network effects -- the more carriers share data, the better the system gets. A startup cannot replicate this. Mysa's fraud signal agent can flag anomalies as one of its six decision sub-steps, but fraud detection should not be the primary positioning. [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md, Part 2]

### Estimation Tools (Verisk = $35B+ market cap)

Estimation means calculating the cost to repair physical damage -- what materials are needed, what labor costs, what the regional price should be.

**Who is here:**
- **Verisk/Xactimate** -- 75-80% of all US property claims use Xactimate for estimation. $35B+ market cap public company. [SOURCE: mysa_product_strategy.md, Part 4b]
- **CCC Intelligent Solutions** -- $13B+ market cap, dominates US auto estimation. Acquired EvolutionIQ for $730M. [SOURCE: competitive_landscape_reality_check.md]
- **Solera/Audatex** -- EU motor estimation monopoly. 4.5B+ vehicle damage images. [SOURCE: home_property_competitive_deep_dive.md, Section 20]
- **Cotality/CoreLogic (Symbility)** -- Distant #2 to Xactimate in US property [SOURCE: home_property_competitive_deep_dive.md, Section 3]

**Why to avoid:** These are entrenched monopolies with decades of data. Competing with Xactimate on estimation is "essentially impossible." [SOURCE: home_property_competitive_deep_dive.md, Section 15] The correct strategy is to build AROUND these tools (as a decision layer that uses estimation data as input), not against them.

### The Takeaway

> "Not FNOL (crowded). Not estimation (Verisk's moat). Not auto casualty guidance (CCC's moat). The coverage to triage to investigation to reserve workflow for mid-market buyers who use Xactimate for pricing but have nothing for deciding."
> [SOURCE: home_property_competitive_deep_dive.md, Section 19]

---

## 5.2 Where Mysa Wins -- The Unoccupied Territory

Four areas of claims technology have effectively zero competition. These are Mysa's primary battleground.

### Convention Systems (Zero Competition -- Confirmed)

**What convention systems are:** In EU motor claims, standardized protocols (IDS in Portugal, IRSA in France, CARD in Italy, CIDE/ASCIDE/CICOS in Spain) define rules for which insurer pays in multi-party accidents. When two drivers fill out a European Accident Statement (EAS) form, the checkboxes and diagram can be matched against a convention lookup table to determine fault percentage -- deterministically, without human judgment. These systems could theoretically auto-resolve 60-70% of motor claims. In practice, only ~10% achieve straight-through processing (STP). [SOURCE: mysa_product_strategy.md, Part 2b; MODULE_01_POSITIONING.md, Section 1.2]

**The gap:** The STP gap exists because the data going INTO the convention system is garbage. Paper EAS forms with shaky handwriting and unclear checkboxes need to be digitized, structured, and validated before the convention lookup can work. Nobody is building this pipeline -- not Shift, not Solera, not Tractable, not Bdeo, not Five Sigma. [SOURCE: home_property_competitive_deep_dive.md, Section 20]

**Competition check (across all sources):**
- Five Sigma/Clive: "No evidence whatsoever" of EU convention system support [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md]
- Shift Technology: "IRSA, CARD, IDS, and CIDE convention system support is NOT explicitly documented anywhere" [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md]
- omni:us: "No specific EU convention system support confirmed" [SOURCE: Sprout_ai_vs_Omnius_Deep_Research.md]
- Sprout.ai: "No explicit confirmation" of EAS processing [SOURCE: Sprout_ai_vs_Omnius_Deep_Research.md]
- Assured: No EU operations at all [SOURCE: home_property_competitive_deep_dive.md, Section 4]

**Mysa's position:** Convention matching is built for Portugal (IDS/CIMPAS rules encoded, 91% inter-insurer agreement rate). The OCR engine (Caravela) reads EAS forms at 81.5% normalized accuracy. This is the wedge product. [SOURCE: MODULE_01_POSITIONING.md, Section 1.6; CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md]

### Coverage Determination (~99% Empty)

**What coverage determination is:** Reading a policy, matching it against claim facts, and determining "is this covered?" This includes interpreting exclusions, sub-limits, endorsements, and making judgment calls on ambiguous situations (e.g., "was this water damage sudden and accidental, or gradual from deferred maintenance?"). [SOURCE: home_property_competitive_deep_dive.md, Section 21]

**Competition check:**
- Crawford CoverAI: The closest competitor. AI-driven policy coverage review. BUT: absorbed back into Crawford's TPA stack (Turvi standalone brand failed), limited external traction, no causation analysis. Not available as a standalone product. [SOURCE: mysa_product_strategy.md, Part 3c; home_property_competitive_deep_dive.md, Section 19]
- Five Sigma/Clive: "LLM coverage matching is fragile -- uses LLM to read policies, breaks on complex exclusions, nested clauses" [SOURCE: mysa_product_strategy.md, Part 4a]
- Wamy: Launched from stealth December 2025, claims to validate coverage, but brand new and pre-traction [SOURCE: mysa_product_strategy.md, Part 3c]
- Everyone else: Nobody [SOURCE: market_landscape_overview.md]

| Market Segment | Openness | Evidence |
|----------------|----------|---------|
| EU mid-market | 90-95% open | Only 4% of insurers have scaled claims AI |
| US mid-market | 75-85% open | Top carriers building in-house; mid-market buying |
| Property decision AI | ~99% open | Crawford CoverAI reabsorbed; Wamy pre-traction; nobody else trying |

[SOURCE: market_landscape_overview.md]

### SOP-Driven Workflows (Nobody Does Carrier-Specific)

**What SOP-driven workflows are:** Standard Operating Procedures are the rules each carrier's adjusters are supposed to follow. Different carriers have different authority levels, different investigation triggers, different reserve thresholds, different documentation requirements. A workflow system that encodes these per-carrier rules turns tribal knowledge into repeatable process. [SOURCE: MODULE_01_POSITIONING.md, Section 1.1]

**Competition check:**
- Five Sigma/Clive: Uses "pre-defined investigation workflows per claim type" -- generic playbooks, not carrier-specific SOPs. "Routing quality depends entirely on the insurer's SOP configuration -- Clive follows rules, it does not independently optimize assignment." [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md, Phase 1; mysa_product_strategy.md, Part 4a]
- Shift Technology: "Limited workflow customization" and "no SOP-driven workflows" [SOURCE: mysa_product_strategy.md, Part 4c]
- Assured: Flow Builder allows "low-code customization of question sequences by LOB/location" -- configurable but not SOP-encoded [SOURCE: home_property_competitive_deep_dive.md, Section 4]
- Nobody else: No competitor encodes carrier-specific SOPs into decision workflows

**Mysa's advantage:** Once a carrier's SOPs are encoded into Mysa, switching costs become prohibitive. The SOPs are the carrier's institutional knowledge -- migrating them to a competitor would require re-encoding months of work. This is the lock-in mechanism. [SOURCE: mysa_product_strategy.md, Part 1]

### Decision Ground Truth (New Data Category)

**What decision ground truth is:** Capturing not just what was decided on a claim, but WHY the adjuster decided it. Every accept/modify/reject creates training data. Over time, this builds a dataset that no competitor has: adjuster decision reasoning linked to outcomes. [SOURCE: MODULE_01_POSITIONING.md, Section 1.1]

**Competition check:**
- CCC/Verisk have claim OUTCOMES -- what was paid. They do not have decision REASONING -- why it was paid.
- Five Sigma: "Doesn't systematically capture WHY adjusters decide" [SOURCE: mysa_product_strategy.md, Part 4a]
- Nobody else captures this data

> "CCC and Verisk have claim outcomes. Anthropic and OpenAI have general intelligence. We have adjuster decision reasoning."
> [SOURCE: MODULE_01_POSITIONING.md, Section 1.8]

---

## 5.3 Five Sigma / Clive -- The Closest Competitor

> "I also care a lot about them [Five Sigma]. For me, they are still my main competitor, and I'm trying to find ways to win."
> -- Tiago Brigido, Co-founder [TRANSCRIPT: Feb 7, 2026]

> "But I think they're everywhere and nowhere at the same time."
> -- Jeremy Blehaut, Co-founder [TRANSCRIPT: Feb 7, 2026]

### What Five Sigma Actually Does

Five Sigma is an Israeli-founded company (HQ: Rocky Hill, Connecticut) that builds a cloud-native Claims Management System (CMS) with an AI assistant called Clive. Think of it as a modern CMS that also has an AI copilot built in. Clive is a multi-agent system -- six specialized AI agents that each handle a different part of the claims process. [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md, Part 1]

### Company Profile

| Attribute | Detail |
|-----------|--------|
| **Founded** | 2017, Israel |
| **HQ** | Rocky Hill, Connecticut |
| **Total Funding** | ~$20M (Series A) |
| **Revenue (2024)** | $10.1M (up from $3.6M -- ~180% YoY growth) |
| **Team Size** | 53 people |
| **Key Investors** | Aquiline Capital Partners, 83North, F2 Venture Capital, Pipeline Capital Partners, Google Cloud |
| **Geographic Split** | ~70% US, ~30% Europe/UK/Australia |
| **Technology** | Google Gemini LLM, Vertex AI, LangChain, LangSmith |
| **Known Customers** | Starr Insurance (Jan 2026), Qover, INSHUR, Xceedance, INIC, L+M Development Partners |
| **Partnerships** | Sutherland (claims modernization), Liberate (voice AI for FNOL), Vitesse (payments) |

[SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md, Part 1]

### What Clive's Agents Do

Clive deploys six specialized AI agents:

1. **Communication Agent** -- Drafts emails and correspondence
2. **Investigation Agent** -- Guides investigation steps using pre-defined playbooks
3. **Evaluation Agent** -- Coverage matching and liability assessment using LLM policy reading
4. **Compliance Agent** -- Regulatory checks
5. **Knowledge Agent** -- Searches claim history and policy database
6. **Management Agent** -- Workflow orchestration across agents

[SOURCE: mysa_product_strategy.md, Part 4a; Five_Sigma_vs_Shift_Technology_Deep_Research.md]

### How They Sell

Five Sigma sells their platform as a full CMS replacement OR as Clive (AI layer) on top of existing CMS via REST APIs. The Starr Insurance partnership (January 2026) is their largest named win. They position as "the full claims management platform with AI built in." [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md]

### Pricing Model

Not publicly disclosed. Based on their known customer base (mid-market carriers, MGAs, TPAs) and $10.1M revenue across a small customer set, estimated contract values are in the $200K-$1M+ ACV range for full CMS + AI deployment. Per-claim pricing also offered for Clive-only overlay. [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md; CLAUDE ANALYSIS]

### Is Clive Actually Autonomous?

**Verdict: Clive is a copilot with limited autonomous capabilities for simple claims.** [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md]

Evidence:
- "For situations that require judgment, exceptions, or when faced with complex issues, Clive consults its colleagues -- human adjusters and claim managers"
- "His automation depends on the insurer's permissions and SOP"
- The only concrete STP data is for pet insurance (90% reduction in handling time) -- a trivially simple line of business
- Five Sigma's own CEO acknowledges: "You can't just throw ChatGPT at a 10-year-old bodily injury claim"

For simple, low-value, single-peril claims (pet insurance, basic property below threshold), Clive can operate end-to-end. For anything involving complexity, judgment, bodily injury, or high value, it is firmly a copilot. [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md]

### Five Sigma's Confirmed Gaps (Mysa's Advantages)

| Gap | Detail | Mysa's Advantage |
|-----|--------|-----------------|
| **No EU convention systems** | Cannot match EAS data against IRSA/CARD/CIDE/IDS. No evidence whatsoever in any materials. | Mysa builds this as core wedge product |
| **Generic playbooks** | Pre-defined investigation templates, not carrier-specific SOPs | Mysa encodes carrier SOPs into tailored workflows |
| **LLM coverage matching is fragile** | Uses LLM to read policies -- breaks on complex exclusions, nested clauses | Mysa supplements LLM with structured rules + SOP compliance |
| **No property-specific features** | No Xactimate integration, no scope-of-loss, no contractor coordination | Mysa will integrate with Xactimate (US expansion) |
| **No causation analysis** | Cannot determine "sudden vs gradual" for property | Mysa builds this for property thesis |
| **Limited EU presence** | 30% of business, US-first mindset | Mysa is EU-first |
| **No P&L-aware reserve setting** | Basic reserve suggestions only | Mysa frames reserves as P&L impact -- CFO-level selling point |
| **No decision ground truth capture** | Doesn't systematically capture WHY adjusters decide | Mysa's core moat is decision reasoning data |

[SOURCE: mysa_product_strategy.md, Part 4a; Five_Sigma_vs_Shift_Technology_Deep_Research.md]

### Why Five Sigma Matters

Five Sigma is growing fast ($3.6M to $10.1M revenue = 180% YoY) and has proven that the AI-on-any-CMS approach works. They landed Starr Insurance, a meaningful mid-market carrier. Their Gemini-based multi-agent system validates the same architectural approach Mysa would use. [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md]

**The risk:** If Five Sigma decides to build convention system support and carrier-specific SOP encoding, they have the revenue, the team, and the customer base to do it. Their 30% EU presence means they are already talking to European carriers. Speed matters -- Mysa needs to establish the convention system wedge and SOP lock-in before Five Sigma expands there.

**The honest assessment:** Five Sigma is "everywhere and nowhere at the same time." They are the most direct competitor, but their breadth (all lines, all geographies, CMS + AI) creates a surface area problem. Mysa's bet is that depth in the decision layer -- convention systems, SOP encoding, decision ground truth -- beats breadth. This is a defensible bet, but it is a bet.

---

## 5.4 Verisk / XactAI -- The Existential Long-Term Risk

> "How can we integrate with them? I want this integrated with them."
> -- Tiago Brigido, Co-founder (about Xactimate) [TRANSCRIPT: Feb 7, 2026]

### What Verisk Actually Is

Verisk is a $35B+ market cap public company (NYSE: VRSK) that owns Xactimate, the estimation tool used for 75-80% of all US property claims. Every adjuster, TPA, carrier, and independent adjuster in US property uses Xactimate or integrates with it. Verisk also owns XactAnalysis (workflow), XactContents (contents valuation), and has integrated Hover (3D property measurement from smartphone photos). [SOURCE: mysa_product_strategy.md, Part 4b; home_property_competitive_deep_dive.md, Section 3]

### What XactAI Actually Does (Launched September 2025)

XactAI was launched in September 2025 as AI tools bundled FREE with Xactimate Pro subscriptions. This is important -- bundled free means instant distribution to every Xactimate user. [SOURCE: mysa_product_strategy.md, Part 4b; home_property_competitive_deep_dive.md, Section 19]

**What XactAI does today:**
- Photo labeling -- AI tags and categorizes damage photos
- Transcription summaries -- converts voice notes to structured text
- Admin efficiency features -- faster data entry, less manual work

**What XactAI does NOT do today:**
- No coverage analysis
- No reserve recommendation
- No investigation scoping
- No decision support of any kind
- No convention system support
- No SOP-driven workflows

> "Verisk/XactAI is in every property adjuster's hands but only does photo labels and transcription summaries -- features, not decisions. Bundled free with Xactimate Pro."
> [SOURCE: home_property_competitive_deep_dive.md, Section 19]

### Why Mysa Has Time (For Now)

| Factor | Assessment |
|--------|-----------|
| **Strategic DNA** | Verisk is an estimation + data analytics company, NOT a decision support company |
| **Buyer mismatch** | XactAI buyer = CTO/IT (platform). Decision engine buyer = VP Claims. Different budgets, different champions. |
| **Current XactAI scope** | Admin automation (faster data entry), not expert judgment |
| **Domain expertise gap** | Building real decision AI requires insurance adjusting expertise they don't have internally |
| **Timeline** | 2-3 years before meaningful decision support -- Mysa needs to establish by then |
| **EU presence** | Minimal. Verisk is overwhelmingly US-focused for property. |

[SOURCE: mysa_product_strategy.md, Part 4b]

### Why This Risk Is Existential

If Verisk decides to build coverage analysis on top of their estimation data, they have:

- **Every property claim estimate ever written** -- decades of data
- **Regional pricing databases** -- the authoritative source
- **75-80% US market share** -- every carrier already pays them
- **Free distribution** -- bundle with Xactimate like they did with XactAI
- **Hover partnership** -- 3D property measurement integrated
- **4.5B+ data points** across the ecosystem

> "Verisk has the data (every Xactimate estimate ever written) and the distribution (75-80% market share). If they decide to build a real decision engine inside Xactimate -- not just photo labels, but actual coverage analysis and triage -- they could own this overnight."
> [SOURCE: home_property_competitive_deep_dive.md, Section 19]

### Mysa's Defensive Strategy

1. **EU-first buys time.** Verisk has minimal EU presence. By the time Verisk might build decision AI (if they do), Mysa needs the decision ground truth data moat established in EU markets. [SOURCE: mysa_product_strategy.md, Part 4b]

2. **Integrate, don't compete.** The co-founder's instinct to integrate with Xactimate is correct. In the US, Mysa wants to be the decision layer that feeds INTO Xactimate, not competes with it. Verisk's Xactimate ecosystem is open -- APIs, third-party integrations, partner program. [SOURCE: home_property_competitive_deep_dive.md, Section 15; mysa_product_strategy.md, Part 4b]

3. **Build what Verisk cannot easily build.** Convention system expertise, carrier-specific SOP encoding, and decision ground truth data are domain-knowledge-intensive products that Verisk's engineering team (estimation-focused) cannot replicate quickly. [SOURCE: CLAUDE ANALYSIS]

**The honest question:** Can Mysa move fast enough that Verisk doesn't build this themselves? Crawford's Turvi/CoverAI is the early warning signal -- if Verisk starts licensing decision tools standalone, the gap is closing. [SOURCE: home_property_competitive_deep_dive.md, Section 19]

---

## 5.5 Shift Technology -- The EU Danger

### What Shift Technology Actually Is

Shift Technology is a Paris-founded company that started as a fraud detection platform in 2014 and has spent 10+ years building ML models that identify suspicious insurance claims. In September 2025, they launched "Shift Claims" -- an expansion from fraud detection into full claims automation using agentic AI. This is their pivot from "fraud company" to "claims company." [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md, Part 2]

### Company Profile

| Attribute | Detail |
|-----------|--------|
| **Founded** | 2014, Paris, France |
| **Total Funding** | $320M across 6 rounds |
| **Valuation** | $1B+ (unicorn since May 2021) |
| **Customers** | ~100+ insurers across 25+ countries |
| **Claims Analyzed** | Nearly 2 billion (cumulative) |
| **Technology** | Azure OpenAI Service (GPT series), Azure AI Vision, proprietary ML models |
| **Key Investors** | Accel, Bessemer, General Catalyst, Advent International, Guidewire (strategic) |
| **Notable Customers** | AXA (Switzerland, France via Direct Assurance), Generali France, Mitsui Sumitomo, Assurant, Shelter Insurance |
| **Key Partnership** | Guidewire (Strategic Partner since Nov 2024), Duck Creek |

[SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md, Part 2]

### Shift's Product Portfolio

| Product | Maturity | What It Does |
|---------|----------|-------------|
| **Shift Claims Fraud Detection** | Very mature (10+ years) | AI-native fraud scoring against hundreds of scenarios. Network fraud detection. Insurance Data Network (IDN) for cross-carrier data sharing. |
| **Shift Claims** (Sept 2025) | Very new (<6 months) | Agentic AI for full claims workflow. STP agent for eligible claims. Handler assistance for complex claims. |
| **Shift Subrogation** | Mature (standalone product) | AI-based recovery opportunity identification. 90%+ liability accuracy. |

[SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md, Part 2]

### The "60% Automation Rate" -- What It Actually Means

AXA Switzerland reported a 60% automation rate with Shift Claims. This headline is impressive but requires scrutiny:

- **60% of TASKS automated, not 60% of DECISIONS.** There is a crucial difference. Automating document classification and data entry counts as "task automation" alongside actual claims decisions. [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md, Part 2; mysa_product_strategy.md, Part 4c]
- **Single customer, single market.** The 60% figure comes from one customer (AXA Switzerland) in one market. [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md]
- **Vendor-reported, not independently audited.** [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md]
- **No breakdown by line of business.** Motor property likely much higher than bodily injury. [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md]
- **The 99% accuracy claim** is for "claims assessment" (classification/scoring), not for claims decisions or settlement accuracy. [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md]

### The Key Distinction: Workflow vs. Judgment

> "Shift automates the workflow. Mysa automates the judgment. These are different layers. Shift makes the process flow faster. Mysa makes the decisions better."
> [SOURCE: mysa_product_strategy.md, Part 4c -- CLAUDE ANALYSIS]

Shift starts downstream of coverage decisions. Their fraud product scores claims for suspicious patterns. Their claims product routes claims, automates tasks, and assists handlers. But they do not make the triage decision itself -- they automate what happens AFTER triage. [SOURCE: home_property_competitive_deep_dive.md, Section 19]

### Shift Technology's Confirmed Gaps

| Gap | Detail |
|-----|--------|
| **Starts downstream** | Automates workflow AROUND decisions, not the decisions themselves |
| **Fraud-first architecture** | AI optimized for pattern matching, not judgment reasoning |
| **No convention matching** | Doesn't process EAS data into convention system fault determination (IRSA, CARD, CIDE, IDS). Not explicitly documented anywhere despite EU HQ. |
| **No SOP-driven workflows** | Limited workflow customization |
| **Claims product maturity** | Shift Claims launched September 2025. Less than 6 months of production history. Fraud product has 10+ years. The maturity gap is enormous. |
| **Fraud false positive rate** | ~31% of alerts are not accepted for investigation (69% acceptance rate). For SIU teams processing hundreds of alerts, this is significant. |

[SOURCE: mysa_product_strategy.md, Part 4c; Five_Sigma_vs_Shift_Technology_Deep_Research.md]

### Why Shift Is the EU Danger

Shift is the most dangerous EU competitor for three reasons:

1. **Capital.** $320M in funding vs. Mysa's pre-seed. They can build anything they decide to build.
2. **EU relationships.** Paris HQ, AXA, Generali France, 25+ countries. They are already inside the carriers Mysa wants to sell to.
3. **Guidewire partnership.** Strategic partner since November 2024. Guidewire is a major CMS in the EU mid-market. This gives Shift preferred distribution.

**The bet:** Shift is focused on downstream workflow automation, not upstream data quality and convention matching. The EAS-to-STP pipeline is a document AI problem, not a workflow automation problem, and Shift is unlikely to prioritize it. But if they do -- with $320M and AXA as a customer -- they could close this gap. [SOURCE: home_property_competitive_deep_dive.md, Section 20]

---

## 5.6 Wamy -- The New Entrant

### What We Know

Wamy is a new claims AI company that launched from stealth in December 2025. Information is limited across all source documents. [SOURCE: mysa_product_strategy.md, Part 3c; market_landscape_overview.md]

| Attribute | Detail |
|-----------|--------|
| **Launched** | December 2025 (from stealth) |
| **Focus** | P&C claims automation, "AI workforce" approach |
| **Market** | US-only (as far as can be determined) |
| **Funding** | Undisclosed |
| **Traction** | Pre-traction (brand new) |
| **Coverage claim** | Claims to validate coverage |

[SOURCE: mysa_product_strategy.md, Part 3c; market_landscape_overview.md]

### What Wamy Claims to Do

Wamy positions as an "AI workforce" for claims -- similar to the FurtherAI framing but with more emphasis on coverage validation. They claim to validate coverage as part of their automation. [SOURCE: mysa_product_strategy.md, Part 3c]

### Assessment

**What we can say with confidence:**
- Wamy is brand new and pre-traction. Being in market for less than 3 months means negligible customer base, unproven technology, and unknown staying power.
- US-only positioning means no EU presence, no convention system capability, no EU regulatory compliance.
- No evidence of SOP-driven workflows or decision ground truth capture.
- "Claims AI workforce" is a broad positioning that doesn't indicate depth in any specific area.
- Their coverage validation claim is worth monitoring but unproven.

**What we cannot assess:** Technology quality, team strength, specific architecture, pricing, customer pipeline, actual product capabilities. The lack of public information makes Wamy impossible to evaluate rigorously.

**Risk level to Mysa:** Low in the near term. Wamy is US-only with no EU presence, no convention systems, and no proven technology. However, any company claiming coverage validation should be monitored. If they achieve traction in the US market before Mysa expands there, they could become a competitor for the US property decision layer. [SOURCE: market_landscape_overview.md; mysa_product_strategy.md, Part 3c]

---

## 5.7 Secondary Competitors

These companies are not direct threats to Mysa's primary positioning but represent adjacent players that investors will ask about.

### Assured (~$1B Valuation)

**What they do:** Assured is the most-deployed agentic AI in P&C claims. Their platform includes digital FNOL with dynamic question flows, "Emma" (an AI agent that handles 70% of interactions autonomously -- collecting documents, photos, sending reminders, answering questions), omnichannel messaging, fraud detection, and catastrophe tools. They explicitly "augment your core system, not replace it" -- layering on top of Guidewire, Duck Creek, etc. [SOURCE: home_property_competitive_deep_dive.md, Section 4]

| Attribute | Detail |
|-----------|--------|
| **Founded** | 2019, Palo Alto |
| **Valuation** | $1B (March 2025, Series A from ICONIQ Capital + Kleiner Perkins) |
| **Team** | ~65 employees |
| **Traction** | 50M+ customer interactions for the largest US insurers |
| **Product examples** | Heavily auto-focused: 3D vehicle damage painting, collision dynamics |

**Gaps:** US-only. Product examples are heavily auto-focused -- no evidence of property-specific features, Xactimate integration, field inspection workflows, or contractor coordination. No EU convention systems (IRSA, CARD, IDS, CIDE). No EU operations or GDPR/AI Act compliance positioning. [SOURCE: home_property_competitive_deep_dive.md, Section 4]

**Threat to Mysa:** Low for EU motor. Moderate for US property if they decide to go deep on property. High if they enter EU with their capital base. The $1B valuation and institutional backing mean Assured can pivot into adjacent areas rapidly.

### Avallon ($4.6M Seed, YC S25)

**What they do:** AI agents for calls, emails, document triage, and data entry in insurance claims. Workers' comp and auto focused. 10x revenue growth during YC batch. [SOURCE: competitive_landscape_reality_check.md; home_property_competitive_deep_dive.md, Section 5]

> "They are just calling the repair guy."
> -- Co-founder [TRANSCRIPT: Feb 7, 2026]

**Threat to Mysa:** Low. Intake automation only. No decision support. No EU. No convention systems.

### ClaimSorted (~$13.3M Raised)

**What they do:** AI-first TPA. Positions as a technology-enabled claims processor, not a software product. 3-10x faster processing. UK + EU + US expansion. [SOURCE: competitive_landscape_reality_check.md; mysa_product_strategy.md, Part 4d]

> "Their positioning is the worst."
> -- Co-founder [TRANSCRIPT: Feb 7, 2026]

**Threat to Mysa:** Low. TPA model (services + tech) is fundamentally different from Mysa's software model. They compete with Sedgwick and Crawford, not with Mysa.

### FurtherAI ($30M, a16z)

**What they do:** "AI workforce for insurance." Broad horizontal tool across all insurance lines. Claims 30x faster intake and 95% accuracy. [SOURCE: mysa_product_strategy.md, Part 4d; home_property_competitive_deep_dive.md, Section 5]

> "They are trying to do everything."
> -- Co-founder [TRANSCRIPT: Feb 7, 2026]

**Threat to Mysa:** Low-to-moderate. Well-funded (a16z) but horizontally positioned. "Trying to do everything" means they are unlikely to build deep convention system or SOP workflow capability.

### omni:us (~EUR 45M Raised)

**What they do:** Berlin-based. End-to-end P&C claims automation. 70% auto-settlement rate claimed. Pre-built for 7 P&C lines. Allianz Austria customer (processed 2024 storms with zero backlog). UNIQA case study: 60% STP + 25% semi-automated = 85% with AI involvement. Strong subrogation detection (EUR 1B cumulative identified). [SOURCE: Sprout_ai_vs_Omnius_Deep_Research.md]

| Attribute | Detail |
|-----------|--------|
| **HQ** | Berlin, Germany |
| **Funding** | ~EUR 45M (Series A across three tranches) |
| **Team** | ~65 employees, 19 nationalities |
| **Customers** | ~30 pilot/active across 6 EU countries + USA |
| **Tech** | NLP, Computer Vision, OCR, Google Cloud |

**Gaps:** No confirmed EU convention system support. Handwritten OCR is mediocre (7.25% character error rate per Google Cloud case study). EUR 5,000 cap on automated cost assessment. Conflicting automation claims (50% vs 70%) across materials. [SOURCE: Sprout_ai_vs_Omnius_Deep_Research.md]

**Threat to Mysa:** Moderate. EU-native with real traction (Allianz, UNIQA). But focused on document processing and automation, not decision support or convention matching. If they build convention capability, they become a serious EU competitor.

### MarvelX (EUR 5.4M, Founded 2025)

**What they do:** Amsterdam-based. Building "ClaimOS MaX" -- EU-first agentic AI for claims processing, fraud detection, and customer communications. Founded in 2025. [SOURCE: home_property_competitive_deep_dive.md, Section 5]

**Threat to Mysa:** Low for now (pre-traction, seed-stage). Worth monitoring as the closest "EU-first Assured." If they gain traction with EU carriers before Mysa does, they could compete for the same buyer relationships.

### Crawford / Turvi CoverAI

**What they do:** Crawford ($1.29B revenue, public NYSE: CRD) spun out Turvi in 2025 as a standalone insurtech subsidiary. Three products: CoverAI (AI-driven policy coverage review), Asservio (digital estimate review), and Digital Desk (claims triage). Crawford also operates the largest independent contractor network (6,000+ vetted contractors, $2.5B in project costs). [SOURCE: home_property_competitive_deep_dive.md, Section 1]

**Threat to Mysa:** CoverAI is the closest to building the coverage decision layer -- but it was reabsorbed into Crawford's TPA stack. No standalone availability. No causation analysis. If Crawford starts licensing Turvi/CoverAI standalone, the gap is closing and this becomes an important signal. [SOURCE: home_property_competitive_deep_dive.md, Section 19; mysa_product_strategy.md, Part 3c]

### Tractable

**What they do:** London-based. Computer vision for motor damage assessment. AI-generated repair estimates and triage. Works with Aviva (UK), Admiral Seguros (Portugal/Spain). 70-75% of customers complete claims digitally. [SOURCE: home_property_competitive_deep_dive.md, Section 20]

**Threat to Mysa:** Low. Photo-based damage assessment is a different layer (physical estimation) not decision support. Does not touch coverage determination, convention systems, or SOP workflows.

### Bdeo

**What they do:** Spanish startup. Visual intelligence for motor AND property insurance. Works with 7 of 10 top Spanish auto insurers (Zurich, Mutua Madrilena, Mapfre). Present in 20 countries. Can identify cause of damage, assess severity, and recommend repair professionals. [SOURCE: home_property_competitive_deep_dive.md, Sections 20, 21]

**Threat to Mysa:** Low-to-moderate. Bdeo is the most relevant EU property competitor for visual damage assessment. But their focus is visual intelligence (damage photos), not coverage determination or decision support.

### Hi Marley

**What they do:** Omnichannel communication platform for insurance. SMS-based communication between adjusters, policyholders, and service providers.

**Threat to Mysa:** Low. Communication layer, not decision layer. Does not compete with Mysa's core positioning.

### CCC / EvolutionIQ ($730M Acquisition)

**What they do:** CCC ($13B+ market cap) acquired EvolutionIQ for $730M (closed Q1 2025). EvolutionIQ tells adjusters what to do next on injury claims -- triage + investigation guidance. CCC launched "Medhub for Casualty" in Q3 2025 for medical record synthesis. IX Cloud Platform connects 35,000+ businesses. [SOURCE: competitive_landscape_reality_check.md]

**Gaps:** US-only. Auto casualty and workers' comp only. No property footprint. No EU presence. Their 35,000-business auto network does not transfer to property. [SOURCE: home_property_competitive_deep_dive.md, Section 19]

**Threat to Mysa:** Low for EU motor. Low for property. CCC owns auto casualty guidance but has zero footprint in the areas Mysa targets. However, the $730M acquisition validates the market -- CCC paid $730M specifically because the decision guidance layer is where value is. [SOURCE: competitive_landscape_reality_check.md]

---

## 5.8 The Property Claims AI Gap

This section documents one of the most striking findings across all competitive research: the disparity between investment in physical property data versus investment in property claims decision support.

### $3B+ Invested in Physical Tools, ~$0 in Decision Tools

| Company | What They Do | Funding | Decisions? |
|---------|-------------|---------|-----------|
| **Hover** | 3D property models from smartphone photos | $142M (investors include Travelers, State Farm, Nationwide) | NO -- measurement only |
| **EagleView** | Aerial imagery, roof models, 3B+ photos, 94% US coverage | ~$2.8B (PE-backed) | NO -- visual data only |
| **Nearmap (+ itel)** | Aerial imagery + material pricing | $730M (Thoma Bravo) | NO -- estimation data |
| **CAPE Analytics** | Geospatial AI property risk, hail damage rating 96%+ accuracy | $75M (acquired by Moody's) | NO -- underwriting only |
| **ZestyAI** | Property risk intelligence | $50M | NO -- underwriting only |
| **Encircle** | Field documentation: photos, videos, floor plans, moisture readings | ~$3.6M | NO -- field docs only |
| **Xactimate/XactAI** | Estimation + admin AI (75-80% market share) | Public (Verisk $40B+) | NO -- estimation efficiency |
| **Crawford CoverAI** | Policy interpretation for coverage decisions | Corporate | Closest -- but reabsorbed into TPA stack |
| **Wamy** | Claims AI workforce, coverage validation claim | Undisclosed | Brand new (Dec 2025), pre-traction |

[SOURCE: market_landscape_overview.md; mysa_product_strategy.md, Part 3c]

### The Gap Stated Precisely

> "$3B+ invested in the physical side of property claims. Almost zero in decisions."
> [SOURCE: market_landscape_overview.md]

- Hover digitizes the BUILDING (3D models, measurements). It doesn't decide if the damage is COVERED.
- EagleView photographs the ROOF. It doesn't determine if the storm damage was from THIS storm or pre-existing.
- Xactimate calculates the COST. It doesn't determine if the policy PAYS for it.
- CAPE Analytics predicts the RISK. It doesn't handle the CLAIM.

The coverage question ("is this covered?"), the causation question ("what caused this?"), the triage question ("desk review, virtual inspection, or boots on the ground?"), and the reserve question ("what's the realistic exposure?") -- these are the highest-value, most time-consuming parts of property adjusting, and no standalone product addresses them. [SOURCE: home_property_competitive_deep_dive.md, Sections 16, 21]

### The Honest Competitive Map for Property

| Layer | US | EU | Gap? |
|-------|-----|-----|------|
| Damage estimation | Xactimate (monopoly) | Fragmented (no monopoly) | No |
| Photo damage assessment | Hover, CAPE, EagleView | Bdeo | Getting competitive |
| Claims intake/FNOL | Assured, Sprout.ai, Shift | Sprout.ai, Shift | Crowded |
| Fraud detection | Shift, carriers in-house | Shift | Shift dominates |
| Field documentation | Encircle, BuildArray | Limited | Some tools exist |
| **Coverage determination** | **Crawford/Turvi CoverAI (proprietary)** | **NOBODY** | **Open** |
| **Causation analysis** | **NOBODY** | **NOBODY** | **Wide open** |
| **Triage decision (desk/virtual/field)** | **NOBODY (standalone)** | **NOBODY** | **Open** |
| **Reserve recommendation** | **Gradient AI (underwriting-focused)** | **NOBODY** | **Mostly open** |
| **Adjuster copilot** | Five Sigma/Clive | Five Sigma/Clive (30% EU) | Early |

[SOURCE: home_property_competitive_deep_dive.md, Section 21]

### Why This Gap Exists

Five structural reasons explain why the decision layer remains unbuilt. Understanding them is important because the same barriers that have kept competitors out will challenge Mysa:

1. **Liability fear.** A wrong coverage determination could trigger bad-faith lawsuits. Companies build around the decision rather than supporting it. The counter: human-in-the-loop design (AI recommends, adjuster decides) manages this liability -- CCC, Five Sigma, and Crawford all prove this model works in production. [SOURCE: home_property_competitive_deep_dive.md, Section 16]

2. **Domain expertise gap.** Building triage/decision/investigation tools requires deep insurance knowledge -- policy language interpretation, state-by-state regulation, coverage nuances, claims investigation methodology, fraud indicators. "Tech founders don't have this knowledge. And insurance people who do have it usually don't start tech companies." The talent intersection of "deep claims expertise" + "can build software" is incredibly thin. [SOURCE: home_property_competitive_deep_dive.md, Section 16]

3. **The easy stuff gets funded first.** VCs want fast traction. The fastest path is intake automation -- 30x faster FNOL, 98% accuracy on documents. These are real, measurable, fast to build, and easy to sell. "Telling a VP Claims 'we'll help your adjusters make better coverage decisions' is harder to quantify, longer to prove, and scarier to buy." [SOURCE: home_property_competitive_deep_dive.md, Section 16]

4. **Verisk/Xactimate could do it.** The estimation monopoly has the data, distribution, and carrier relationships to build decision tools. The constant shadow of "Verisk could build this" discourages startup investment in the space. [SOURCE: home_property_competitive_deep_dive.md, Sections 8, 19]

5. **Regulatory complexity.** 50 US states with different settlement rules. EU has country-by-country conventions plus GDPR. The EU AI Act classifies claims AI as high-risk. Nobody wants to build the "universal" decision layer because the rules differ everywhere. [SOURCE: competitive_landscape_reality_check.md]

---

## 5.9 The Moat -- Mysa's Competitive Defenses

Mysa's competitive strategy does not rely on being first to market (others are already here) or having more capital (others have 10-100x more). It relies on building assets that compound over time and are structurally difficult to replicate.

### Layer 1: Decision Ground Truth Data

**What it is:** Every time an adjuster uses Mysa to process a claim, the system captures the AI's recommendation AND the adjuster's actual decision -- including any modifications and the reasoning behind them. This creates a dataset that links claim inputs, AI suggestions, human decisions, and outcomes. [SOURCE: MODULE_01_POSITIONING.md, Section 1.1]

**Why it's a moat:**
- No competitor captures this data. CCC and Verisk have claim OUTCOMES (what was paid). Nobody has decision REASONING (why it was paid). [SOURCE: mysa_product_strategy.md, Part 4a]
- The data compounds: every claim processed makes the next recommendation more accurate
- The data is carrier-specific: each carrier's decision patterns create a proprietary model that improves over time
- It cannot be acquired -- you have to process millions of claims to build it

**Honest assessment:** This moat only works once Mysa has meaningful claim volume. Until then, it is a theoretical advantage. The chicken-and-egg problem is real: the data moat builds with customers, but you need customers first. [SOURCE: home_property_competitive_deep_dive.md, Section 8]

### Layer 2: SOP-Encoded Workflows (Carrier Lock-In)

**What it is:** Mysa encodes each carrier's Standard Operating Procedures into AI-guided decision workflows. Different carriers have different authority levels, investigation triggers, reserve thresholds, and documentation requirements. Once encoded, the carrier's institutional knowledge lives in Mysa. [SOURCE: MODULE_01_POSITIONING.md, Section 1.1]

**Why it's a moat:**
- Switching costs are prohibitive. Migrating encoded SOPs to a competitor requires re-encoding months of work.
- SOPs are the carrier's own knowledge -- they are unique to each carrier
- Once adjusters are trained on Mysa's SOP workflows, behavioral lock-in reinforces contractual lock-in
- No competitor offers carrier-specific SOP encoding (Five Sigma uses generic playbooks) [SOURCE: mysa_product_strategy.md, Part 4a]

**Honest assessment:** The lock-in only works if Mysa delivers enough value that carriers accept the switching cost trade-off. A product that locks in a customer but doesn't deliver results loses the customer anyway. The SOP encoding also requires significant upfront effort per carrier -- this is a sales cycle burden.

### Layer 3: Convention System Expertise

**What it is:** Country-by-country knowledge of EU inter-insurer convention systems -- IDS (Portugal), IRSA (France), CARD (Italy), CIDE/ASCIDE/CICOS (Spain) -- encoded into software. Each country has different rules, different lookup tables, different data requirements, different exception handling. [SOURCE: MODULE_01_POSITIONING.md, Section 1.2]

**Why it's a moat:**
- Takes years to replicate. Each country requires deep regulatory and industry knowledge.
- Confirmed across all competitors: nobody else is building this [SOURCE: Five_Sigma_vs_Shift_Technology_Deep_Research.md; Sprout_ai_vs_Omnius_Deep_Research.md]
- Network effects within each country -- as more carriers in a market use Mysa, the convention matching data improves
- EU AI Act creates a regulatory moat for compliance-first products [SOURCE: home_property_competitive_deep_dive.md, Section 20]

**Honest assessment:** This moat is EU-specific and motor-specific. It does not apply to property claims (no convention systems exist for property) or to the US market. It is the strongest moat for the initial wedge but must be supplemented by Layers 1 and 2 for long-term multi-market defense.

### Layer 4: Annotation Tools as Competitive Weapon

**What it is:** Caravela's OCR engine and its associated annotation/validation tools create a continuous improvement loop. Every human correction of an OCR extraction improves the model. The annotation interface and training pipeline are assets that competitors would need to build from scratch. [SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md]

**Current position:**
- 81.5% normalized accuracy on Portuguese EAS forms (44 claims with ground truth) [SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md]
- Competitive with Google Document AI (82%) and above Amazon Textract (78%) [SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md]
- Below Azure Document Intelligence (93%) and template-based solutions (99%) -- gap explained by handwriting, Portuguese diacritics, and no template/zone-based extraction yet [SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md]
- Roadmap to 85-88% via prompt engineering and preprocessing; 90%+ requires fine-tuning with 200+ training examples [SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md]

**Why it's a moat:**
- Every EAS form processed and corrected improves the model
- The annotation pipeline (human-in-the-loop for low-confidence fields) creates a data flywheel
- Competitors starting from scratch would need to build the same training pipeline and collect similar training data
- The dataset (ground truth annotations linked to convention outcomes) is uniquely valuable

**Honest assessment:** At 81.5% accuracy with 44 claims, this is an early-stage moat. The OCR competitive landscape includes much larger players (Azure at 93%, Hyperscience claiming 99% with HITL). The moat becomes meaningful only as the dataset scales past hundreds of validated claims. The annotation tools are a defensible asset, but OCR accuracy alone is not a sufficient moat -- it must be combined with the convention matching and decision workflow layers. [SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md]

---

## 5.10 Master Comparison Matrix

### Multi-Dimensional Competitive Assessment

| Dimension | **Mysa** | **Five Sigma / Clive** | **Verisk / XactAI** | **Shift Technology** | **Wamy** | **Assured** |
|-----------|----------|----------------------|--------------------|--------------------|----------|------------|
| **Category** | Claims decision engine | CMS + AI copilot | Estimation + admin AI | Fraud detection + claims workflow | Claims AI workforce | FNOL + messaging AI |
| **Founded** | 2024 (pivot to claims) | 2017 | Public company (decades) | 2014 | Dec 2025 (stealth exit) | 2019 |
| **Funding** | Pre-seed | ~$20M (Series A) | Public ($35B+ market cap) | $320M (6 rounds, $1B+ valuation) | Undisclosed | ~$1B valuation (Series A) |
| **Revenue** | Pre-revenue | $10.1M (2024, 180% YoY) | Multi-billion (Verisk total) | Not disclosed | Pre-revenue | Not disclosed |
| **Team** | 2 co-founders | 53 people | Thousands (Verisk total) | 200+ estimated | Unknown | ~65 people |
| **Customers** | 1 design partner (Caravela) | Starr, Qover, INSHUR, Xceedance, others | Every US property adjuster (Xactimate) | ~100+ insurers (AXA, Generali, Mitsui) | Pre-traction | 50M+ interactions, "largest US insurers" |
| **Geography** | EU-first (Portugal, expanding Southern EU) | 70% US, 30% EU | US-dominant (minimal EU) | 25+ countries (Paris HQ) | US-only | US-only |
| **SOP-driven workflows** | **YES -- core feature, per carrier** | NO -- generic pre-defined playbooks | NO | Limited customization | Unknown | NO -- Flow Builder for question sequences |
| **Convention systems** | **YES -- built for Portugal (IDS/CIMPAS), expanding** | **NO -- zero evidence** | **NO** | **NO -- not documented despite EU HQ** | **NO** | **NO** |
| **Coverage determination** | **Primary feature -- AI reads policy, matches claim facts** | Basic LLM matching (fragile on complex exclusions) | None (estimation only) | None (workflow automation) | Claims coverage validation (unproven) | None (intake focus) |
| **Decision ground truth** | **Core moat -- captures WHY adjusters decide** | Does not capture reasoning | Claim outcomes only (what was paid) | Fraud patterns only | Unknown | Interaction data only |
| **Reserve recommendation** | **AI + P&L framing (CFO selling point)** | Basic pre-fill | None | None | Unknown | None |
| **Causation analysis** | Planned (property: sudden vs gradual) | None | None | None | Unknown | None |
| **Fraud capability** | Fraud signal agent (one of 6 decision steps) | Basic anomaly detection | None | **Industry-leading** (10+ years, IDN) | Unknown | Built-in (basic) |
| **Data moat** | Decision reasoning (building) | Limited (small customer base) | Massive (every estimate ever written) | 2B claims analyzed, IDN cross-carrier | None yet | 50M+ interactions |
| **Pricing model** | Per-claim SaaS (landing) + platform (expansion) | Platform license + per-claim for Clive overlay | Bundled free with Xactimate | Enterprise license | Unknown | Enterprise license |
| **Integration approach** | Any CMS via API (overlay) | Any CMS via API OR full CMS replacement | Xactimate ecosystem only | Own platform + Guidewire/Duck Creek partnerships | Unknown | Any CMS (overlay) |
| **Target buyer** | VP Claims at mid-market carriers (EUR 100-200M GWP) | Mid-market carriers, MGAs, TPAs | All Xactimate users (CTO/IT buyer) | Large carriers (enterprise sale) | Unknown | Large US carriers |
| **EU AI Act readiness** | Built compliance-first (human-in-the-loop from Day 1) | Not documented | Minimal EU presence | Likely compliant (EU HQ) | N/A (US-only) | N/A (US-only) |

[SOURCE: mysa_product_strategy.md, Part 4e; Five_Sigma_vs_Shift_Technology_Deep_Research.md; home_property_competitive_deep_dive.md; competitive_landscape_reality_check.md; market_landscape_overview.md; MODULE_01_POSITIONING.md]

### Key Risk to Mysa -- Per Competitor

| Competitor | Primary Risk | Probability | Mitigation |
|-----------|-------------|------------|------------|
| **Five Sigma** | Builds convention systems + SOP encoding for EU expansion. They have 30% EU presence and are growing 180% YoY. | Medium (2-3 year timeline) | Move fast on EU wedge. Lock in carrier SOPs before Five Sigma can replicate. Build decision ground truth data moat. |
| **Verisk / XactAI** | Builds coverage analysis on top of estimation data. Free distribution to 75-80% of US property market. | Medium-high (2-3 year timeline) | EU-first strategy avoids Verisk's US stronghold. Integrate with Xactimate rather than compete. Build decision data that Verisk doesn't have. |
| **Shift Technology** | Expands Shift Claims into convention matching and decision support for EU carriers. $320M and AXA give them resources and relationships. | Medium (1-2 year timeline) | Shift is focused on downstream workflow, not upstream data quality. EAS-to-STP is a document AI problem that Shift's workflow approach doesn't solve. Build fast in Southern EU before Shift prioritizes conventions. |
| **Wamy** | Achieves US traction in coverage validation before Mysa enters US. | Low (pre-traction, unknown capability) | Monitor closely. If Wamy proves coverage validation works in US market, accelerate US expansion timeline. |
| **Assured** | Enters EU or goes deep on property with $1B+ in capital. | Low-medium (no EU signal yet) | Different core positioning (intake vs decisions). If Assured enters EU, differentiate on SOP depth and convention expertise. |
| **Allianz-style in-house build** | Large carriers build proprietary decision tools internally, shrinking the addressable market. | Medium (already happening at enterprise tier) | Target mid-market carriers (EUR 100-200M GWP) who cannot build internally. This segment is 90-95% untouched by AI claims tools. |

[SOURCE: mysa_product_strategy.md, Parts 4a-4e; competitive_landscape_reality_check.md; home_property_competitive_deep_dive.md]

---

## The Honest Summary

> "The 'adjuster operating system' is being built -- by multiple players, from multiple angles. CCC is coming from estimating. Five Sigma from CMS. Shift from fraud. Allianz from inside. Avallon and Strada from voice/workflow. Microsoft from the platform layer."
> [SOURCE: competitive_landscape_reality_check.md]

**What is genuinely not being done by anyone -- confirmed across all research:**
1. EU convention systems natively (IRSA, CARD, IDS, CIDE) -- nobody
2. Decision ground truth capture -- everyone automates workflow, nobody captures WHY the adjuster decided
3. Carrier-specific SOP-encoded workflows -- everyone uses generic templates
4. Coverage determination + causation analysis as standalone product -- $3B+ in physical property tools, ~$0 in decision tools

**What is clear-eyed and honest:**
- This is a crowded, competitive space where well-funded players are converging. $730M acquisitions and $320M funding rounds confirm the market is real. [SOURCE: competitive_landscape_reality_check.md]
- The question is not "is the opportunity real?" -- it clearly is. The question is whether Mysa's specific angle (EU conventions + decision ground truth + carrier-specific SOPs) is differentiated enough to win against players with 100x more data and capital. [SOURCE: competitive_landscape_reality_check.md]
- Speed is the most critical variable. Mysa has a 2-3 year window before Verisk, Shift, or Five Sigma potentially closes the gaps. The convention system wedge and SOP lock-in must be established in that window.
- The talent intersection of "deep claims expertise" + "can build software" is thin. That is simultaneously the reason the gap exists and Mysa's primary founder-market fit advantage. [SOURCE: home_property_competitive_deep_dive.md, Section 16]

> "The contrarian bet: everyone else is building the safe, obvious thing (FNOL/intake/docs). The outlier outcome comes from building the hard, scary thing (decisions/investigation/estimation workflow) -- with the right guardrails."
> [SOURCE: home_property_competitive_deep_dive.md, Section 16]

---

## Sources

| Source | Type | Sections Used |
|--------|------|--------------|
| `mysa_product_strategy.md` Part 4 (lines 641-778) | Primary -- competitor deep dives, head-to-head matrix | 5.2-5.5, 5.7, 5.8, 5.10 |
| `competitive_landscape_reality_check.md` | Primary -- market reality check, honest assessment | 5.1, 5.7, Summary |
| `Five_Sigma_vs_Shift_Technology_Deep_Research.md` | Primary -- detailed phase-by-phase analysis of Five Sigma and Shift | 5.2, 5.3, 5.5, 5.10 |
| `Sprout_ai_vs_Omnius_Deep_Research.md` | Primary -- Sprout.ai and omni:us analysis | 5.1, 5.2, 5.7 |
| `home_property_competitive_deep_dive.md` | Primary -- property claims competitive landscape, Assured, TPA analysis, gap analysis | 5.1, 5.2, 5.4, 5.5, 5.7, 5.8, 5.9, Summary |
| `CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md` | Primary -- OCR competitive positioning, accuracy benchmarks | 5.9 |
| `market_landscape_overview.md` | Primary -- Wamy details, funded competitor matrix, property gap | 5.2, 5.6, 5.8 |
| `MODULE_01_POSITIONING.md` | Context -- Mysa's positioning, ICP, value stack | 5.2, 5.9, 5.10 |
| Feb 7, 2026 Granola call -- Co-founder strategy | Transcript | 5.3, 5.4 |
| Feb 7, 2026 Granola call -- Competitive discussion | Transcript | 5.3, 5.7 |

---

# Part 6: Product Specification & Demo

# Module 6: Product Specification & Demo

**Status:** DRAFT v1.0
**Last updated:** February 9, 2026
**Feeds:** Demo build spec, marketing product page, engineering planning, investor walkthrough

---

## 6.1 Product Flow

### The 7-Step Claims Pipeline

Mysa's product follows a claim from arrival to learning loop. Each step has defined system logic, data inputs, and adjuster interaction points. This is the end-to-end architecture — "the demo on paper."

> "So think the product is quite similar to Avalon in the way that it is built. Like, you have the process. You can generate emails. You can parse emails that we are getting. We can draft the email... we parse that. We understand if something is missing. Then you can send automated emails. You can have AI calling."
> [TRANSCRIPT: Feb 7, 2026]

```
CLAIM ARRIVES (email, portal, API, broker submission)
  |
  v
STEP 1: INTAKE PARSING
  | System logic: Parse incoming documents, emails, photos, scanned forms.
  | Identify source type (EAS form, FNOL portal, broker email, API).
  | Extract all machine-readable data; flag handwriting for OCR pipeline.
  | If data is missing, queue auto-outreach (SMS/email to policyholder).
  | "If I'm missing data, I'll go back to the user" [TRANSCRIPT: Feb 7, 2026]
  |
  v
STEP 2: DATA STRUCTURING
  | System logic: Run Caravela OCR engine on all documents.
  | Extract fields into structured claim record (JSON).
  | Validate completeness against carrier-specific field requirements.
  | Cross-reference fields for consistency (e.g., date on EAS vs date on police report).
  | Output: Structured claim object with confidence scores per field.
  | "We need to structure the data" [TRANSCRIPT: Feb 7, 2026]
  |
  v
STEP 3: TRIAGE
  | System logic: Score claim complexity (low/medium/high/critical).
  | Apply SOP-driven routing rules:
  |   - Catastrophe check -> Route to CAT team
  |   - Injury/fatality -> High priority BI specialist
  |   - Cost threshold (70-80% of vehicle ACV) -> Total loss flag, stops STP
  |   - Fraud score above threshold -> SIU investigation
  |   - Coverage ambiguity -> Manual review
  | Assign to appropriate desk: PD desk, BI unit, SIU, total loss, litigation.
  | Set diary dates and investigation plan.
  | "When we onboard, we upload SOPs, translate SOPs into workflows" [TRANSCRIPT: Feb 7, 2026]
  | "Auto triage: I have 20-30%. So you still have value here if you can create more" [TRANSCRIPT: Feb 7, 2026]
  |
  v
STEP 4: INVESTIGATION SUPPORT
  | System logic: Generate investigation checklist from carrier SOP per claim type.
  | Scope required evidence: police report, recorded statements, photos, medical records.
  | Guide adjuster through calls (scripted questions per SOP).
  | Record and transcribe calls.
  | Cross-reference databases (ISO ClaimSearch, NICB, LexisNexis, internal history).
  | Track outstanding items and auto-follow-up on stale requests.
  | "We are recording the calls that you need to make.
  |  We are guiding you through those calls." [TRANSCRIPT: Feb 7, 2026]
  |
  v
STEP 5: DECISION ENGINE -- The 6 Judgment Sub-Steps
  | System logic: For each sub-step, AI generates a recommendation with:
  |   - Confidence score (0-100%)
  |   - Explanation chain (why this recommendation)
  |   - Cited evidence (policy clauses, comparable claims, SOP rules)
  |   - Alternative outcome if evidence changes
  |
  |  +----------------------------------------------------------+
  |  | 1. Coverage verification    <- Policy parsing + SOP       |
  |  | 2. Policy report checking   <- Document completeness      |
  |  | 3. Repair assessment        <- Comparable analysis         |
  |  | 4. Cost analysis            <- Market rates + historicals  |
  |  | 5. Reserve calculation      <- Statistical model + P&L    |
  |  | 6. Fraud detection          <- Pattern matching + signals  |
  |  +----------------------------------------------------------+
  |
  | Human reviews each recommendation: ACCEPT / MODIFY / REJECT.
  | Authority check: if decision exceeds adjuster authority level, escalate to supervisor.
  | "Within decisions, there are six subsections, and for each one of them,
  |  we already help you" [TRANSCRIPT: Feb 7, 2026]
  |
  v
STEP 6: DOCUMENT GENERATION
  | System logic: Generate all required documents per SOP template and decision outputs.
  | Document types: coverage determination letter, reserve memo, denial letter (if applicable),
  | investigation summary, settlement recommendation, convention submission data (EU).
  | Apply carrier branding and template formatting.
  | "We are generating all the documents for you" [TRANSCRIPT: Feb 7, 2026]
  |
  v
STEP 7: FEEDBACK LOOP -- Decision Ground Truth Capture
  | System logic: Compare adjuster's actual decision vs AI recommendation.
  | Record: what was recommended, what was decided, what was changed, why.
  | This data feeds model retraining: accept = positive label, modify = partial label,
  | reject = negative label with correction as ground truth.
  | "We are training our models to eventually start taking these steps" [TRANSCRIPT: Feb 7, 2026]
  | Flywheel: better data -> better recommendations -> more trust -> more data
```

[SOURCE: mysa_product_strategy.md, Part 5a; TRANSCRIPT: Feb 7, 2026]

### System Logic Summary per Step

| Step | AI Role | Adjuster Role | Key Output | Time (Before Mysa) | Time (With Mysa) |
|------|---------|---------------|------------|---------------------|-------------------|
| 1. Intake Parsing | Parse, extract, identify gaps | None (automated) | Structured data + gap alerts | 20-30 min manual entry | 30 sec automated |
| 2. Data Structuring | OCR, validate, cross-reference | Review flagged anomalies (1-2 min) | Clean claim record | 10-15 min | 2 min review |
| 3. Triage | Score complexity, route per SOP | Confirm or override routing | Assigned claim + investigation plan | 5-15 min | 2-3 min review |
| 4. Investigation | Generate checklist, guide calls, transcribe | Conduct calls, review evidence, use judgment | Evidence package | 1-15 hours (varies) | 30-70% reduction |
| 5. Decision Engine | Recommend on 6 sub-steps with reasoning | Accept / modify / reject each | Decision record + audit trail | 65-120 min | 10-15 min review |
| 6. Doc Generation | Auto-generate per SOP templates | Review and sign off | All required documents | 15-30 min | 1-2 min review |
| 7. Feedback Loop | Capture decision vs recommendation | None (passive capture) | Training data | N/A | Continuous |

[SOURCE: mysa_product_strategy.md, Parts 1, 5a; claims_journey_discovery.md, Phases 6-8]

---

## 6.2 The 6 Decision Sub-Steps

### Detailed Breakdown

This is the core product scope -- the 6 expert judgment steps that consume 60-70% of adjuster time. No competitor addresses all six. Each sub-step is a self-contained decision with defined data inputs, system logic, adjuster review, and measurable time saved.

> "The decision is breaking basically breaking down in six different categories. You have coverage. You have checking the policy reports. You need to check the repairs. You need to check how much it costs. You need to check... how much money you are reserving... does it have fraud? There are, like, six steps. That's the judgment."
> -- Tiago Brigido, Co-founder [TRANSCRIPT: Feb 7, 2026]

[SOURCE: mysa_product_strategy.md, Part 1]

---

### Sub-Step 1: Coverage Verification

**What the adjuster does today:** Manually reads the policy document (often 40-80 pages), cross-references claim facts against coverage clauses and exclusions, checks endorsements, verifies policy was active at time of loss, and confirms the insured item matches what is being claimed.

**Data inputs:**
- Policy document (parsed into structured coverage map)
- Claim facts (from intake/structuring)
- Date and time of loss
- Insured item details (VIN for auto, property address for homeowners)
- Named insured vs claimant identity
- Carrier-specific coverage rules from SOP

**System logic:**
1. Parse entire policy document into structured coverage map: covered perils, exclusions, conditions, endorsements, limits, deductibles.
2. Match claim facts against coverage clauses. Highlight applicable coverage in green, applicable exclusions in red, ambiguous areas in yellow.
3. Check policy status: was coverage active at time of loss? Were premiums current? Any lapse?
4. Verify insured item: does the VIN/property address match the policy? Is the driver listed or excluded?
5. Check endorsements that modify base coverage (e.g., added coverage for rental reimbursement, or excluded coverage for business use).
6. Generate coverage determination with confidence score: COVERED / NOT COVERED / REQUIRES INVESTIGATION.
7. For ambiguous cases (e.g., "sudden vs gradual" water damage), generate specific investigation questions needed to resolve ambiguity.
8. Cite specific policy clauses for every determination.

**Adjuster review:** Review coverage determination. Accept if clear. If ambiguous, use investigation questions generated by system to resolve. Override if adjuster disagrees -- system captures override reason.

**Time saved:** 15-30 min (manual) --> 2 min review. The reading and cross-referencing is automated; the adjuster confirms the logic.

**EU-specific:** In convention claims (EU motor), coverage is simpler -- the convention system determines fault allocation between insurers. Coverage verification focuses on policy validity, not peril applicability. Non-convention EU claims (property, liability) follow the same pattern as US.

**US-specific:** State-by-state variation in coverage rules. Comparative vs contributory negligence. Stacking of UM/UIM coverage. HO-3 vs HO-5 policy form differences. System must encode state-specific rules.

[SOURCE: mysa_product_strategy.md, Part 1; claims_journey_discovery.md, Phase 7 -- Coverage analysis activity]

---

### Sub-Step 2: Policy Report Checking

**What the adjuster does today:** Checks if all documentation is complete, facts are consistent across documents, nothing is missing or contradictory. Verifies that the claim narrative matches the physical evidence, that dates align, that party information is consistent.

**Data inputs:**
- All claim documents (EAS, police report, photos, repair estimates, medical records)
- Claim narrative (from FNOL or recorded statement)
- Cross-document field comparison matrix

**System logic:**
1. Validate completeness: check every field required by carrier SOP against what has been received. Generate missing-items list.
2. Cross-reference for consistency: does the date on the EAS match the date on the police report? Does the damage described match the photos? Does the location match telematics data (if available)?
3. Flag contradictions: party A says they were stopped, party B says party A was moving. Photo shows front-end damage, but EAS indicates rear-end collision.
4. Generate gap report: list of missing documents, inconsistent data points, and recommended follow-up actions.
5. Auto-draft follow-up communications (email/SMS) requesting missing items from policyholder, broker, or third party.

**Adjuster review:** Review gap report. Confirm which follow-ups to send. Resolve contradictions through investigation (calls, additional evidence requests).

**Time saved:** 10-20 min (manual) --> 1 min review. System reads all documents simultaneously and cross-references instantly.

[SOURCE: mysa_product_strategy.md, Part 1; claims_journey_discovery.md, Phase 7 -- Documentation activity]

---

### Sub-Step 3: Repair Assessment

**What the adjuster does today:** Reviews the proposed repair scope from a body shop, independent appraiser, or AI estimation tool. Checks if the repair is reasonable -- are line items appropriate for the damage? Are there missing items (hidden damage)? Are there over-scoped items (work not needed)? Compares against comparable claims.

**Data inputs:**
- Repair estimate (from CCC, Mitchell, Audatex, or body shop direct)
- Claim photos (damage photos, scene photos)
- Comparable claims database (similar vehicle, similar damage, similar region)
- Carrier repair guidelines (OEM vs aftermarket parts rules, labor rate schedules, paint time allowances)
- Vehicle specifications (year, make, model, pre-loss condition)

**System logic:**
1. Ingest repair estimate and parse line items: labor operations, parts (OEM/aftermarket/used), paint/materials, sublet operations.
2. Compare each line item against carrier guidelines: is the labor rate within the approved range? Is the parts selection per policy (OEM vs aftermarket)?
3. Compare total estimate against comparable claims: for this vehicle, this damage type, in this region, what is the typical repair cost? Flag outliers (>1 standard deviation from mean).
4. Check for missing items: based on damage type and vehicle, are there operations that should be included but are not (e.g., ADAS recalibration after windshield replacement)?
5. Check for over-scoped items: operations included that do not match the damage pattern (e.g., rear bumper repair on a frontal collision claim).
6. Assess repair vs total loss: compare estimated repair cost to vehicle ACV (Actual Cash Value -- the market value of the vehicle immediately before the loss). If repair exceeds threshold (typically 70-80% of ACV, varies by state/country), flag as potential total loss.
7. Generate assessment summary with anomaly flags and confidence score.

**Adjuster review:** Review flagged anomalies. Negotiate with body shop on disputed line items. Approve or request supplement for hidden damage.

**Time saved:** 15-25 min (manual) --> 3 min review. System handles the line-by-line comparison; adjuster focuses on flagged items only.

**Note:** Mysa does NOT replace estimation tools (Xactimate, CCC, Audatex). It reviews and validates their output against carrier rules and historical data. Integration with estimation tools is required for this sub-step to function.

[SOURCE: mysa_product_strategy.md, Parts 1, 5a; claims_journey_discovery.md, Phase 8 -- Repair estimate review, total loss assessment]

---

### Sub-Step 4: Cost Analysis

**What the adjuster does today:** Compares the repair cost estimate against market rates, historical claims for similar damage, and carrier-specific pricing databases. Validates that the total amount is reasonable before setting reserves or making a settlement offer.

**Data inputs:**
- Validated repair estimate (from Sub-Step 3)
- Market rate databases (regional labor rates, parts pricing)
- Historical claims database (same vehicle type, same damage type, same region)
- Carrier pricing rules (DRP -- Direct Repair Program -- rates, aftermarket parts policy)
- Vendor invoices (towing, rental, storage)

**System logic:**
1. Compare total claim cost against historical distribution for similar claims. Generate percentile ranking ("This claim is at the 73rd percentile for cost among similar claims in this region").
2. Identify cost drivers: which line items are above market rate? Which components drive the total above the median?
3. Calculate total claim cost: repair estimate + rental + towing + storage + any additional coverage components.
4. For BI (bodily injury) claims: analyze medical bills against typical treatment costs for the injury type. Flag outlier charges. Compare to Colossus output where available.
5. Generate cost analysis summary with expected range (e.g., "$7,800-$9,200 based on 847 comparable claims").

**Adjuster review:** Review cost analysis. Accept if within expected range. If outlier, investigate further or negotiate with vendor.

**Time saved:** 10-20 min (manual) --> 2 min review.

[SOURCE: mysa_product_strategy.md, Part 1; claims_journey_discovery.md, Phase 8 -- Cost validation activities]

---

### Sub-Step 5: Reserve Calculation

**What the adjuster does today:** Estimates total expected claim cost for financial reporting purposes. Reserves are recognized immediately on the P&L -- over-reserving ties up capital, under-reserving creates surprise losses. This is a financial decision with direct balance-sheet impact.

> "Do you know this concept? It's not what they are paying that matters. It's how much money they are reserving. Because reserves are already recognized in the P&L right away."
> -- Tiago Brigido, Co-founder [TRANSCRIPT: Feb 7, 2026]

**Data inputs:**
- Cost analysis output (from Sub-Step 4)
- Historical claims outcomes for comparable cases
- Claim trajectory data (how similar claims have developed over time)
- Carrier reserve rules (initial reserve formulas, adjustment triggers, authority levels)
- Reinsurance thresholds (does this claim approach reinsurance treaty triggers?)

**System logic:**
1. Calculate recommended reserve using multiple methods:
   - Formula-based: carrier's own reserve calculation rules (e.g., initial reserve = estimate x 1.2 for PD; initial reserve = medical bills x multiplier for BI).
   - Comparable-based: median outcome of similar claims in carrier's history, weighted by recency and similarity score.
   - Trajectory-based: for open claims, project likely development based on how similar claims evolved over time.
2. Generate confidence interval: "Recommended reserve: EUR 3,100. 90% confidence interval: EUR 2,400-EUR 4,200."
3. Calculate P&L impact: "This reserve will increase incurred losses by EUR 3,100 for [line of business] in [accounting period]."
4. Flag if reserve exceeds adjuster authority level (e.g., adjuster authority is EUR 10,000; recommended reserve is EUR 12,500 -- escalate to supervisor).
5. Track reserve adequacy over time: as new information arrives (supplements, investigation findings), recommend reserve adjustments with explanation.

**Adjuster review:** Review recommended reserve. Accept or adjust based on judgment (e.g., adjuster knows this body shop tends to find hidden damage, so adds a buffer). Every adjustment is captured as training data.

**Time saved:** 10-15 min (manual) --> 1 min review. Reserve calculation is math + comparison; the system does both instantly.

**Why this sub-step matters to CFOs:** Reserve accuracy directly impacts financial statements. A 5% improvement in reserve accuracy at a Caravela-sized carrier (57K claims/year) could mean EUR 500K-EUR 750K in freed capital or avoided losses per year. This is the selling point that opens the CFO as a second buyer. [SOURCE: mysa_product_strategy.md, Part 9b -- ROI calculation]

[SOURCE: mysa_product_strategy.md, Parts 1, 2d; TRANSCRIPT: Feb 7, 2026]

---

### Sub-Step 6: Fraud Detection

**What the adjuster does today:** Looks for red flags -- inconsistencies in the claim narrative, patterns that match known fraud schemes, unusual timing or circumstances, prior claim history that suggests serial fraud.

**Data inputs:**
- All claim data (structured from intake)
- Fraud pattern database (known fraud indicators per claim type)
- External databases (ISO ClaimSearch, NICB, LexisNexis)
- Internal claim history for all parties involved
- Carrier-specific fraud rules from SOP
- Shift Technology / FRISS scores (where available)

**System logic:**
1. Score claim against fraud indicators:
   - Timing anomalies (claim filed immediately after policy inception or renewal)
   - Inconsistencies between narrative, photos, and evidence
   - Prior claim frequency for policyholder (serial claimant pattern)
   - Known fraud patterns (staged accident indicators, inflated medical treatment, phantom passengers)
   - Network analysis (connections between parties, repair shops, attorneys, medical providers)
2. Generate fraud risk score: LOW (0-30) / MEDIUM (30-60) / HIGH (60-100).
3. For HIGH scores: generate SIU referral recommendation with evidence summary listing each red flag and its weight.
4. For MEDIUM scores: generate list of additional investigation steps to confirm or clear suspicion.
5. For LOW scores: clear for processing (no action needed).

**Adjuster review:** Review fraud risk score. For HIGH: confirm SIU referral. For MEDIUM: follow recommended investigation steps. System captures adjuster's fraud assessment decision as training data.

**Time saved:** 5-10 min (manual assessment) --> automated flagging. The adjuster no longer needs to manually check databases and pattern-match. System does it in real time at intake.

**Note:** Mysa is NOT a dedicated fraud detection product (that market is dominated by Shift Technology at ~$320M raised). Fraud detection is one of six sub-steps. The value is integration -- fraud signals feed into the coverage, reserve, and decision steps rather than existing as an isolated score. [SOURCE: mysa_product_strategy.md, Part 1; WEB: Crunchbase -- Shift Technology]

---

### Decision Sub-Steps Summary

| # | Sub-Step | Data Inputs | AI Output | Adjuster Action | Time: Before | Time: After |
|---|----------|-------------|-----------|-----------------|-------------|-------------|
| 1 | Coverage Verification | Policy doc, claim facts, SOP rules | Coverage determination + confidence + cited clauses | Accept/modify/reject | 15-30 min | 2 min |
| 2 | Policy Report Checking | All documents, cross-reference matrix | Gap report + contradiction flags + auto-drafted follow-ups | Confirm follow-ups, resolve contradictions | 10-20 min | 1 min |
| 3 | Repair Assessment | Estimate, photos, comparables, carrier guidelines | Anomaly flags + repair vs total loss assessment | Review flags, negotiate with vendor | 15-25 min | 3 min |
| 4 | Cost Analysis | Validated estimate, market rates, historicals | Cost percentile + driver analysis + expected range | Accept if in range, investigate outliers | 10-20 min | 2 min |
| 5 | Reserve Calculation | Cost analysis, historicals, carrier rules, trajectory | Reserve recommendation + confidence interval + P&L impact | Accept/adjust reserve | 10-15 min | 1 min |
| 6 | Fraud Detection | All claim data, fraud patterns, external databases | Risk score + SIU referral recommendation + evidence summary | Confirm/clear fraud flags | 5-10 min | Automated |
| | **Total** | | | | **65-120 min** | **10-15 min** |

**Productivity gain:** 4-8x on the decision step alone. Decision-making consumes 60-70% of adjuster time, so this translates to a net 2-3x productivity improvement across the full workflow.

[SOURCE: mysa_product_strategy.md, Part 1]

---

## 6.3 SOP-Driven Workflow Engine

### Why SOPs Are the Core Differentiator

Every insurance carrier and TPA operates according to Standard Operating Procedures (SOPs) -- documented processes that define how claims should be handled. These SOPs specify:
- When to escalate
- What authority levels apply at what thresholds
- Which documents are required per claim type
- What investigation steps to follow
- What templates to use for correspondence
- How to calculate reserves
- When to refer to SIU

The problem: SOPs exist as PDFs or Word documents. Nobody reads them during live claims processing. New adjusters take 6 years to internalize them. Veterans develop shortcuts that may or may not follow the SOP. There is no system that enforces or even tracks SOP compliance.

> "Everything that we build, needs to be really around SOP, like, what is the SOP that your insurance company or your TPA follows for that."
> -- Tiago Brigido, Co-founder [TRANSCRIPT: Feb 7, 2026]

> "When we onboard an insurance company, we upload the SOPs, and we also translate those SOPs into workflows. And you can also go there and manually create more workflows."
> -- Tiago Brigido, Co-founder [TRANSCRIPT: Feb 7, 2026]

[SOURCE: mysa_product_strategy.md, Part 1]

### How It Works

**Onboarding Phase:**

```
1. UPLOAD
   Carrier uploads SOPs (PDF, Word, scanned docs)
   Mysa OCR extracts rules, thresholds, escalation paths, templates

2. PARSE
   AI identifies discrete workflow rules within SOPs:
   - "If repair estimate exceeds EUR 10,000, escalate to supervisor"
   - "Total loss threshold: 75% of ACV for vehicles < 3 years old"
   - "Coverage denial requires written letter within 5 business days citing
     specific policy clause"
   - "SIU referral if fraud score > 70 OR if 3+ claims in 12 months"

3. STRUCTURE
   Rules are organized into decision trees per claim type:
   - Motor PD (physical damage) -- convention claim
   - Motor PD -- non-convention claim
   - Motor BI (bodily injury)
   - Motor total loss
   - Property -- water damage
   - Property -- fire
   - Property -- storm/weather
   - Liability -- general
   - [Custom per carrier]

4. REVIEW
   Carrier claims manager reviews generated workflows.
   Adjusts thresholds, adds missing rules, confirms logic.
   This is a human validation step -- AI proposes, human confirms.

5. ACTIVATE
   Workflows go live. Every claim entering the system is matched to the
   appropriate workflow based on claim type and complexity.
```

**Per-Claim Phase:**

```
Claim data arrives
  -> Mysa matches claim type to relevant SOP workflow(s)
  -> AI walks adjuster through each decision step per carrier's own rules
  -> At each step, system checks: "Does this conform to SOP?"
  -> Documents generated per carrier's templates and requirements
  -> Decisions checked against SOP compliance
  -> Deviations flagged with explanation required from adjuster
```

### Three Workflow Types

The Feb 9 call defined three categories of workflows that must coexist:

| Type | Description | Source | Example |
|------|-------------|--------|---------|
| **Standard (always-deployed)** | Best-practice workflows built from industry standards. Available to all carriers from Day 1. | Mysa's domain knowledge | "Motor PD -- simple collision" workflow with industry-standard steps |
| **Carrier-customized** | Workflows generated from carrier's own SOPs. Carrier-specific thresholds, templates, authority levels. | Carrier SOP upload | Caravela's specific reserve authority matrix (EUR 5K desk, EUR 15K supervisor, EUR 50K VP) |
| **Net-new** | Workflows the carrier wants to create that don't exist in their current SOPs. Mysa helps build them. | Carrier request + Mysa guidance | "AI-assisted triage for property claims" -- new workflow for a carrier expanding into property |

[SOURCE: meeting_notes_2026-02-09_claims_workflow.md]

### Why This Creates Lock-In

Once a carrier's SOPs are encoded into Mysa's workflows:

1. **Switching costs are high** -- reconstructing SOP-driven workflows in a competitor system means re-doing the onboarding work
2. **Institutional knowledge is captured** -- the workflows represent carrier-specific expertise that may not even be fully documented in the SOPs themselves (adjusters add corrections during review)
3. **Training data is carrier-specific** -- every adjuster interaction with the workflows creates training data that only works within Mysa's system
4. **Compliance depends on it** -- once a carrier uses Mysa for SOP compliance tracking, removing it means losing the audit trail

[SOURCE: mysa_product_strategy.md, Part 1 -- SOP-driven workflow generation; CLAUDE ANALYSIS]

---

## 6.4 The Core Loop

### Trigger -> Action -> Reward -> Investment

This is the behavioral loop that drives adoption and creates the data flywheel.

```
+-------------------------------------------------------------------+
|                                                                     |
|  TRIGGER: Claim arrives on adjuster's desk                         |
|     (email notification, CMS queue, supervisor assignment)          |
|                                                                     |
|     |                                                               |
|     v                                                               |
|                                                                     |
|  ACTION: Adjuster reviews Mysa's AI-generated decisions            |
|     - 6 sub-step recommendations pre-filled                        |
|     - Documents pre-generated                                       |
|     - SOP compliance checked                                        |
|     Adjuster: ACCEPT / MODIFY / REJECT each recommendation         |
|                                                                     |
|     |                                                               |
|     v                                                               |
|                                                                     |
|  REWARD: Claim resolved in 10-15 min instead of 65-120 min        |
|     - Adjuster feels competent (AI supports their judgment)         |
|     - Adjuster goes home on time (caseload manageable)              |
|     - Supervisor sees consistent decisions (fewer audit flags)      |
|     - New hire feels confident (SOP guides every step)              |
|                                                                     |
|     |                                                               |
|     v                                                               |
|                                                                     |
|  INVESTMENT: Every accept/modify/reject trains the model           |
|     - Accepts = positive training signal                            |
|     - Modifications = correction data (most valuable)               |
|     - Rejections = negative signal with adjuster's alternative      |
|     - Over time: recommendations get better                         |
|     - Over more time: routine claims need minimal review            |
|     - Eventually: near-STP for simple claims                        |
|                                                                     |
|     |                                                               |
|     +-----------> Back to TRIGGER (next claim, better model)       |
|                                                                     |
+-------------------------------------------------------------------+
```

### The Flywheel Timeline

```
Day 1:    SOP workflows + document parsing -> basic recommendations
            (60% recommendation accuracy -- out-of-the-box)

Month 3:  Historical claims data ingested -> better comparable matching
            (70% accuracy -- historical context improves recommendations)

Month 6:  Decision ground truth captured (adjuster accepts/modifies/rejects)
            -> model learns carrier-specific patterns
            (80% accuracy -- model adapts to this carrier's decision style)

Month 12: Enough data to predict outcomes -> proactive recommendations
            (85-90% accuracy -- system anticipates what adjuster will decide)

Month 18+: Models can handle routine decisions with minimal review -> near-STP
            (90%+ for routine claims -- adjuster reviews by exception only)
```

> "When we come in and we use the historical data, and the out-of-the-box thing, we get 60%. As soon as we start getting better data and training the models, we go to 70 or 80%."
> -- Tiago Brigido, Co-founder [TRANSCRIPT: Feb 7, 2026]

> "The second time that you have a second case, for that claim type, it will be always [faster] and it might already be slightly automated because our AI [learned from the first one]."
> -- Tiago Brigido, Co-founder [TRANSCRIPT: Feb 7, 2026]

### Why the Loop Compounds

The critical insight: Mysa captures not just what was decided, but **why**. Every competitor has claim outcomes (what was paid). Nobody has decision reasoning (why the adjuster decided what they decided). This is a new data category.

> "You see the end result. You see what you order and the end result. That's a claim. That's what they get. They don't know exactly how they got to that end result."
> -- Tiago Brigido, Co-founder [TRANSCRIPT: Feb 7, 2026]

[SOURCE: mysa_product_strategy.md, Parts 1, 5a -- Feedback Loop; TRANSCRIPT: Feb 7, 2026]

---

## 6.5 The "Clippy" Architecture

### Concept: Insurance Knowledge Clippy

The product's primary delivery mechanism is not a standalone portal. It is a Chrome extension -- an always-present overlay that sits on top of whatever system the adjuster already uses. The analogy: what Superhuman did for email, Mysa does for claims.

> "Insurance knowledge Clippy" -- sits on top of whatever system the adjuster uses. Like Superhuman for email. Context-aware across all pages. Chat with Vault knowledge base.
> [SOURCE: MODULE_01_POSITIONING.md, Section 1.6; TRANSCRIPT: Feb 9, 2026]

[SOURCE: meeting_notes_2026-02-09_claims_workflow.md; MODULE_07_TECHNICAL.md, Section 7.7]

### Why a Chrome Extension

**The integration problem:** Mid-market carriers run a mix of systems -- Guidewire ClaimCenter, Duck Creek Claims, homegrown web apps, legacy mainframe terminals accessed through browser emulators, and various vendor portals. Getting API access to any of these takes 6-18 months of partnership negotiation. Most mid-market carriers do not have the IT resources to build custom integrations.

**The solution:** A Chrome extension that reads what the adjuster sees on screen, without requiring backend access to the carrier's CMS.

### How It Works

```
ADJUSTER'S EXISTING WORKFLOW
  |
  +-- Opens browser (Guidewire ClaimCenter, Duck Creek, legacy web app, email)
  |     |
  |     +-- Mysa Chrome Extension reads page context
  |     |     - Claim number, policy data, reserve amounts
  |     |     - Page structure recognition (which CMS, which screen)
  |     |     - Documents visible on screen
  |     |
  |     +-- Mysa overlay panel appears (side panel or floating):
  |           - Coverage analysis recommendation
  |           - Convention match result (EU motor)
  |           - Reserve suggestion with confidence interval
  |           - SOP compliance checklist
  |           - "Ask Vault" chat interface for knowledge queries
  |           - Document generation buttons
  |           - Decision log (accept/modify/reject)
  |
  +-- Adjuster reviews recommendations in overlay
  |     |
  |     +-- Accepts / modifies / rejects each recommendation
  |           (every interaction = training data)
  |
  +-- Adjuster enters decision into their CMS (their normal workflow)
        |
        +-- Extension captures: what was decided vs what was recommended
```

[SOURCE: MODULE_07_TECHNICAL.md, Section 7.7]

### Three Components of the Clippy Architecture

#### 1. The Overlay (Always-On Side Panel)

The core interface. Appears when the adjuster is viewing a claim in any browser-based system. Contains:

| Panel Section | Content | Interaction |
|---------------|---------|-------------|
| **Claim Summary** | Structured claim data extracted from OCR + current page | Auto-populated, adjuster can correct |
| **Decision Cards** | 6 sub-step recommendations, each with confidence score and reasoning | Accept / Modify / Reject per card |
| **SOP Checklist** | Carrier-specific SOP steps for this claim type, with completion tracking | Checkbox progress |
| **Alerts** | Missing documents, SOP deviations, authority exceedances, fraud flags | Actionable links |
| **Documents** | One-click generation of all required documents per SOP | Generate / preview / send |

#### 2. The Vault (Knowledge Base)

A searchable, carrier-specific knowledge base that the adjuster can chat with in natural language. Contains:

| Knowledge Source | Content | Example Query |
|------------------|---------|---------------|
| **Carrier SOPs** | All uploaded SOPs, parsed and indexed | "What's the authority limit for PD reserves?" |
| **Policy Library** | All policy forms used by this carrier | "Does the HO-3 cover mold remediation?" |
| **Convention Rules** | IDS, IRSA, CARD, CIDE -- all convention tables | "What IRSA scenario applies to a rear-end collision?" |
| **State/Country Regulations** | Insurance regulations per jurisdiction | "What's the statute of limitations for motor PD in Texas?" |
| **Decision History** | Past decisions on similar claims (anonymized) | "How did we handle similar water damage claims last year?" |

Every answer from the Vault includes a citation: "From: [SOP Section 4.3 -- Investigation Procedures]" or "From: [IRSA Convention, Scenario 4]." This is critical for trust and audit trail.

[SOURCE: meeting_notes_2026-02-09_claims_workflow.md; claims_journey_discovery.md, lines 11516-11520]

#### 3. The Context Engine

The background intelligence that powers both the Overlay and the Vault. It:

- Recognizes which CMS the adjuster is using (Guidewire, Duck Creek, legacy portal) and adapts screen-reading logic
- Tracks which claim is currently being viewed and pre-loads relevant data
- Maintains session context across multiple browser tabs (adjuster may have CMS, email, and estimation tool open simultaneously)
- Stores local context for fast response (Vault queries should feel instant, not require a round-trip to server)

### Why This Architecture Wins

| Advantage | Explanation |
|-----------|-------------|
| **Zero integration required** | Works on Day 1 with any browser-based CMS. No API partnership needed. |
| **No workflow change** | Adjuster keeps using their existing system. Mysa sits alongside, not in the way. |
| **Data capture from Day 1** | Every interaction (accept/modify/reject) creates training data, regardless of CMS integration status. |
| **Sales objection killer** | "We don't change how you work. We sit on top of your existing system." This removes the #1 adoption barrier. |
| **Platform agnostic** | Same extension works on Guidewire, Duck Creek, homegrown systems, Colossus output screens, legacy terminals. |

### Limitations

- **Read-only on locked systems:** The extension can read data from any browser page but cannot write data back to locked CMSes. Adjuster must still enter decisions manually into their CMS.
- **UI dependency:** If a carrier's CMS changes its interface layout, the extension's screen-reading logic may need updating.
- **Enterprise browser policies:** Some large carriers may block browser extensions. This is less common at mid-market carriers (the primary target).
- **Non-browser applications:** Thick-client (non-browser) applications require a desktop agent component, not just a Chrome extension.

[SOURCE: MODULE_07_TECHNICAL.md, Section 7.7; TRANSCRIPT: Feb 9, 2026]

---

## 6.6 All Personas & How the Product Helps Each

Every claim involves a network of professionals. Mysa touches most of them -- directly as users, or indirectly through data exchange and workflow integration. This table maps each persona to their pain, Mysa's help, and the corresponding demo screen.

| Persona | Primary Pain Point | How Mysa Helps | Demo Screen |
|---------|--------------------|----------------|-------------|
| **Desk Adjuster** | Drowning in 125+ open claims. 30-40% of time on admin. 65-120 min per decision. Inconsistent outcomes across adjusters. | Primary user. AI pre-fills 6 decision sub-steps. 65-120 min --> 10-15 min per claim. SOP-guided workflows for consistency. Documents auto-generated. | **Adjuster Dashboard:** Claim queue with priority scoring. Click into claim --> 6 decision cards pre-filled. Accept/modify/reject per card. One-click document generation. |
| **Field Adjuster** | Coordinates inspections, interviews, evidence collection. 2.7 call attempts per party. 30-40% of investigation time wasted on phone tag. Documentation burden (5-10 min documentation per 10 min investigation). | Investigation scoping per SOP. Call recording + transcription. Auto-generated investigation summaries. Evidence checklist with completion tracking. | **Investigation Panel:** SOP-driven checklist. Call recording widget. Auto-transcription. Document generation. Outstanding items tracker. |
| **BI (Bodily Injury) Adjuster** | Complex medical records (50-500+ pages). Treatment appropriateness assessment. BI negotiations span months. Colossus dependency for valuation. | Medical record parsing. Treatment timeline visualization. Comparable injury analysis. Reserve calculation with BI-specific models. Colossus output integration. | **BI Decision Panel:** Medical timeline. Treatment cost analysis. Comparable injury outcomes. Reserve recommendation with confidence interval. |
| **SIU Investigator** | False positive rate on fraud referrals wastes time. Manual pattern matching across databases. Evidence compilation for investigation is manual. | Receives pre-compiled fraud referral packages with scored red flags. Network analysis (connections between parties). Evidence summary auto-generated. | **SIU Referral View:** Fraud score with weighted indicators. Network graph. Evidence timeline. Red flag list with severity. |
| **Supervisor / Team Lead** | Reviews decisions above authority. Manages 10-30 adjusters. Cannot see SOP compliance across team. Bottleneck for escalations. | Decision audit trail dashboard. SOP compliance scores per adjuster. Workload distribution visualization. Batch review of AI-recommended decisions for escalated claims. | **Supervisor Dashboard:** Team view with KPIs. SOP compliance heatmap. Escalation queue. Decision variance report. |
| **Broker / Agent** | Back-and-forth with customers to collect claim information. Manual email-to-claim creation. No visibility into claim status after submission. | White-labeled FNOL forms. Chrome extension on email for one-click claim creation (like Superhuman). AI gap analysis reduces policyholder back-and-forth. Status visibility. | **Broker Portal:** FNOL form builder. Email-to-claim creation (select text --> create claim). Gap analysis alerts. Claim status tracker. |
| **Appraiser** | Scheduling delays for inspections. Estimate disputes with carriers. Re-inspection for supplements adds days. | Receives structured data feeds: claim photos, repair scopes, comparable estimates. Outputs structured estimate back into Mysa for decision workflow. | **Data Exchange:** Structured estimate ingestion. Supplement request and approval workflow. |
| **Medical Case Manager** | Complex treatment timelines. Return-to-work probability unknown. Treatment cost projections manual. | Treatment timeline tracking. Medical cost analysis against comparable injuries. Return-to-work probability scoring from historical data. | **Medical Timeline View:** Treatment events, cost accrual, RTW probability, comparable outcomes. |
| **VP Claims / CCO** | Staffing crisis. Inconsistent decisions. STP gap (10% actual vs 60-70% promised). Growing open claims backlog. | 3x adjuster productivity. New adjusters productive in weeks. Consistent decisions per SOP. STP rate improvement. Decision audit trail for compliance. | **Executive Dashboard:** Claims throughput. STP rate. Reserve accuracy. Adjuster productivity. SOP compliance. Decision consistency scores. |
| **CFO / Finance Director** | Reserve surprise at year-end. Capital tied up in over-reserves. Regulatory capital adequacy pressure. | AI-calculated reserves with confidence intervals. P&L impact per claim. Portfolio-level reserve accuracy reporting. Reserve development tracking. | **Finance View:** Reserve adequacy dashboard. P&L impact by LOB. Reserve development triangle. Capital efficiency metrics. |

[SOURCE: MODULE_01_POSITIONING.md, Section 1.3; claims_journey_discovery.md -- full persona mapping; TRANSCRIPT: Feb 9, 2026]

---

## 6.7 User Journey Maps

### Journey 1: New Claim Intake (Desk Adjuster -- Motor PD)

| Step | User Action | System Logic | Emotional Outcome |
|------|-------------|-------------|-------------------|
| 1. Notification | Adjuster sees new claim in queue (email alert or CMS notification) | Claim has been parsed, structured, and triaged by Steps 1-3. Priority score assigned. | **Neutral** -- another claim, but priority is clear |
| 2. Open claim | Adjuster clicks claim in Mysa overlay (or opens in CMS, extension activates) | System loads claim context: structured data, documents, initial recommendations | **Curious** -- "let's see what Mysa found" |
| 3. Review summary | Adjuster reads claim summary: parties, damage, timeline, policy status | System highlights key facts: fault indicators, damage description, policy coverage status | **Informed** -- all context in one view, no system-hopping |
| 4. Coverage check | Adjuster reviews coverage determination card. "COVERED -- Section I, Coverage A. Deductible: EUR 500." | Sub-Step 1 output with cited policy clauses. Green highlight = covered perils. Red = exclusions. | **Confident** -- AI confirmed what adjuster suspected. Cited clauses provide backup. |
| 5. Report check | Adjuster sees gap report: "Police report: RECEIVED. Counterparty statement: MISSING." | Sub-Step 2 output. Auto-drafted SMS to counterparty requesting statement. | **Relieved** -- system caught what adjuster might have missed |
| 6. Repair review | Adjuster sees estimate flagged: "Labor rate 15% above regional average. OEM parts specified; carrier SOP requires aftermarket for vehicles > 5 years." | Sub-Step 3 output. Anomaly flags with specific line items. | **Empowered** -- has specific negotiation points for body shop call |
| 7. Cost review | "Estimated total: EUR 2,800. 68th percentile for similar claims. Within expected range." | Sub-Step 4 output. Comparable distribution chart. | **Validated** -- claim is normal, no surprises |
| 8. Reserve | "Recommended reserve: EUR 3,100. 90% CI: EUR 2,400-EUR 4,200. Within authority." | Sub-Step 5 output. P&L impact note. Authority check passed. | **Decisive** -- clear number, within authority, no escalation needed |
| 9. Fraud check | "Fraud score: 12/100 (LOW). No indicators flagged." | Sub-Step 6 output. Green checkmark. | **Clear** -- no red flags, move forward |
| 10. Decision | Adjuster clicks "Accept All" (or modifies individual cards). Decision logged. | All 6 sub-steps recorded: recommendation + adjuster action + timestamp. Documents auto-generated. | **Accomplished** -- claim decided in 12 minutes. 5 more before lunch. |
| 11. Documents | Settlement recommendation letter, reserve memo auto-generated. Adjuster reviews, clicks "Send." | Document generation per carrier SOP template. Sent to policyholder and/or broker. | **Done** -- no manual typing, no template hunting |

**Total time: ~12 minutes. Previous workflow: ~90 minutes.**

---

### Journey 2: Investigation (Field Adjuster -- Complex Motor)

| Step | User Action | System Logic | Emotional Outcome |
|------|-------------|-------------|-------------------|
| 1. Assignment | Field adjuster receives claim assigned as "complex -- requires investigation" | Triage scored HIGH complexity: disputed liability, multiple parties, potential BI | **Alert** -- this needs attention |
| 2. Investigation plan | Reviews SOP-generated investigation checklist: recorded statements (3 parties), police report, photos, witness contact, body shop inspection | Step 4 logic: checklist generated from carrier SOP for this claim type. Outstanding items tracked. | **Organized** -- clear plan, nothing missed |
| 3. Call prep | Before calling Party A, reviews Mysa's call guide: suggested questions per SOP, key facts to verify, contradictions to probe | Investigation Agent provides scripted questions based on claim facts and SOP requirements | **Prepared** -- knows exactly what to ask |
| 4. Call recording | Makes call. Mysa records and transcribes. Key facts auto-extracted from transcript. | Recording + real-time transcription. Fact extraction: "Party A states they were stopped at a red light" | **Focused** -- can concentrate on listening, not note-taking |
| 5. Evidence review | Reviews photos uploaded by both parties. Mysa flags: "Front damage on Party A inconsistent with claimed rear-end collision" | Photo analysis + narrative cross-reference. Inconsistency flag. | **Vigilant** -- AI caught something worth investigating further |
| 6. Liability determination | Reviews Mysa's liability recommendation: "60/40 Party A / Party B based on evidence analysis" with reasoning chain | Sub-Step integrated with investigation findings. Confidence score + alternative scenario. | **Thoughtful** -- recommendation is a starting point for adjuster's own judgment |
| 7. Escalation | Claim complexity score updated. Reserve exceeds authority. Mysa routes to supervisor with full evidence package. | Authority check failed. Auto-generated escalation memo with decision rationale + evidence summary. | **Relieved** -- escalation is clean, supervisor gets full context without verbal walkthrough |

---

### Journey 3: Decision (Desk Adjuster -- US Property Water Damage)

| Step | User Action | System Logic | Emotional Outcome |
|------|-------------|-------------|-------------------|
| 1. Claim arrives | Email from homeowner: "Water in my basement. Photos attached." | Intake parsing extracts: water damage, basement, photos analyzed for extent (~200 sq ft). Policy loaded. | **Routine** -- common claim type |
| 2. Coverage question | Mysa flags: "Coverage determination requires: was this sudden or gradual? HO-3 Section I covers sudden accidental discharge. Exclusion 2.c excludes gradual seepage." | Coverage Agent identified the decision fork. Generated specific investigation steps to resolve. | **Focused** -- the key question is clear immediately |
| 3. Investigation | Adjuster requests plumber's report. Mysa auto-drafts request email. Tracks as outstanding item. | Investigation Agent generates request per SOP. Diary date set. Auto-follow-up if not received in 5 business days. | **Efficient** -- one click, request sent, follow-up automatic |
| 4. Evidence arrives | Plumber's report uploaded. Mysa parses: "Pipe failure due to sudden rupture. No evidence of prior leakage or corrosion." | Document parsing extracts key finding. Updates coverage determination: "COVERED -- sudden burst confirmed." | **Resolved** -- evidence confirms coverage |
| 5. Settlement | Reserve set: "$9,200. Based on 312 comparable water damage claims in this region. 90% CI: $7,400-$11,800." Documents generated. | Full 6 sub-steps executed. All documents per SOP. Settlement offer letter generated. | **Complete** -- from ambiguity to resolution, guided by system |
| 6. What-if (denial path) | If plumber's report had found gradual seepage: "Exclusion 2.c APPLIES. Recommend DENIAL." Denial letter auto-generated with policy citations. | Same system, opposite outcome. Coverage Agent reasons in both directions. Denial letter cites specific clause. | **Protected** -- denial is documented, defensible, per SOP |

---

### Journey 4: Settlement (EU Motor -- Convention Claim)

| Step | User Action | System Logic | Emotional Outcome |
|------|-------------|-------------|-------------------|
| 1. Decision complete | Decision approved: coverage confirmed, liability assigned via CIMPAS convention, reserve set | All 6 sub-steps accepted. Convention match: CIMPAS Case 7, 100% to Party A. | **Clear** -- decision is clean |
| 2. Offer generation | Mysa calculates settlement: repair estimate EUR 2,400 minus EUR 500 deductible = EUR 1,900 | Settlement calculation per carrier rules. Authority check: within desk adjuster limit. | **Straightforward** -- math is simple, system confirms |
| 3. Offer communication | Settlement letter generated and sent to policyholder via preferred channel (email, post) | Document Agent generates per carrier template. Tracks delivery and response. | **Professional** -- no manual letter drafting |
| 4. Payment authorization | Adjuster approves payment within authority. Payment routed to finance for processing. | Authority matrix check. Payment request submitted to carrier's payment system. | **Done** -- claim moves to finance without paperwork |
| 5. Convention submission | Mysa generates convention data package for CIMPAS submission. Structured data for clearing house. | Convention data output per CIMPAS format. Inter-insurer reimbursement triggered at forfait rate. | **Automated** -- convention submission is data output, not manual entry |
| 6. Closure | Claim status updated. File closed. Reserve adjusted to match actual payment. | File closure checklist per SOP completed. Reserve-to-payment reconciliation. Training data captured. | **Satisfied** -- clean close, full audit trail |

[SOURCE: mysa_product_strategy.md, Parts 1, 5a, 8; claims_journey_discovery.md, Phases 6-11; TRANSCRIPT: Feb 9, 2026]

---

## 6.8 Human-in-the-Loop: Why

### The Non-Negotiable Design Principle

Mysa recommends. Humans decide. This is not a limitation -- it is a feature with four distinct justifications.

> "It's mandatory to always have a human step."
> -- Jeremy Blehaut, Co-founder [TRANSCRIPT: Feb 7, 2026]

---

### (a) Regulatory Requirement

**EU AI Act (Regulation 2024/1689):** Insurance claims AI will be classified as "high-risk" under Annex III -- AI systems used in contexts that affect access to essential services. High-risk classification requires:

| Requirement | What It Means | Mysa's Compliance |
|-------------|--------------|-------------------|
| Human oversight (Art. 14) | A natural person must be able to understand, interpret, and override AI outputs | Adjuster reviews every recommendation. Accept/modify/reject on every sub-step. |
| Transparency (Art. 13) | Users must be informed they are interacting with AI; system must explain its outputs | Every recommendation includes confidence score + reasoning chain + cited evidence |
| Conformity assessment (Art. 43) | System must undergo assessment before deployment in high-risk context | Architecture designed for assessment from Day 1 |
| Risk management (Art. 9) | Ongoing risk management system for the AI | Decision ground truth tracking identifies when AI recommendations diverge from human decisions |
| Data governance (Art. 10) | Training data must meet quality criteria | Every training data point is human-validated (adjuster decision) |

**GDPR Article 22:** Prohibits fully automated decisions with legal or similarly significant effects on individuals. A claims decision (approve, deny, settle amount) has direct legal and financial effect on the policyholder. Human oversight is required.

**US State Regulations:** While the US lacks a federal AI Act, individual states are enacting AI oversight rules for insurance. Colorado SB 21-169 (enacted 2021) requires insurers to test AI/ML for unfair discrimination. New York Circular Letter No. 1 (2019) requires oversight of AI-driven underwriting and claims decisions.

[SOURCE: mysa_product_strategy.md, Part 5d; WEB: EU AI Act (Regulation 2024/1689), Annex III; WEB: GDPR Article 22; REGULATORY_COMPLIANCE.md]

---

### (b) Trust: Adjusters Will Not Use Black Boxes

Adjusters have deep professional pride. They are experts who have spent years developing judgment. A system that says "here's the answer, trust me" will be rejected. A system that says "here's my analysis and reasoning -- what do you think?" will be adopted.

**The adoption gradient:**

| System Behavior | Adjuster Reaction | Adoption Rate |
|----------------|-------------------|---------------|
| "Claim denied. Amount: $0." (no explanation) | "I don't trust this. I'll do it myself." | <5% |
| "Recommend denial based on Exclusion 2.c. Here's why..." (with reasoning) | "Interesting. Let me check that... yes, that's right." | 40-60% |
| "Here's my analysis of coverage, with the relevant clauses highlighted. You decide." (decision support) | "This is useful. It saved me 20 minutes of reading." | 70-90% |

The goal is the third pattern. Mysa provides the analysis. The adjuster provides the judgment. Over time, as trust builds, the adjuster moves toward the second pattern -- reviewing AI reasoning rather than doing independent analysis.

**Key UX principle:** Every AI recommendation must be dismissible. The adjuster must never feel trapped by the AI's suggestion. The "modify" and "reject" options must be as prominent as "accept."

---

### (c) Training Data: Every Correction Improves the Model

Human-in-the-loop is the engine that powers the flywheel (Section 6.4). Without human decisions, the model cannot learn.

| Adjuster Action | Training Signal | Value |
|-----------------|----------------|-------|
| **Accept** | Positive reinforcement -- AI recommendation was correct | Confirms model accuracy for this pattern |
| **Modify** | Correction -- AI was directionally right but details wrong | Most valuable signal. Teaches model the precise adjustment. Example: "Reserve was $3,100 but I set it to $3,500 because I know this body shop always finds supplements." |
| **Reject** | Negative signal -- AI was wrong | Teaches model what NOT to recommend. Adjuster's alternative becomes ground truth. |

**The modification signal is the most valuable.** An accept tells you "keep doing this." A reject tells you "don't do this." A modification tells you "do this, but slightly different, and here's how." This is the data that no competitor captures.

---

### (d) Liability: Human Decides, AI Recommends

If an AI makes a claims decision that turns out to be wrong -- a wrongful denial, an underpaid claim, a missed fraud case -- who is liable?

**Current legal framework:** The carrier is liable for claims decisions. If an adjuster makes a bad decision, the carrier bears the consequences (bad faith lawsuit, regulatory action, financial loss).

**With AI in the loop:** If the AI made the decision autonomously, the liability question becomes complex and untested in court. If the AI recommended and the human decided, the liability framework is unchanged -- the carrier is responsible for the human's decision, and the AI was a tool that informed it.

**This matters for sales:** VP Claims will not approve a system that creates new liability exposure. "The AI recommends, but your adjuster always decides" is a critical sales message. It means Mysa augments the existing liability framework rather than disrupting it.

| Scenario | Without Mysa | With Mysa (Human-in-the-Loop) |
|----------|-------------|-------------------------------|
| Wrongful denial | Adjuster error. Carrier liable. Standard bad faith claim. | AI recommended denial with reasoning. Adjuster reviewed and approved. Same liability as before -- but better documented. |
| Overpayment (leakage) | Adjuster missed red flags. Carrier absorbs loss. | AI flagged anomalies. Adjuster overrode. Decision logged. If adjuster ignored flags, that's documented for internal review. |
| Missed fraud | Adjuster didn't catch indicators. SIU never saw it. | AI flagged fraud risk. If adjuster dismissed flag, that's documented. If AI missed it, same outcome as today -- but system improves from the miss. |

[SOURCE: mysa_product_strategy.md, Part 5d; TRANSCRIPT: Feb 7, 2026; REGULATORY_COMPLIANCE.md]

---

## 6.9 Demo Spec: Adjuster Portal

### Design Principle: Block by Block

> "I tried to build two demos today, and they basically... I think we need to build block by block."
> -- Tiago Brigido, Co-founder [TRANSCRIPT: Feb 7, 2026]

> "Yeah. It has to be. Otherwise, it goes everywhere and nowhere at the same time."
> -- Jeremy Blehaut, Co-founder [TRANSCRIPT: Feb 7, 2026]

**Principle:** Do not try to show the full product. Show specific, impressive steps. Each demo is a focused scenario that demonstrates a concrete workflow from start to decision.

[SOURCE: mysa_product_strategy.md, Part 8]

---

### Demo 1: EU Motor -- EAS to Settlement ("The Easy Case")

**Scenario:** Portuguese motor claim. Two-car fender bender. No injuries. Paper EAS form filled out at scene. Straightforward convention claim.

> "On the demo, we already see that, oh, let me call the repair shop. But that's a demo like this. It's the most easy case possible."
> -- Tiago Brigido, Co-founder [TRANSCRIPT: Feb 7, 2026]

**Step-by-step flow:**

| Step | What Shows on Screen | What to Highlight (Talking Point) | Technical Requirement |
|------|---------------------|-----------------------------------|----------------------|
| **1. Claim arrives** | Email inbox view. New email with scanned EAS form attachment. Subject: "Sinistro AUTO-2026-04812." | "This is what arrives today -- a messy, handwritten paper form attached to an email. This is where every motor claim in Europe starts." | Email parsing, attachment extraction |
| **2. OCR extraction** | Split screen: raw EAS image on left (messy handwriting, crossed-out fields, coffee stain on corner). Structured data table on right, populating field by field in real time. | "In 30 seconds, Mysa extracts every field from this handwritten form. Watch the accuracy on this handwriting -- our OCR engine handles real-world document quality, not just clean samples." Show specific hard-to-read fields being correctly extracted. | Caravela OCR engine running on EAS form. Real-time extraction visualization. |
| **3. Missing data flagged** | Orange alert banner: "2 issues found." Detailed view: (1) "Counterparty policy number: MISSING" (2) "Checkbox 7 (changing lanes): AMBIGUOUS -- confidence 62%." | "Mysa catches what humans miss. The counterparty forgot to write their policy number. And this checkbox is marked ambiguously -- the system flags it rather than guessing." | Field validation, completeness checking, confidence thresholds |
| **4. Auto-outreach** | Draft SMS displayed: "Caro(a) Sr(a). [Name], referente ao sinistro de 07/02/2026. Necessitamos do numero de apolice do outro condutor. Pode confirmar? Obrigado, [Carrier name]." Button: "Send" / "Edit" | "Automated follow-up in the policyholder's language -- no adjuster time spent. The adjuster can edit before sending, or send as-is." | Template generation in carrier's language, SMS/email integration |
| **5. Convention match** | After missing data resolved: green banner: "CIMPAS Match: Case 7 -- Reversing vehicle collides with parked vehicle. Confidence: 95%." Visual: EAS checkbox pattern mapped to convention case diagram. | "The convention system is a solved problem -- it's a lookup table. The bottleneck was always getting clean, structured data FROM the messy form INTO the convention system. That's what we just did in 30 seconds." | Convention matching engine (deterministic rules for CIMPAS) |
| **6. Fault determination** | Decision card: "Based on checkboxes 2, 4, 7 and diagram analysis: 100% liability to Party A (reversing vehicle). Convention: deterministic -- no adjuster judgment required for fault allocation." | "Show the reasoning chain. Not just the answer -- the WHY. Every checkbox, every rule, cited and traceable. This is what auditors and compliance teams need." | Explainable AI output, convention rule citation |
| **7. Reserve recommendation** | Decision card: "Estimated repair: EUR 2,400-EUR 3,100. Recommended reserve: EUR 3,100. Based on 847 similar claims in the Lisbon region for this vehicle class." Chart: histogram showing distribution of similar claims with this claim's position marked. | "The reserve is calculated from historical data -- not a guess. And here's the P&L impact: this EUR 3,100 is immediately recognized as a loss on the carrier's books. Getting this number right matters." | Historical data matching, statistical reserve model |
| **8. Settlement recommendation** | Full recommendation panel: reserve set, settlement offer calculated (EUR 2,400 minus EUR 500 deductible = EUR 1,900). Auto-generated documents: settlement offer letter, reserve memo, convention data submission. | "Before: 3-5 days, 45 minutes of adjuster time per claim. After: 4 minutes of review. Everything is generated -- the letter, the memo, the convention submission. The adjuster just reviews and clicks approve." | Document generation per carrier SOP template |
| **9. Adjuster review** | Three buttons prominent: ACCEPT ALL / REVIEW INDIVIDUAL / MODIFY. Adjuster clicks "Accept All." Green confirmation: "Decision logged. Documents sent. Convention data submitted. File updated." | "The human always decides. The AI recommends. And notice -- that click just created training data. The model learned that for this pattern, this was the right answer. Next time, it's even more confident." | Human-in-the-loop UI, decision logging, training data capture |

**What makes this demo impressive:**
- **Speed:** 30 seconds from paper EAS to structured data
- **Accuracy:** On real-world messy handwriting, not clean samples
- **Automation:** Convention matching is instant once data is clean
- **Documents:** Everything generated automatically, in the carrier's language and template
- **Before/after:** 3-5 days --> 4 minutes
- **The flywheel:** Every decision makes the system smarter

[SOURCE: mysa_product_strategy.md, Part 8 -- Demo 1]

---

### Demo 2: US Property -- Water Damage ("The Hard Case")

**Scenario:** Homeowner reports water damage in basement. Standard HO-3 policy (Homeowners 3 -- the most common US homeowners policy form, covering dwelling and personal property against named perils). The key question: is this covered? Sudden burst pipe = covered. Gradual seepage = excluded.

> "Imagine that you get the claim. It's a water leakage. You have, oh, let me look at the images on my desk. Let me check. Okay. Actually, this seems a bit -- I'm not sure. So I need to send someone there."
> -- Tiago Brigido, Co-founder [TRANSCRIPT: Feb 7, 2026]

**Step-by-step flow:**

| Step | What Shows on Screen | What to Highlight (Talking Point) |
|------|---------------------|-----------------------------------|
| **1. Claim arrives** | Email from homeowner: "We came home from vacation and found 3 inches of standing water in our basement. The wall is buckling. Photos attached." Three photos: standing water, damaged drywall, wet furniture. | "This is what lands on a desk adjuster's screen. A scared homeowner, some photos, and a question: is this covered?" |
| **2. Photo analysis** | Mysa annotates photos: "Water damage detected. Affected area: ~200 sq ft. Damage severity: MODERATE-HIGH. Visible: standing water (3-4 inches), drywall damage (buckling indicates prolonged exposure), water staining on baseboards." | "AI reads photos, not just stores them. The system identifies damage type, estimates affected area, and notes details the adjuster will need -- like the buckling, which hints at the duration question that will matter for coverage." |
| **3. Policy parsing** | HO-3 policy loaded. Split view: full policy on left (40+ pages). On right: extracted coverage map. Green highlight: "Section I, Coverage A -- Dwelling. Covered: sudden and accidental discharge of water." Red highlight: "Exclusion 2.c -- Water damage: continuous or repeated seepage over 14+ days." | "Mysa reads the WHOLE policy -- not just the declarations page. Coverage clauses highlighted in green, exclusions in red. The adjuster sees the relevant sections without reading 40 pages." |
| **4. Coverage question identified** | Yellow decision card: "COVERAGE DETERMINATION REQUIRES INVESTIGATION. Key question: Was this damage caused by sudden pipe burst (COVERED under Section I) or gradual seepage (EXCLUDED under 2.c)? Evidence needed: plumber's inspection report." | "This is the judgment call that nobody automates. The AI identified the exact question that determines whether this claim is paid or denied. And it tells the adjuster what evidence will resolve the question." |
| **5. SOP-driven investigation** | Investigation checklist generated: (1) Request plumber's inspection report, (2) Check maintenance records, (3) Assess damage pattern (sudden vs gradual indicators), (4) Check for prior water claims at this property, (5) Schedule field inspection if needed. Each item labeled: "Per [Carrier Name] SOP Section 4.3 -- Water Damage Investigation." | "Every carrier has different SOPs for how to investigate a water damage claim. Mysa follows YOUR procedures -- not generic best practices. This checklist comes from your SOP, not ours." |
| **6a. Decision: COVERED** | After plumber confirms sudden burst: Coverage card turns green: "Coverage APPLIES under Section I, Coverage A. Cause: sudden accidental discharge (burst pipe). Deductible: $1,000." Reserve card: "Median similar claims in this ZIP code: $8,400. Recommended reserve: $9,200 (accounts for hidden damage probability of 73% for water claims). 90% CI: $7,100-$12,400." | "The 6 sub-steps, with reasoning. Coverage confirmed with cited clause. Reserve calculated from 312 comparable claims. The 73% hidden damage probability adjusts the reserve upward -- because the system knows from history that water damage claims almost always have supplements." |
| **7. Document generation** | Three documents generated: (1) Coverage determination letter to policyholder, (2) Reserve memo for file, (3) Investigation summary with plumber's findings. All formatted per carrier template. | "Every document your SOP requires, auto-generated. The adjuster reviews and sends. No typing, no template hunting, no manual letter drafting." |
| **6b. The "what-if" (denial path)** | SWITCH SCENARIO: Evidence now shows gradual seepage. Coverage card turns red: "Exclusion 2.c APPLIES. Damage caused by continuous seepage over estimated 30+ days based on damage pattern analysis. Recommend DENIAL." Denial letter auto-generated: cites policy language, references evidence, includes appeal rights. | "Same product, opposite outcome. The AI adapts to evidence -- it doesn't have a bias toward approval or denial. When the evidence changes, the recommendation changes. And the denial letter cites the exact policy language. This is defensible in court." |

**What makes this demo impressive:**
- **Coverage determination:** Nobody else automates "sudden vs gradual" -- the hardest judgment call in property claims
- **SOP compliance:** Workflows come from the carrier's own procedures, not generic templates
- **The what-if:** Showing the AI can reason in both directions proves it is not biased
- **Documents:** Denial letter with correct policy language citations is gold for compliance teams
- **Human-in-the-loop:** The adjuster always decides. The AI provides the analysis.

[SOURCE: mysa_product_strategy.md, Part 8 -- Demo 2]

---

### Demo 3: Historical Data Flywheel (If Time Permits)

**Scenario:** After processing 100+ water damage claims, show how the system improves.

**What shows on screen:**
- Dashboard: "Water damage claims processed: 147. Recommendation accuracy: 89%. Average adjuster modification rate: 11%."
- For a new water damage claim: "87% of similar claims in your region with this damage pattern were covered. Average settlement: $9,100. Recommend expedited processing -- confidence: HIGH."
- Time-series chart: recommendation accuracy improving from 60% (Month 1) to 89% (Month 6).

**What to highlight:** "This is the flywheel. Every claim your adjusters process makes the system smarter. After 147 water damage claims, the system predicts outcomes with 89% accuracy. The adjusters who modify recommendations are teaching the model your carrier's specific decision patterns. Nobody else has this data."

[SOURCE: mysa_product_strategy.md, Part 8 -- Demo 3]

---

### Demo Requirements Summary

**Must show (non-negotiable):**
1. OCR accuracy on real documents (EAS forms, policies, emails)
2. SOP --> workflow generation (upload SOP, see structured workflow)
3. The 6 decision sub-steps with AI recommendations + confidence scores
4. Human-in-the-loop (adjuster reviews, adjusts, approves)
5. Document generation per decision
6. Before/after time comparison (manual vs Mysa)

**Should NOT try to show:**
- Full CMS replacement (Mysa is not a CMS)
- Real-time call recording (complex, save for v2)
- Xactimate/Audatex integration (US/EU estimation tools -- complex, save for Phase 4)
- Multi-user workflow (single-adjuster view is enough for demo)
- Historical data flywheel (only if time permits)

**Technical build requirements for demo:**
1. EAS OCR pipeline (use Caravela engine)
2. Convention matching rules engine (CIMPAS for Portugal, at minimum)
3. Policy document parser (Gemini for initial demo)
4. SOP upload --> workflow UI
5. Adjuster dashboard with 6 decision sub-step cards
6. Document generation templates (coverage letter, denial letter, reserve memo, settlement letter)
7. Before/after comparison screen

[SOURCE: mysa_product_strategy.md, Part 8]

---

## 6.10 Demo Spec: Broker Flow

### The Broker Problem

Brokers are the front door for many claims. In many EU markets, the broker is the first person the policyholder calls after an accident. The broker then creates the claim and submits it to the carrier. Today, this process is manual, email-heavy, and full of back-and-forth.

**Current broker workflow:**
```
1. Policyholder calls broker: "I had an accident"
2. Broker asks questions, takes notes (often incomplete)
3. Broker emails carrier with claim info + attachments
4. Carrier opens FNOL, finds missing information
5. Carrier emails broker asking for missing data
6. Broker calls policyholder to get missing data
7. Policyholder provides (partially)
8. Broker emails carrier again
9. Repeat steps 5-8 until carrier has enough to open claim
```

**Average cycles of back-and-forth:** 2-4
**Time wasted per claim:** 30-60 minutes across broker + carrier

[SOURCE: meeting_notes_2026-02-09_claims_workflow.md; TRANSCRIPT: Feb 9, 2026]

### The Mysa Broker Flow

Three components deliver value to brokers:

#### Component 1: White-Labeled FNOL Forms

Carrier-branded intake forms that brokers send to policyholders. The forms are smart -- they adapt based on claim type, ask only relevant questions, and validate completeness before submission.

| Feature | What It Does | Why It Matters |
|---------|-------------|----------------|
| **Dynamic fields** | Form shows/hides fields based on claim type (auto, property, liability) and answers to prior questions | No more generic forms that ask irrelevant questions |
| **Carrier-specific** | Each carrier configures their required fields per claim type | Compliance with carrier's intake requirements |
| **Completeness validation** | Form will not submit until all required fields are filled. Missing fields are highlighted. | Eliminates the back-and-forth cycle |
| **Photo upload** | Policyholder can take photos directly from phone and upload | Photos arrive structured, not scattered across emails |
| **GDPR-compliant** | Consent checkboxes, data processing notices, booking links for phone calls when written consent is required | Regulatory compliance built in |
| **White-labeled** | Form carries the broker's or carrier's brand, not Mysa's | Broker maintains client relationship |

**Demo flow:**
1. Broker receives call from policyholder
2. Broker sends white-labeled FNOL link via SMS/email
3. Policyholder fills out form on phone: accident details, photos, counterparty info
4. Form validates: all required fields present
5. Claim arrives at carrier fully structured, complete, ready for triage
6. Zero back-and-forth

#### Component 2: Chrome Extension on Email

This is the broker equivalent of the adjuster Clippy. The broker works primarily in email. The Chrome extension sits on top of Gmail/Outlook web and enables one-click claim creation.

**How it works:**
1. Broker receives email from policyholder describing accident
2. Broker selects relevant text in email (the accident narrative, dates, parties)
3. Right-clicks: "Create Claim with Mysa"
4. Extension extracts structured data from selected text: date of loss, parties, damage description, policy number (if mentioned)
5. Pre-fills FNOL form with extracted data
6. Highlights missing fields: "Policy number: found. Date of loss: found. Counterparty info: MISSING."
7. Broker completes missing fields or sends gap analysis to policyholder
8. Claim submitted to carrier

**What to highlight in demo:** "The broker creates a claim from an email in 2 clicks. No re-typing. No switching to the carrier's portal. No calling the policyholder back to ask for information they already provided. The AI extracts what's there and flags what's missing."

[SOURCE: meeting_notes_2026-02-09_claims_workflow.md -- "Email-based claim creation with Chrome extension (like Superhuman)"]

#### Component 3: AI Gap Analysis

Once the broker submits a claim, Mysa's gap analysis runs automatically:

1. Cross-references submitted data against carrier's required fields for this claim type
2. Identifies missing information
3. Auto-generates a follow-up message to the policyholder (via broker) requesting specific missing items
4. Tracks which items are outstanding
5. Alerts broker when all required information has been received

**The value proposition for brokers:** "Submit once. We tell you if anything is missing before the carrier rejects it. No more 3-4 round trips."

### Broker Demo Flow (Full Walkthrough)

| Step | Screen | Action | Talking Point |
|------|--------|--------|---------------|
| 1 | Gmail inbox | Broker opens email from policyholder: "Had an accident on Rua Augusta. Photos attached." | "This is what brokers deal with every day -- unstructured emails with partial information." |
| 2 | Gmail + Mysa extension | Broker selects email text, right-clicks "Create Claim with Mysa." | "Two clicks. That's it. No portal login, no re-typing." |
| 3 | Claim creation overlay | Pre-filled form: date, location, narrative extracted. Orange flags: "Counterparty name: MISSING. Policy number: FOUND. Damage photos: 3 ATTACHED." | "AI extracted what was there and flagged what was not. The broker knows exactly what to ask for." |
| 4 | Gap analysis view | Broker clicks "Send Gap Analysis." Auto-drafted message to policyholder: "Para completar o seu sinistro, necessitamos: nome do outro condutor." | "One click sends a professionally formatted request in the policyholder's language." |
| 5 | Carrier portal | Carrier receives fully structured claim. All fields populated. Documents attached. Ready for triage. | "The carrier gets a clean claim. No garbage in. The STP potential just went up because the data quality is right." |

[SOURCE: meeting_notes_2026-02-09_claims_workflow.md; TRANSCRIPT: Feb 9, 2026]

---

## 6.11 Demo Data & Workflow Specs

### Realistic Claim Data Examples

The demo must pass the "pro test" -- an experienced claims professional should watch the demo and think "yes, that's how it actually works." This requires realistic data, realistic workflows, and realistic decision trees.

---

### Example 1: EU Motor -- Portuguese Convention Claim

**Claim data:**

| Field | Value | Source |
|-------|-------|--------|
| **Claim ID** | AUTO-2026-04812 | System-generated |
| **Date of loss** | February 7, 2026, 08:45 | EAS form, Box 1 |
| **Location** | Rua Augusta, Lisbon, Portugal | EAS form, Box 2 |
| **Party A (Insured)** | Maria Santos, Policy #CAR-PT-2024-08891, Caravela Seguros | EAS form, Box 6 |
| **Vehicle A** | 2021 Volkswagen Golf, AA-12-BB | EAS form, Box 7 |
| **Party B (Counterparty)** | Joao Ferreira, Policy #FID-PT-2023-12045, Fidelidade | EAS form, Box 9 |
| **Vehicle B** | 2019 Renault Clio, CC-34-DD | EAS form, Box 10 |
| **Circumstances** | Party A was reversing out of parking space. Party B was stationary in traffic lane. Contact: rear of Vehicle A to front-left of Vehicle B. | EAS form, diagram + checkboxes |
| **EAS Checkboxes** | Party A: Box 2 (leaving parking), Box 4 (reversing), Box 14 (hitting rear). Party B: Box 1 (parked/stopped). | EAS form, Section 12 |
| **Injuries** | None reported | EAS form, Box 3 |
| **Police report** | Not filed (no injuries, both parties agreed on EAS) | EAS form, Box 4 |
| **Damage A** | Rear bumper, rear-left quarter panel. Photos: 3 attached. | EAS form + email attachments |
| **Damage B** | Front-left bumper, headlight housing cracked. Photos: 2 attached. | EAS form + email attachments |

**Convention matching:**

| Rule | Application |
|------|-------------|
| **Convention system** | IDS/CIMPAS (Portugal) |
| **Matched case** | Case 7 -- Vehicle reversing collides with stationary/moving vehicle |
| **Fault allocation** | 100% Party A (reversing vehicle) |
| **Confidence** | 95% (checkbox pattern is unambiguous) |
| **Deterministic?** | Yes -- no adjuster judgment required for fault |

**6 Decision Sub-Steps for this claim:**

| Sub-Step | AI Recommendation | Confidence | Evidence |
|----------|-------------------|------------|----------|
| 1. Coverage | COVERED. Policy CAR-PT-2024-08891 active. Vehicle matches. Driver listed. No exclusions apply. | 98% | Policy document parsed. Premium paid through Feb 2026. |
| 2. Report check | COMPLETE with 1 exception: counterparty policy number was initially missing (resolved via auto-outreach). All other fields present and consistent. | 95% | Cross-reference: EAS date matches email date. Damage description matches photos. Location consistent. |
| 3. Repair assessment | Estimate from DRP body shop: EUR 2,400. Rear bumper replacement EUR 980, quarter panel repair EUR 720, paint EUR 450, labor EUR 250. All within guidelines. | 92% | Compared to 847 similar claims in Lisbon region. Estimate at 58th percentile. No anomalies. |
| 4. Cost analysis | Total claim cost: EUR 2,400 (repair) + EUR 180 (towing) = EUR 2,580. Within expected range for this damage type. | 94% | Historical range for similar claims: EUR 1,800-EUR 3,600 |
| 5. Reserve | Recommended: EUR 3,100 (includes 20% buffer for supplements -- historical supplement rate for this body shop: 65%). 90% CI: EUR 2,400-EUR 4,200. Within desk adjuster authority (EUR 5,000). | 90% | Based on 847 comparable claims. Body shop supplement history factored in. |
| 6. Fraud | Score: 8/100 (LOW). No indicators flagged. First claim for this policyholder in 3 years. No network connections to flagged entities. | 99% | ISO ClaimSearch: no prior claims. Internal history: clean. |

**Authority levels (Caravela example):**

| Level | Authority Limit | Who |
|-------|----------------|-----|
| Desk adjuster | EUR 5,000 | Any desk adjuster |
| Senior adjuster | EUR 15,000 | Adjusters with 3+ years |
| Supervisor | EUR 50,000 | Claims team lead |
| VP Claims | EUR 200,000 | Department head |
| Board | Unlimited | For catastrophe or exceptional claims |

This claim (EUR 3,100 reserve) falls within desk adjuster authority. No escalation required.

---

### Example 2: US Property -- Water Damage Claim

**Claim data:**

| Field | Value | Source |
|-------|-------|--------|
| **Claim ID** | PROP-2026-11847 | System-generated |
| **Date of loss** | February 3, 2026 (discovered February 5 upon return from vacation) | FNOL email |
| **Location** | 4218 Maple Drive, Plano, TX 75024 | FNOL email |
| **Policyholder** | James and Sarah Mitchell, Policy #HO3-TX-2023-44219 | Policy lookup |
| **Policy type** | HO-3 Special Form (most common US homeowners policy -- covers dwelling on an open-peril basis, personal property on a named-peril basis) | Policy document |
| **Coverage A (Dwelling)** | $425,000 limit | Policy declarations |
| **Deductible** | $1,000 | Policy declarations |
| **Loss description** | "Water in basement. 3-4 inches standing water. Drywall buckling. Furniture damaged. Mold visible on lower walls." | FNOL email narrative |
| **Photos** | 6 photos: standing water, damaged drywall, wet furniture, mold on wall, utility room (pipe visible), water line on wall | Email attachments |
| **Prior claims** | 1 wind/hail claim in 2022 (resolved, $3,200) | Internal history |
| **Cause** | Unknown at FNOL. Investigation required to determine sudden burst vs gradual seepage. | Adjuster determination needed |

**Decision tree for this claim:**

```
WATER DAMAGE CLAIM RECEIVED
  |
  v
COVERAGE CHECK #1: Policy active?
  |-- YES: Policy active, premiums current through March 2026
  |
  v
COVERAGE CHECK #2: Is this a covered peril?
  |
  +-- HO-3 Section I: Covers "sudden and accidental discharge of water"
  +-- HO-3 Exclusion 2.c: Excludes "water damage from continuous or repeated
  |   seepage or leakage over a period of 14 or more days"
  |
  v
INVESTIGATION REQUIRED: Sudden or gradual?
  |
  +-- Request plumber's inspection report
  +-- Check maintenance records (when was plumbing last serviced?)
  +-- Analyze damage pattern:
  |     - Mold present = suggests prolonged exposure (days-weeks)
  |     - Water line height on wall = indicates duration
  |     - Pipe condition (corrosion suggests gradual; clean break suggests sudden)
  +-- Check for prior water damage claims at this property
  |
  v
PLUMBER'S REPORT RECEIVED
  |
  +-- FINDING A: "Copper supply line failed at solder joint.
  |   Clean break. No evidence of prior seepage or corrosion.
  |   Failure is consistent with sudden pressure event."
  |   |
  |   v
  |   COVERAGE: APPLIES
  |   Cite: Section I, Coverage A, "sudden and accidental discharge"
  |   Mold presence explained by: loss occurred Feb 3, discovered Feb 5
  |   (48 hours of standing water = mold growth is expected and does not
  |   indicate pre-existing condition)
  |   |
  |   v
  |   RESERVE: $9,200
  |   - Water extraction: $1,800
  |   - Drywall repair: $3,200
  |   - Mold remediation: $2,400
  |   - Furniture replacement: $1,800
  |   Based on 312 comparable water damage claims in DFW metro
  |
  +-- FINDING B (alternative): "Copper supply line shows significant
      corrosion and mineral deposits. Pinhole leak pattern consistent
      with gradual deterioration. Estimated seepage duration: 30+ days."
      |
      v
      COVERAGE: EXCLUDED
      Cite: Exclusion 2.c, "continuous or repeated seepage over 14+ days"
      |
      v
      DENIAL LETTER generated with:
      - Specific policy clause citation
      - Evidence summary (plumber's report findings)
      - Appeal rights per Texas DOI regulations
      - 30-day response timeline per TX Insurance Code 542.056
```

**Texas-specific regulatory requirements:**

| Requirement | Regulation | Mysa Implementation |
|-------------|-----------|---------------------|
| Acknowledge claim within 15 days | TX Ins. Code 542.055 | Auto-generated acknowledgment letter at FNOL |
| Accept or reject within 15 business days of receiving all info | TX Ins. Code 542.056 | Diary date set automatically. Alert if approaching deadline. |
| Pay within 5 business days of acceptance | TX Ins. Code 542.057 | Payment authorization workflow triggered on acceptance |
| 18% penalty interest on late payments | TX Ins. Code 542.060 | System flags if payment deadline is approaching |

---

### Triage Decision Logic (From Discovery Phases 6-8)

The following triage decision tree should be encoded as the default standard workflow, customizable per carrier SOP:

```
CLAIM ARRIVES AT TRIAGE
  |
  v
CHECK 1: Is this a catastrophe event?
  |-- YES -> Route to CAT team (surge protocols, field deployment)
  |-- NO  -> Continue
  |
  v
CHECK 2: Are there injuries or fatalities?
  |-- FATALITY -> Route to major loss unit + legal
  |-- SEVERE INJURY -> Route to BI specialist, HIGH priority
  |-- MINOR INJURY -> Flag for BI follow-up, continue PD processing
  |-- NO INJURIES -> Continue
  |
  v
CHECK 3: Fraud score?
  |-- HIGH (>70) -> Route to SIU for investigation before proceeding
  |-- MEDIUM (30-70) -> Flag for enhanced investigation, continue with adjuster
  |-- LOW (<30) -> Clear, continue
  |
  v
CHECK 4: Estimated claim cost vs vehicle/property value?
  |-- >70-80% of ACV (auto) -> Flag as POTENTIAL TOTAL LOSS, stop STP
  |-- >50% of dwelling limit (property) -> Route to major loss
  |-- Within normal range -> Continue
  |
  v
CHECK 5: Coverage issues?
  |-- Coverage clear -> Continue
  |-- Coverage ambiguous -> Flag for coverage investigation, issue RESERVE OF RIGHTS letter
  |-- Coverage excluded -> Route to denial workflow with letter
  |
  v
CHECK 6: Claim complexity score?
  |-- LOW (routine, single party, clear fault, within STP parameters)
  |     -> STP candidate: auto-process through decision engine, minimal review
  |-- MEDIUM (some ambiguity, multiple parties, moderate value)
  |     -> Desk adjuster: full 6 sub-step workflow
  |-- HIGH (disputed liability, attorney involved, large loss, multi-party)
  |     -> Senior adjuster or supervisor: enhanced investigation + full workflow
  |-- CRITICAL (litigation, regulatory inquiry, media attention)
  |     -> Major loss unit + legal + management notification
  |
  v
ASSIGNMENT
  Route to: [desk adjuster / field adjuster / BI specialist / SIU / total loss desk / CAT team / major loss unit]
  Priority: [URGENT / HIGH / STANDARD / LOW]
  Investigation plan: [generated from SOP per claim type and complexity]
  Diary dates: [set per SOP requirements and regulatory deadlines]
```

[SOURCE: claims_journey_discovery.md, Phase 6 -- Triage; meeting_notes_2026-02-09_claims_workflow.md]

### Investigation Activities Reference (Phase 7)

For the demo to pass the pro test, investigation workflows must include these 13 activities identified from the discovery document, each with realistic time estimates:

| # | Activity | Time per Instance | EU | US | Mysa Automation |
|---|----------|-------------------|----|----|-----------------|
| 1 | Take recorded statements | 15-30 min per party (x2-4 parties) | Rare for routine PD (EAS serves as statement) | Near-universal | Call recording + transcription + auto-extraction of key facts |
| 2 | Review police report | 10-20 min | ~20-30% of claims | ~60-70% | Auto-retrieval (LexisNexis), parsing, key fact extraction |
| 3 | Analyze scene photos/video | 10-30 min | Review policyholder photos, compare to EAS | Both parties + dashcam | AI photo analysis: damage classification, consistency check |
| 4 | Match to convention scenario (EU) | 5-10 min | Core activity, ~40% need judgment | N/A | Convention matching engine (deterministic for clear cases) |
| 5 | Determine liability | 15-60 min | Non-convention cases | All claims | AI liability recommendation with evidence chain |
| 6 | Coverage analysis | 10-30 min | Edge cases | More complex (state rules) | Policy parsing + SOP-driven coverage determination |
| 7 | Contact witnesses | 10-20 min per witness | Rare for routine PD | Common for disputed liability | Auto-drafted outreach, contact tracking |
| 8 | Order/review medical records (BI) | 30-60 min per review | For BI claims | Extensive (50-500+ pages) | Medical record parsing, treatment timeline extraction |
| 9 | Coordinate with legal | 15-30 min per interaction | If attorney involved | ~40% of BI claims | Legal correspondence tracking, deadline management |
| 10 | Cross-reference databases | 5-10 min | Internal history | ISO, NICB, LexisNexis | Automated database checks, result aggregation |
| 11 | Request additional evidence | 5-15 min per request | Yes | Yes | Auto-drafted requests, outstanding item tracking |
| 12 | Document everything | 3-5 min per entry (ongoing) | Yes | Yes | Auto-documentation from adjuster actions in system |
| 13 | Supervisor review / escalation | 10-20 min | If reserve exceeds authority | If complex | Auto-generated escalation package with full context |

[SOURCE: claims_journey_discovery.md, Phase 7 -- Investigation, lines 1747-1763]

### Assessment Activities Reference (Phase 8)

| # | Activity | Time | Mysa Automation |
|---|----------|------|-----------------|
| 1 | Review repair estimate | 15-30 min | Auto-ingest from CCC/Mitchell/Audatex. Flag anomalies vs carrier guidelines and comparables. |
| 2 | Negotiate estimate with body shop | 15-30 min per supplement | Generate negotiation points from anomaly analysis. Track supplement cycle. |
| 3 | Determine repair vs total loss | 10-20 min | Auto-calculate repair cost vs ACV. Apply state/country-specific threshold. Flag total loss candidates. |
| 4 | ACV valuation (total loss) | 20-40 min | Pull comparables from CCC Valuescope / market data. Generate ACV report. |
| 5 | Review medical bills (BI) | 30-60 min per review | Parse medical bills. Flag outlier charges. Compare to UCR (usual, customary, reasonable) rates. |
| 6 | Calculate BI damages | 30-120 min | Multiplier method or per diem method. Historical comparable injuries. Colossus integration where available. |
| 7 | Evaluate property damage (non-auto) | 30-60 min | Xactimate integration (US). Scope of loss analysis. |
| 8 | Set/adjust reserves | 10-20 min | Statistical reserve calculation with confidence interval and P&L impact memo. |
| 9 | Review vendor invoices | 10-15 min per invoice | Parse invoices. Cross-reference against approved rates and SOP limits. |
| 10 | Prepare assessment summary | 15-30 min | Auto-generate from all assessment data. Format per carrier template. |
| 11 | Quality review (supervisor) | 10-20 min | Dashboard: assessment variance from comparables. SOP compliance score. |
| 12 | Subrogation potential evaluation | 5-10 min | Auto-flag if third-party liability established. Calculate recovery amount. |

[SOURCE: claims_journey_discovery.md, Phase 8 -- Assessment, lines 1836-1851]

### Settlement Activities Reference (Phases 9-10)

| # | Activity | EU Convention | US Adversarial | Mysa Automation |
|---|----------|---------------|----------------|-----------------|
| 1 | Calculate settlement amount | Repair cost minus deductible. Convention forfait for inter-insurer. | Repair cost minus deductible, depreciation, betterment. BI: medical x multiplier. | Auto-calculation per formula + carrier rules. |
| 2 | Generate settlement offer | Letter per carrier template. Regulatory timeline (e.g., Italy: 30/60 days to offer). | Letter per carrier template. State-specific timeline (e.g., TX: 15 business days). | Auto-generated with regulatory deadline tracking. |
| 3 | Authority check | Within adjuster limit? If not, escalate. | Within adjuster limit? If not, escalate. Committee for large losses. | Auto-check against authority matrix. Escalation package auto-generated. |
| 4 | Policyholder communication | Email/post per carrier preference. | Email/post. Attorney communication if represented. | Channel-appropriate communication. Attorney flag for legal compliance. |
| 5 | Negotiation (if disputed) | Limited for PD (convention amounts are standard). BI may negotiate. | Common. Initial offers typically 30-50% below final. Multiple rounds. | Negotiation range recommendation. Authority tracking through rounds. |
| 6 | Payment processing | SEPA transfer (EUR). Convention clearing house for inter-insurer. | ACH/EFT, check, wire. Dual-payee for financed vehicles. | Payment authorization workflow. Regulatory deadline alerts. |
| 7 | Supplement handling | Re-estimation if hidden damage found during repair (50-90% of claims). | Same. Average 1.3 supplements per claim. | Supplement intake, re-assessment, reserve adjustment, additional payment authorization. |
| 8 | Subrogation initiation | Convention clearing house handles inter-insurer recovery. | Demand letter to at-fault party's insurer. Arbitration Forums if disputed. | Auto-generate subrogation demand. Track recovery. |
| 9 | Document settlement | Release form. Settlement recorded. File notes. | Release form. 1099 for BI > $600. Medicare Set-Aside if applicable. | Auto-generate release. Track tax reporting requirements. |
| 10 | Close file | Reserve adjusted to match payment. SOP closure checklist. | Same. Escheatment rules for uncashed checks. | Closure checklist per SOP. Reserve-to-payment reconciliation. Training data captured. |

[SOURCE: claims_journey_discovery.md, Phases 9-10 -- Decision and Settlement]

### Convention System Quick Reference

For EU motor demo scenarios, the following convention data must be encoded:

| Country | Convention | System | How Fault Is Determined | Settlement Mechanism | Timeline |
|---------|-----------|--------|------------------------|---------------------|----------|
| **Portugal** | IDS/CIMPAS | Digital platform (CIMPAS) | Checkbox pattern on EAS mapped to numbered cases. Deterministic for clear matches. | Direct settlement: each insurer pays own policyholder. Inter-insurer reimbursement at forfait through clearing house. | ~1.94 days average decision time. 91% inter-insurer agreement rate. |
| **Spain** | CIDE/ASCIDE | CICOS digital platform | Tabla de Culpabilidad (fault table) + CICOS processing. | Direct settlement + CICOS clearing house. | Covers 70-83% of motor claims. 2.5M claims/year via CICOS. |
| **France** | IRSA | Paper/digital | 13 standardized cases. Outputs ONLY 0%, 50%, or 100% fault. Simplest model in EU. | Direct settlement + inter-insurer clearing. | Deterministic (instant lookup for clear cases). ~80% of material motor claims. 7.4M claims/year total. |
| **Italy** | CARD | CONSAP clearing house | Mandatory for 2-vehicle claims with <9% permanent disability. Civil code + CAI form. | Direct settlement + CONSAP Stanza di Compensazione. | 30 days with signed EAS to offer, 60 days without. 15 days to pay after acceptance. ~2M claims paid/year. |

[SOURCE: mysa_product_strategy.md, Part 6b -- Convention Systems by Country]

### Authority Matrix Template

Every carrier defines authority levels differently. The demo should use this realistic template that can be customized per carrier during onboarding:

| Decision Type | Level 1: Desk Adjuster | Level 2: Senior Adjuster | Level 3: Supervisor | Level 4: VP Claims | Level 5: Board/Committee |
|---------------|----------------------|------------------------|--------------------|--------------------|-------------------------|
| **Reserve setting** | Up to EUR 5,000 / $10,000 | Up to EUR 15,000 / $25,000 | Up to EUR 50,000 / $100,000 | Up to EUR 200,000 / $500,000 | Unlimited |
| **Settlement authority** | Up to EUR 3,000 / $7,500 | Up to EUR 10,000 / $20,000 | Up to EUR 35,000 / $75,000 | Up to EUR 150,000 / $350,000 | Unlimited |
| **Denial authority** | Routine denials (policy lapsed, excluded driver) | Coverage denials with investigation | Complex denials, BI denials | Denials with litigation risk | Denials with regulatory/media risk |
| **SIU referral** | Can flag, cannot refer | Can refer with supervisor approval | Can refer directly | Oversight | Policy decisions |
| **Total loss declaration** | Can flag, cannot declare | Can declare up to EUR 15,000 ACV | Can declare up to EUR 50,000 ACV | All total losses | N/A |

**System behavior:** At each decision point, Mysa checks the recommended action against the logged-in adjuster's authority level. If the action exceeds authority, the system:
1. Blocks the action (adjuster cannot approve)
2. Generates an escalation package with full decision rationale, evidence, and recommendation
3. Routes to the next authority level
4. Tracks time in escalation queue (bottleneck visibility for supervisor dashboard)

[SOURCE: claims_journey_discovery.md, Phase 6 -- Triage authority levels; meeting_notes_2026-02-09_claims_workflow.md -- authority limits]

---

## Sources

| Source | Type | Sections Used |
|--------|------|--------------|
| `mysa_product_strategy.md` Parts 1, 5a-5d, 8 | Primary -- product flow, decision sub-steps, agent architecture, demo specs | 6.1-6.4, 6.8, 6.9, 6.11 |
| `meeting_notes_2026-02-09_claims_workflow.md` | Transcript summary -- Clippy, Vault, Chrome extension, broker flow, triage logic | 6.3, 6.5, 6.10, 6.11 |
| `claims_journey_discovery.md` Phases 6-8 | Discovery -- Triage, Investigation, Assessment activities, competitor solutions, handoff points | 6.6, 6.7, 6.11 |
| `claims_journey_discovery.md` Phases 9-10 | Discovery -- Decision, Settlement activities, EU vs US differences, convention bodies | 6.7, 6.11 |
| `MODULE_01_POSITIONING.md` | Prior FOS module -- positioning context, persona table, Product Now vs Tomorrow | 6.1, 6.5, 6.6 |
| `MODULE_07_TECHNICAL.md` Section 7.7 | Prior FOS module -- Chrome extension architecture, Vault, limitations | 6.5 |
| Feb 7, 2026 Granola call | Transcript -- product flow quotes, demo strategy, SOP discussion, reserve importance | 6.1-6.4, 6.8, 6.9 |
| Feb 9, 2026 Granola call | Transcript -- Clippy/Superhuman architecture, broker flow, triage decision logic, EU vs US | 6.3, 6.5, 6.6, 6.10 |
| `REGULATORY_COMPLIANCE.md` | Secondary -- EU AI Act, GDPR Article 22, US state regulations | 6.8 |

---

# Part 7: Technical Architecture

# Module 7: Technical Architecture

**Status:** DRAFT v1.0
**Last updated:** February 9, 2026
**Feeds:** Technical due diligence, CTO/engineering hiring brief, partner integration conversations, investor appendix

---

## 7.1 Architecture Philosophy

### Agent-Native: Why This Is Not a Feature Choice

Mysa is built agent-native. This is not a marketing label or a design preference — it is a structural decision that determines what the product can and cannot do at scale.

The distinction matters because insurance claims are governed by rules that are:
- **Carrier-specific** — each insurer has different SOPs, authority levels, and escalation paths
- **Country-specific** — convention systems differ by jurisdiction (IDS in Portugal, IRSA in France, CARD in Italy, CIDE in Spain)
- **Constantly changing** — insurer enforcement patterns shift, regulations update, contracts renew
- **Combinatorially explosive** — 10+ insurers multiplied by 1,000s of procedures multiplied by per-carrier workflow variations

Traditional software encodes business rules as code. Every new rule is an `if/else` branch. Every new insurer is a development sprint. Every rule change requires a code deployment. A large Portuguese healthcare group with 40+ clinics and $100M in revenue "spent millions building a submission tool. They're still on spreadsheets." [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Appendix D — "The Spreadsheet Evidence"]

**"Features are prompts, not code."** [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 1]

In Mysa's architecture, business rules live as knowledge, not code. An agent orchestrator understands intent, retrieves relevant knowledge, composes atomic tool calls, and validates output. The same tools work across every carrier — only the knowledge differs.

| Characteristic | Traditional Software | Agent-Native (Mysa) |
|----------------|---------------------|---------------------|
| Rules storage | Hardcoded in application logic | Knowledge base (structured + unstructured) |
| New insurer / carrier | Development sprint (weeks) | Knowledge ingestion (hours to days) |
| Rule change | Code deployment | Knowledge update |
| Cross-insurer logic | Separate codepaths per insurer | Same tools, different knowledge |
| Feature addition | Engineering cycle | Prompt engineering + tool composition |
| User customization | Configuration UI | Natural language + SOP upload |

[SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 2 — Architecture Comparison]

### Why "Add AI to Existing Software" Fails

Incumbents cannot replicate this by bolting AI onto their existing architecture:

| Incumbent Approach | Why It Fails |
|-------------------|--------------|
| Add chatbot to existing UI | AI cannot reason about hardcoded rules — it can only surface them |
| Use AI for document OCR only | Extraction without understanding. Reads the form but does not know what to do with it |
| ML for denial/fraud prediction | Predicts outcomes but cannot prevent issues or recommend fixes |
| Fine-tune on claims data | Model sits outside the workflow, not inside the decision |

The fundamental problem: their architecture assumes rules are CODE. Adding AI does not change that. The AI becomes a feature layered on top of a rigid system, not the foundation that the system is built from. [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8.1]

### The Atomic Tools Principle

Tools in Mysa are more granular than features. A single feature (like "check this pre-auth before I submit") is composed from multiple atomic tool calls: field validation, code validation, risk scoring, issue identification, and fix suggestion — each one a discrete, reusable unit. The agent decides which tools to call, in which order, with which knowledge context. [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 4]

This means the tool set scales sublinearly with product scope. Adding a new carrier or a new country requires new knowledge, not new tools.

---

## 7.2 Current Stack

### What Exists Today: The Caravela Pilot

The current production system is a document processing engine built for a single Portuguese motor insurance carrier (Caravela, ~EUR 188M GWP, 57K claims/year). It proves the foundational capability — reading insurance documents with AI, structuring the data, and matching it against convention rules. It is the starting point, not the end state.

| Component | Technology | Detail |
|-----------|-----------|--------|
| **Frontend** | Next.js (React) | App at app.mysa-health.com. Caravela demo at caravela.mysa-health.com |
| **LLM backbone** | Gemini 3 Flash Preview | Google's latest multimodal model. Selected for vision + OCR capability and cost efficiency |
| **Database** | Supabase (PostgreSQL) | Hosted PostgreSQL with Row Level Security. Stores training claims, extraction results, ground truth |
| **Hosting** | Vercel | Auto-deploy from Git branches. Separate projects for marketing site and app |
| **OCR pipeline** | Custom (Caravela engine) | Multi-page image processing, section cropping, x3 voting, GOLDEN RULES normalization |
| **Benchmark system** | benchmark-with-db.ts | Tracks accuracy across models, stores results in Supabase. 44 claims with ground truth |

[SOURCE: MODULE_01_POSITIONING.md, Section 1.6 — "Product Now"; caravela-ocr.md (memory file); mysa_product_strategy.md, Part 5c]

### Key Metrics

- **81.5% normalized field-level accuracy** on Portuguese motor claims (EAS/DAAA forms) — handwritten + printed, with Portuguese diacritics [SOURCE: caravela-ocr.md (memory file) — "81.5% — TARGET HIT (Feb 8)"]
- **44 claims** with validated ground truth data in `training_claims` table [SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md, Section 7]
- **x3 self-consistency voting** — each extraction runs 3 times, majority vote selects the answer. Deployed in production. [SOURCE: FIELD-INVESTIGATION-LOG.md — "+1% deployed"]
- **GOLDEN RULES** — anti-hallucination prompt directives that enforce column discipline, page discipline, and output constraints. Deployed in production. [SOURCE: BENCHMARK-AUDIT-FINDINGS.md — "Lines 8-91: GOLDEN RULES"]
- **70+ normalization rules** — post-extraction matching for dates, addresses, Portuguese names, license plates [SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md, Section 6]

### What This Proves

The Caravela pilot validates that a small team (two founders) can build a production-grade document AI pipeline in 8 weeks using off-the-shelf LLMs, with accuracy competitive with Google Document AI (82%) and above Amazon Textract (78%) — on a harder problem (handwriting + Portuguese diacritics + unstructured forms). [SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md, Section 1]

### What This Does Not Do Yet

Coverage determination, reserve calculation, fraud detection, investigation support, SOP-driven workflow generation, multi-carrier support, property claims, US market support, broker flow. The current system reads documents and matches conventions. The product vision is an end-to-end decision engine.

---

## 7.3 Production Stack Vision

### Where This Needs to Go

The production system must support multiple carriers, each with isolated data, across EU and US jurisdictions, with EU data residency compliance and the ability to process tens of thousands of claims per month per carrier.

### Non-Negotiable Requirements

| Requirement | Rationale |
|-------------|-----------|
| **Multi-tenant, carrier-isolated** | Each carrier's SOPs, claims data, and decision patterns are confidential and must not leak across tenants |
| **EU-hosted data residency** | GDPR requires personal data stay within the EU. Claims data includes PII (names, addresses, policy numbers, injury details) |
| **Human-in-the-loop at every decision point** | GDPR Article 22 prohibits fully automated decisions with legal effect. EU AI Act classifies claims AI as high-risk. [SOURCE: mysa_product_strategy.md, Part 5d; REGULATORY_COMPLIANCE.md] |
| **Audit trail** | Every AI recommendation and every human decision must be logged for regulatory compliance and bad-faith defense |
| **REST API integration** | Must layer on top of existing CMS (Guidewire, Duck Creek, Sapiens, or proprietary) — not replace them [SOURCE: mysa_product_strategy.md, Part 5c] |

### Cloud Provider Decision [FOUNDER INPUT REQUIRED]

This is an open decision. The Caravela pilot runs on Vercel (frontend) + Supabase (database). The production system needs EU-region compute, GPU access for potential fine-tuned models, and carrier-grade security.

| Option | Pros | Cons | Cost Model |
|--------|------|------|------------|
| **Option A: Google Cloud (GCP europe-west)** | Native Vertex AI for Gemini fine-tuning. EU regions available. Existing Gemini relationship. | Vendor lock-in to Google ecosystem. Supabase would need migration to Cloud SQL or AlloyDB | Pay-per-use. Vertex AI fine-tuning has specific pricing |
| **Option B: AWS (eu-west-1 Ireland / eu-central-1 Frankfurt)** | Largest ecosystem. Broadest enterprise insurance market acceptance. Bedrock for multi-model. | No native Gemini — would need to use Gemini via API or switch to Claude/GPT. Less tight integration for fine-tuning | Reserved instances + pay-per-use |
| **Option C: Stay on Supabase + Vercel, add EU region** | Fastest to ship. Supabase has EU hosting. Vercel has EU edge. Lowest migration effort | Less enterprise credibility. Supabase may not meet carrier security audit requirements at scale. Limited GPU access | Subscription + usage |

**Recommendation for Jeremy:** Option A (GCP) is the path of least resistance given the existing Gemini stack and the fine-tuning roadmap (Vertex AI). Option C works for the next 6-12 months while revenue is pre-$1M. Option B becomes relevant if enterprise carriers require AWS certification.

[SOURCE: mysa_product_strategy.md, Part 5c — "EU-region (AWS eu-west / GCP europe-west)"; CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md, Section 7 — Vertex AI fine-tuning]

### Multi-Agent Architecture [FOUNDER INPUT REQUIRED]

The product strategy document proposes 8 specialized agents. The implementation question is whether the orchestrator should be a single LLM or multiple specialized models.

| Option | Description | Trade-off |
|--------|-------------|-----------|
| **Single orchestrator + specialized prompts** | One model (e.g., Gemini) handles all routing and tool composition. Each "agent" is a prompt template with access to specific tools | Simpler to build, easier to debug. Risk: model quality degrades as prompt complexity increases |
| **Multi-model with router** | A lightweight model routes to specialized models. OCR uses Gemini Flash, coverage analysis uses a larger model, fraud detection uses a pattern-matching model | Better accuracy per task. Higher complexity, higher latency, higher cost |
| **LangChain / LangGraph orchestration** | Use an agent framework to manage tool routing, state, and multi-step reasoning | Framework handles complexity. Risk: framework abstractions may not fit insurance domain well |

This does not need to be decided now. The Caravela pilot uses direct Gemini API calls. The first multi-agent implementation should be the simplest option that works (single orchestrator with specialized prompts) and evolve based on observed failures.

[SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 10 — Open Question Q1]

---

## 7.4 OCR & Document Processing

### Current Performance

The Caravela OCR engine processes Portuguese motor claims forms (EAS/DAAA — European Accident Statements). These are among the hardest documents for OCR: handwritten fields, Portuguese diacritics (a, e, c, o, u with accents and tildes), checkbox grids, hand-drawn diagrams, and variable form quality (some scanned, some photographed).

| Metric | Value | Context |
|--------|-------|---------|
| **Normalized field-level accuracy** | 81.5% | 44 claims, 2990+ fields total. Uses normalizedMatch() for comparison |
| **vs. Google Document AI** | Competitive (82% on invoices) | Google tested on printed invoices, not handwritten insurance forms |
| **vs. Amazon Textract** | Above (78% on invoices) | Same caveat — Textract tested on printed, not handwritten |
| **vs. Azure Document Intelligence** | Below (93% on invoices) | Azure uses template-based extraction which Caravela does not yet implement |
| **vs. Zonal OCR (template-based)** | Below (99% on structured forms) | Template matching is the accuracy ceiling for structured forms |

[SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md, Section 1]

### How It Works

```
DOCUMENT ARRIVES (scan, photo, or PDF)
  |
  v
PREPROCESSING
  | Section cropping (7 regions per EAS form)
  | Image quality assessment
  |
  v
EXTRACTION (x3 runs)
  | Each run: Gemini 3 Flash Preview processes image + structured prompt
  | GOLDEN RULES enforce: no hallucination, column discipline (Vehicle A vs B),
  |   page discipline, output format constraints
  | Field extraction hints guide model attention to specific regions
  |
  v
MAJORITY VOTING
  | For each of 88 fields: compare 3 extraction results
  | Select majority answer (case-insensitive matching, preserve original casing)
  |
  v
NORMALIZATION (70+ rules)
  | Date formats, address parsing, Portuguese name conventions
  | License plate format validation, phone number normalization
  | Diacritic-aware matching
  |
  v
OUTPUT: Structured JSON with all 88 fields
```

[SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md, Sections 4-6; FIELD-INVESTIGATION-LOG.md; extraction-runners.ts — voting logic]

### Where the 18.5% Error Gap Comes From

| Error Source | % of Errors | ~Fields Affected | Fixability |
|-------------|------------|------------------|------------|
| A/B Column confusion (Vehicle A vs Vehicle B data swapped) | 30% | ~110 | Medium — prompt engineering (column hints) |
| Address parsing (Portuguese address formats) | 16% | ~60 | Medium — better normalization + zone cropping |
| Diagram interpretation (hand-drawn impact points) | 15% | ~55 | Medium — impact vocabulary + zone cropping |
| Handwriting quality (illegible) | 10% | ~37 | Low — inherent to handwriting |
| Date/number format mismatches | 10% | ~37 | High — normalization rules (mostly done) |
| Over-extraction (model hallucinates data) | 10% | ~37 | Medium — prompt constraints |
| Pure OCR errors (model cannot read text) | 9% | ~33 | Very low — fundamental model limitation |

[SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md, Section 4]

### Path to 90%+

The accuracy roadmap is gated on both engineering effort and dataset size:

```
Current: 81.5%
    |
    +-- TIER 2 (Next 2 weeks): Prompt + preprocessing -> 83-85%
    |   Column A/B hints, image preprocessing (deskew, binarize PDFs),
    |   address normalization expansion
    |
    +-- TIER 2.5 (Parallel): Grow dataset to 200+
    |   Image augmentation (44 x 5 = 220 variants)
    |   Synthetic DAAA form generation (100-200 forms)
    |   Validate production extractions -> add to training_claims
    |
    +-- TIER 3 (When dataset >= 200): Fine-tune -> 88-90%
    |   Fine-tune gemini-2.5-flash on Vertex AI (NO responseSchema)
    |   Output format learned from training data, not constrained at inference
    |   Field confidence scoring + selective re-extraction
    |
    +-- TIER 4 (3+ months): Architecture change -> 95%+
        Human-in-the-loop for low-confidence fields
        Template-based per-field zone extraction
```

**Critical constraint:** Fine-tuning at 44 examples gets you model compression (cheaper inference), NOT accuracy gains. Research shows fine-tuning outperforms prompting only at 200+ examples for structured extraction. The dataset must grow before fine-tuning delivers value. [SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md, Section 7 — Databricks study, ArXiv 2412.13859]

**Mistral OCR 3 eliminated as ensemble candidate.** Independent benchmarks from Reducto showed 45.3% accuracy on structured forms (vs. Mistral's self-reported 88.9%). Gemini 2.0 Flash scored 80.1% on the same benchmark. Multi-model ensembling is not worth the complexity. [SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md, Section 7 — Reducto RD-FormsBench]

### The Benchmark System

`benchmark-with-db.ts` is the automated accuracy tracking system. It:
1. Takes a claim image and its ground truth JSON
2. Runs the extraction pipeline (with current production configuration)
3. Compares extracted fields to ground truth using normalizedMatch()
4. Stores results in Supabase with model ID, configuration, and per-field accuracy
5. Enables A/B testing of prompt changes, model swaps, and preprocessing options

Every change to the extraction pipeline is measured against the full 44-claim corpus before deployment. This prevents regressions — a lesson learned from A/B testing where "concise hints showed +2.86% in isolation, but -0.91% when combined with production stack (GOLDEN RULES + x3 voting)." [SOURCE: FIELD-INVESTIGATION-LOG.md — AB-TEST-LEARNINGS]

---

## 7.5 Convention Matching Engine

### What Convention Systems Are

European motor claims use standardized inter-insurer settlement protocols. When two cars collide, both insurers participate in a convention system that applies deterministic fault rules based on the facts of the accident (checkboxes on the EAS form, diagram, and circumstances). The convention outputs a fault percentage, and the insurers settle with their own policyholders directly — then recover from each other.

Convention systems promise 60-70% straight-through processing (STP) for motor claims. Actual STP rates are approximately 10%. The gap is data quality — getting clean, structured data FROM the paper EAS form INTO the convention system. That is where Mysa's OCR pipeline fits. [SOURCE: mysa_product_strategy.md, Part 6c — STP Reality Gap]

### Convention Systems by Country

| Country | Convention | How It Works | Key Data |
|---------|-----------|-------------|----------|
| **Portugal** | IDS / CIMPAS | Direct compensation protocol. Both insurers settle with own policyholder. | 91% inter-insurer agreement rate. 1.94 days avg decision time. ~100% market participation |
| **Spain** | CIDE / ASCIDE / CICOS | Tabla de Culpabilidad (fault table) + CICOS digital platform. | 70-83% of all motor claims. 2.5M claims/year via CICOS |
| **France** | IRSA | 13 standardized cases. Outputs only 0%, 50%, or 100% fault. | Simplest fault model. ~80% of material motor claims. 7.4M claims/year |
| **Italy** | CARD | Mandatory for 2-vehicle claims, <9% permanent disability. Civil code + CAI form. | Most complex form. 2M claims paid annually, avg EUR 2,105 |

[SOURCE: mysa_product_strategy.md, Part 6b — Convention Systems by Country]

### How It Works Technically

The convention matching engine is deterministic — it is not an AI model. It is a rules lookup:

```
STRUCTURED EAS DATA (from OCR pipeline)
  |
  v
INPUT EXTRACTION
  | Checked boxes (circumstances 1-17)
  | Vehicle positions (from diagram)
  | Number of vehicles involved
  | Injury presence/absence
  |
  v
CONVENTION RULE LOOKUP
  | Match checkbox combination to convention case number
  | Each convention defines a fixed fault table:
  |   - Portugal (CIMPAS): case number -> fault split (e.g., 100/0, 50/50)
  |   - France (IRSA): 13 cases -> 0%, 50%, or 100% fault only
  |   - Spain (CIDE): Tabla de Culpabilidad -> fault percentage
  |   - Italy (CARD): civil code articles -> fault determination
  |
  v
OUTPUT
  | Convention case matched (with confidence)
  | Fault percentage per party
  | Settlement recommendation
  | Supporting documentation auto-generated
```

The convention lookup itself is trivial — it is a database query. The hard problem is not the lookup. The hard problem is getting clean, structured, validated data out of a messy handwritten form and into the lookup. That is the OCR pipeline's job.

**Current status:** CIMPAS/IDS rules encoded for Portugal. Spain (CIDE), France (IRSA), and Italy (CARD) are on the roadmap for months 4-9. [SOURCE: mysa_product_strategy.md, Parts 6d, 7]

### Why This Is a Structural Moat

Convention system expertise takes years to build. Each country has different:
- Form formats (EAS layout differs per country)
- Checkbox semantics (what each circumstance means)
- Fault calculation tables
- Dispute resolution procedures
- Digital platform integration (CICOS in Spain, etc.)

No competitor in the claims AI space has built convention matching. Five Sigma does not do it. Shift Technology does not do it. Assured does not do it. This is Mysa's EU-specific wedge. [SOURCE: mysa_product_strategy.md, Part 4a — Five Sigma gaps; Part 4c — Shift Technology gaps]

---

## 7.6 Integration Map: Open vs. Locked

Mysa operates as a decision layer that sits on top of existing carrier systems. The integration landscape ranges from fully open (REST APIs, documented endpoints) to completely locked (proprietary, no external access).

### Integration Accessibility Table

| System | Category | Access Level | Integration Path | Notes |
|--------|----------|-------------|-----------------|-------|
| **Audatex / Solera** | Estimation (EU) | **OPEN** | REST APIs. Present in 130+ countries. 95% of UK motor insurers. | Dominant EU estimation platform. Qapter AI photo estimating. [SOURCE: claims_adjuster_tech_stack_research.md — Solera Qapter] |
| **Duck Creek Claims** | CMS | **OPEN** | Cloud-first on Azure. Modular API. Partnership ecosystem with Shift Technology and others. | Trusted by 40 of top 50 global insurers (full suite). [SOURCE: claims_adjuster_tech_stack_research.md; Five_Sigma_vs_Shift_Technology_Deep_Research.md — Duck Creek partnership] |
| **LexisNexis** | Data / Analytics | **OPEN** | REST APIs. Insurance data products (claims history, risk scoring). | Predicts 60% of non-injury claims triaged through automation by 2027. [SOURCE: Phase_10_Settlement_Research.md] |
| **Five Sigma** | CMS | **OPEN** | REST APIs. Designed for overlay on any CMS. | "REST API on any CMS — proven this approach works." [SOURCE: mysa_product_strategy.md, Part 4a] |
| **Sapiens** | CMS | **OPEN** | Multi-line, multinational. Strong EU + APAC. API available. | Stronger in Europe than US. [SOURCE: claims_adjuster_tech_stack_research.md] |
| **GT Motive** | Estimation (EU) | **OPEN** | Transaction-based pricing. Growing Solera challenger. Verisk integration. | 80+ companies, 5M+ estimates/year. [SOURCE: claims_adjuster_tech_stack_research.md] |
| **Xactimate (Verisk)** | Estimation (US) | **PARTNER-GATED** | Partner program available. APIs exist. RoofScope, Hover, Scope Technologies all plug in. | 75-80% US property market share. Open ecosystem but Verisk controls the terms. [SOURCE: home_property_competitive_deep_dive.md — "partner program"; mysa_product_strategy.md, Part 4b] |
| **Guidewire ClaimCenter** | CMS | **PARTNER-GATED** | Guidewire Marketplace. Validated accelerator program. Strategic partnerships (e.g., Shift Technology since Nov 2024). | ~21% insurance software market. Most top-25 US carriers. Certification/validation required. [SOURCE: claims_adjuster_tech_stack_research.md; Five_Sigma_vs_Shift_Technology_Deep_Research.md — Guidewire partnership] |
| **Mitchell (Enlyte)** | Estimation + BI | **PARTNER-GATED** | WorkCenter platform. Partner ecosystem. Bundled APD + BI (InjuryIQ). | ~28% US estimating market. Tightly integrated casualty suite. [SOURCE: claims_adjuster_tech_stack_research.md] |
| **CCC Intelligent Solutions** | Estimation (US) | **PARTNER-GATED** | CCC IX Cloud network (35,000+ businesses). CIECA standards for data exchange. | ~50% US auto claims volume. Dominant. "Insurers locked into CCC's ecosystem." [SOURCE: claims_adjuster_tech_stack_research.md; claims_service_blueprint.jsx] |
| **Hi Marley** | Communication | **OPEN** | Integrates with Guidewire ClaimCenter and Verisk XactAnalysis. | Purpose-built SMS for P&C. Growing. [SOURCE: claims_adjuster_tech_stack_research.md] |
| **Colossus (DXC)** | BI Valuation | **LOCKED** | Proprietary. No public API. 750 injury codes, 10,720 value drivers. 50+ years of data. | Used by 70%+ of US insurers. Outputs settlement range. No external integration path. [SOURCE: claims_adjuster_tech_stack_research.md; meeting_notes_2026-02-09_claims_workflow.md — "Colossus (70% market share, 50+ years data)"] |
| **ImageRight (Vertafore)** | Document Mgmt | **PARTNER-GATED** | Direct integration with Guidewire ClaimCenter. | Leading insurance-specific DMS. [SOURCE: claims_adjuster_tech_stack_research.md] |
| **Legacy Mainframe / AS400** | CMS (legacy) | **LOCKED** | No API. Green-screen terminal access only. 74% of insurers still run some legacy tech. | COBOL/RPG systems built 30+ years ago. Engineers retiring. [SOURCE: claims_adjuster_tech_stack_research.md] |

### Strategic Implications

**For EU launch (Months 1-9):** Audatex/Solera and Duck Creek/Sapiens are open and cover the majority of EU mid-market carriers. Convention platforms (CICOS in Spain) have digital interfaces. The integration path for EU motor is clear.

**For US expansion (Months 10+):** Xactimate is gated but accessible through the partner program. Guidewire requires marketplace validation. CCC is the gatekeeping risk — their ecosystem is dominant and their partner terms are restrictive. Colossus has no integration path and must be approached differently (see Section 7.7).

**For legacy systems:** 74% of insurers still run some legacy technology. Many mid-market carriers have a Guidewire or Duck Creek claims system but a 20-30 year old mainframe for policy administration. The adjuster logs into the legacy system in a separate window to verify coverage, then manually transfers the information. This is where the agent/extension approach (Section 7.7) becomes critical.

[SOURCE: claims_adjuster_tech_stack_research.md, Sections 1-6; mysa_product_strategy.md, Part 5c]

---

## 7.7 Agentic Approach for Locked Systems

### The Problem

Several critical systems in the adjuster's workflow have no API or require partnership agreements that take months to years to establish. Colossus (70%+ of US BI claims) is entirely proprietary. Legacy mainframe policy systems have green-screen interfaces only. Even partner-gated systems like Guidewire require marketplace certification before integration.

Waiting for API access is not an option for a startup that needs to deliver value in weeks, not quarters.

### The Solution: Chrome Extension + Desktop Agent

> "Insurance knowledge Clippy" — sits on top of whatever system the adjuster uses. Like Superhuman for email. Context-aware across all pages. Chat with Vault knowledge base.
> [SOURCE: MODULE_01_POSITIONING.md, Section 1.6 — Chrome Extension / Clippy, Months 3-6]

The Chrome extension / desktop agent architecture allows Mysa to:

1. **Read data from any browser-based system** — observe what the adjuster sees on screen (Guidewire, Duck Creek, legacy web portals, insurer portals)
2. **Provide contextual recommendations** — overlay AI guidance on top of whatever application is open
3. **Capture decision reasoning** — when an adjuster makes a decision in their CMS, the extension captures the context and the choice as training data
4. **Work without API integration** — no backend connection to the carrier's CMS required for the overlay layer

```
ADJUSTER'S EXISTING WORKFLOW
  |
  +-- Opens Guidewire ClaimCenter (or Duck Creek, or legacy web app)
  |     |
  |     +-- Mysa Chrome Extension reads page context
  |     |     (claim number, policy data, reserve amounts, etc.)
  |     |
  |     +-- Mysa overlay panel appears:
  |           - Coverage analysis recommendation
  |           - Convention match result (EU motor)
  |           - Reserve suggestion with confidence interval
  |           - SOP compliance checklist
  |           - "Ask Vault" chat interface for knowledge queries
  |
  +-- Adjuster reviews recommendations
  |     |
  |     +-- Accepts / modifies / rejects each recommendation
  |           (every interaction = training data)
  |
  +-- Adjuster enters decision into CMS (their normal workflow)
        |
        +-- Extension captures: what was decided vs what was recommended
```

### Why This Works

This is the same architectural pattern that Superhuman used for email and that Grammarly used for writing — a lightweight layer that augments the existing tool without replacing it.

**For sales:** "We don't change how you work. We sit on top of your existing system." This removes the #1 adoption objection: "I don't want to learn another system." [SOURCE: MODULE_01_POSITIONING.md, Section 1.5 — Sales Version]

**For locked systems:** The extension can read data from Colossus output screens, from legacy mainframe web terminals, from any browser-based application. No API required. No partner agreement required.

**For data capture:** Every adjuster interaction — accept, modify, reject — creates labeled training data. This is how the decision ground truth flywheel works: better data leads to better recommendations leads to more trust leads to more data. [SOURCE: mysa_product_strategy.md, Part 5a — Step 7: Feedback Loop]

### Limitations

- Cannot write data back to locked systems (read-only from screen). Adjuster must still enter decisions manually into their CMS
- Dependent on screen structure — if Guidewire changes its UI layout, the extension needs updating
- Enterprise carriers may have browser extension policies that block installation
- Does not work for thick-client (non-browser) applications without a desktop agent component

### Build vs. Wait Decision [FOUNDER INPUT REQUIRED]

| Path | Timeline | Risk |
|------|----------|------|
| **Build Chrome extension early (Months 3-6)** | Immediate value for adjusters on any system. Captures training data from Day 1 | Extension maintenance burden. Browser compatibility issues |
| **Pursue API partnerships first, extension as fallback** | Cleaner architecture. More reliable data flow | Slower to market. Blocked by partnership timelines |
| **Both in parallel** | Extension for immediate value + partnerships for long-term reliability | Resource split for small team |

**Recommendation for Jeremy:** Build the Chrome extension first. It delivers value immediately, works on any carrier's system, and starts the training data flywheel. Pursue API partnerships in parallel as they become commercially necessary (when specific carriers require deeper integration for production use).

---

## 7.8 Data Model & Knowledge Layer

### Core Entities

The knowledge layer is the structural moat. It stores carrier-specific rules, workflow templates, historical enforcement patterns, and decision ground truth — data that compounds over time and cannot be purchased.

```typescript
// Insurer / Carrier Rule Set
interface InsurerKnowledge {
  insurer_id: string
  insurer_name: string

  // Code mappings (EU healthcare origin, extends to claims)
  terminology: {
    mcdt_code: string
    insurer_name: string
    insurer_code?: string
    specialty?: string
    notes?: string
  }[]

  // Workflow rules (SOP-driven)
  workflows: {
    specialty: string
    request_type: 'pre-auth' | 'claim' | 'convention' | 'property'
    steps: WorkflowStep[]
    required_fields: string[]
    required_documents: string[]
    estimated_response_days: number
    authority_limits: AuthorityLevel[]  // Approval thresholds per adjuster level
  }[]

  // Submission rules
  submission: {
    deadline_days_from_service: number
    deadline_days_pre_auth_validity: number
    portal_url: string
    api_available: boolean
    format_requirements: FormatRule[]
  }

  // Enforcement patterns (LEARNED from claim outcomes)
  enforcement: {
    denial_reasons: DenialPattern[]
    approval_patterns: ApprovalPattern[]
    gray_areas: GrayArea[]  // Things that sometimes pass, sometimes don't
  }
}
```

[SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 5.2 — Knowledge Schema]

```typescript
// Denial Pattern (learned from historical data — highest-value knowledge)
interface DenialPattern {
  reason_code: string
  reason_text: string
  frequency: number           // How often this denial occurs
  procedures_affected: string[]
  common_causes: string[]
  successful_appeals: number
  appeal_success_rate: number
  recommended_fix: string
}

// Decision Ground Truth (the flywheel data)
interface DecisionGroundTruth {
  claim_id: string
  carrier_id: string
  decision_step: 'coverage' | 'policy_check' | 'repair' | 'cost' |
                 'reserve' | 'fraud'
  ai_recommendation: any     // What the AI suggested
  adjuster_action: 'accept' | 'modify' | 'reject'
  adjuster_value?: any       // What the adjuster actually decided (if modified)
  adjuster_reasoning?: string // Why (if captured)
  outcome?: 'approved' | 'denied' | 'partial' | 'appealed'
  timestamp: string
}
```

[SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 5.2; mysa_product_strategy.md, Part 5a — Step 7: Decision Ground Truth Capture]

### Knowledge Layer Sources and Ingestion

| Source | Type | Ingestion Method | Update Frequency |
|--------|------|------------------|------------------|
| Carrier SOPs | Semi-structured (PDF, Word) | LLM parsing + manual review at onboarding | Per SOP change |
| Provider contracts | Structured (PDF) | LLM extraction + human validation | Per contract renewal |
| Convention rule tables | Structured | Manual encoding per country | Rarely (rules are stable) |
| Historical claims data | Structured | Carrier data import at onboarding | One-time + continuous |
| Claim outcomes (approved/denied) | Structured | API/manual entry from carrier CMS | Continuous |
| Adjuster decisions vs AI recommendations | Structured | Chrome extension / in-app capture | Continuous (every claim) |
| Insurer portals | Semi-structured | Scraping + manual capture | Weekly / on-change |
| MCDT registry (Portugal) | Structured | Official database sync | Quarterly |
| ICD-10 codes | Structured | Official database sync | Annual |

[SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 5.1; DATA_SOURCES.md]

### Knowledge Acquisition Phases

**Phase 1 — Bootstrap (Current):** Manual ingestion from Caravela pilot. PDF parsing of contracts. Staff interviews and shadowing sessions. 44 claims with ground truth. [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 5.3]

**Phase 2 — Structured Capture:** In-app knowledge capture during claim processing. "Was this denial expected?" feedback loop. Adjuster corrections feed the knowledge base. Every accept/modify/reject is training data.

**Phase 3 — Automated Learning:** Pattern detection from claim outcomes. Anomaly detection for new denial reasons. Cross-carrier knowledge aggregation (anonymized — no PII crosses carrier boundaries).

### The Defensibility Stack

```
LAYER 1: Architecture (Medium defensibility — 6-12 months to copy)
  Agent-native from Day 1

LAYER 2: Knowledge Base (High defensibility — 12-24 months per market)
  Convention rules, carrier SOPs, workflow templates

LAYER 3: Enforcement Patterns (Highest defensibility — 2-5 years)
  What actually gets enforced vs. what's in contracts
  Historical denial data, gray area learnings
  CANNOT be bought, only learned from claim outcomes

LAYER 4: Network Effects (Future — 3-5 years)
  Cross-carrier learning (anonymized patterns)
  More carriers -> better patterns -> better outcomes -> more carriers
```

[SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8.2 — Competitive Moat Analysis]

---

## 7.9 EU + US Compliance

### GDPR (General Data Protection Regulation)

Claims data is sensitive personal data under GDPR. It includes names, addresses, policy numbers, medical information (for BI claims), financial details, and in some cases, criminal records (fraud investigations).

| GDPR Requirement | Mysa Implication |
|-----------------|------------------|
| **Consent for health data processing** | Required for any claim involving medical/injury information |
| **Data minimization** | Only collect and process data necessary for the claim decision |
| **EU-resident storage** | All personal data must be stored within the EU. Cloud infrastructure must be EU-region |
| **Retention limits** | Medical records: 5-10 years. Claims records: per carrier policy. Must support deletion |
| **Right of access** | Policyholders can request all data held about them |
| **Breach notification** | 72 hours to notify authorities of a data breach |
| **Article 22** | Prohibits "solely automated" decisions with legal or similarly significant effect. Claims decisions fall under this — human-in-the-loop is mandatory, not optional |

[SOURCE: REGULATORY_COMPLIANCE.md — Data Protection (GDPR/RGPD); mysa_product_strategy.md, Part 5d]

**Architecture response:** Human-in-the-loop at every decision point. AI recommends, adjuster decides. This is not a limitation — it is a feature:
1. Regulatory compliance baked into the architecture
2. Adoption — adjusters feel augmented, not replaced
3. Training data — every human decision creates ground truth
4. Error catching — prevents wrongful denials
5. Trust building — carriers need to see AI earn autonomy gradually

[SOURCE: mysa_product_strategy.md, Part 5d — "Human-in-the-loop is a FEATURE, not a limitation"]

### EU AI Act (Regulation 2024/1689)

The EU AI Act is expected to classify insurance claims AI as "high-risk" under Annex III — AI systems used in insurance contexts that affect access to essential services. [SOURCE: MODULE_01_POSITIONING.md, Section 1.1 — "EU AI Act classifies claims AI as high-risk"]

| AI Act Requirement | Mysa Implication |
|-------------------|------------------|
| **Conformity assessment** | Must demonstrate the system meets quality, transparency, and safety requirements before deployment |
| **Human oversight** | Decision-making authority must remain with humans — AI is advisory only |
| **Transparency** | Users (adjusters) must be informed they are interacting with AI. Recommendations must be explainable |
| **Risk management system** | Must document risks, mitigations, and ongoing monitoring |
| **Data governance** | Training data must be relevant, representative, and free from bias |
| **Technical documentation** | Full system documentation available to regulators |
| **Record-keeping** | Audit logs of all AI system outputs and human decisions |
| **Accuracy and robustness** | Must demonstrate system performs consistently and handles errors gracefully |

**Strategic implication:** Compliance with the AI Act creates a regulatory moat. Products built with human-in-the-loop, explainability, and audit trails from Day 1 will meet requirements. Competitors who bolt AI onto legacy architecture — without these properties — will face expensive retrofitting or market exclusion. [SOURCE: MODULE_01_POSITIONING.md, Section 1.1 — "Regulatory Tailwind"]

### US State-by-State Insurance Regulation

The US has no federal insurance regulator. Each of the 50 states (plus DC and territories) has its own Department of Insurance with its own rules.

| US Regulatory Dimension | Implication |
|------------------------|-------------|
| **Unfair Claims Practices Acts** | Each state defines what constitutes unfair claims handling. AI recommendations must not enable unfair practices |
| **NAIC AI Model Bulletin** | By late 2025, 23 states + DC adopted guidance on AI in insurance. Requires transparency, fairness, and human oversight |
| **Algorithmic bias** | AI trained on historical claims data may perpetuate past discrimination. Must demonstrate fairness across protected classes |
| **Explainability** | "If an adjuster cannot explain why a claim was denied, it's more difficult for the insurer to prevail." AI recommendations must cite evidence |
| **State-specific coverage rules** | 50 states have different requirements for coverage, timelines, and consumer protections. Mysa's rules engine must be state-aware |
| **Fault vs. no-fault states** | Different legal frameworks affect liability determination. 12 no-fault states have fundamentally different claims workflows |

[SOURCE: home_property_competitive_deep_dive.md — "23 states + DC adopted the NAIC AI Model Bulletin"; mysa_product_strategy.md, Part 5d]

### Data Residency Architecture

| Jurisdiction | Requirement | Technical Approach |
|-------------|-------------|-------------------|
| **EU carriers** | Data must reside in EU. GDPR Article 44+ restricts international transfers | EU-region cloud hosting (GCP europe-west or AWS eu-west). No data leaves EU boundary |
| **US carriers** | No federal data residency requirement. Some states have data protection laws (California CCPA, etc.) | US-region cloud hosting. Carrier-specific data isolation |
| **Cross-border analytics** | Anonymized patterns can flow across regions. PII cannot | Aggregation and anonymization at the data layer. Only statistical patterns shared cross-region |

### Compliance Gaps Requiring Founder Decision [FOUNDER INPUT REQUIRED]

| Gap | Decision Needed | Timeline |
|-----|----------------|----------|
| **EU AI Act conformity assessment process** | Need legal counsel to define the assessment path for Mysa as a high-risk AI system. Cost: EUR 10-50K for initial assessment | Before first EU carrier goes live in production |
| **Data Processing Agreement (DPA) template** | Standard DPA for carrier onboarding. Must cover GDPR obligations, data residency, breach notification | Before first paying customer |
| **Bias testing framework** | How to test and document that AI recommendations do not discriminate. Required by NAIC Model Bulletin and EU AI Act | Before US market entry |
| **SOC 2 / ISO 27001 certification** | Enterprise carriers will require security certification. When to invest? | When targeting carriers >EUR 200M GWP or US market. 6-12 months to obtain |

---

## Sources

| Source | Type | Sections Used |
|--------|------|--------------|
| `AI_NATIVE_ARCHITECTURE_SPEC.md` | Primary — architecture philosophy, knowledge schema, moat analysis | 7.1, 7.8 |
| `CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md` | Primary — OCR accuracy, error analysis, fine-tuning roadmap | 7.2, 7.4 |
| `mysa_product_strategy.md` Parts 4-7 | Primary — tech stack, convention systems, integration, compliance | 7.2, 7.3, 7.5, 7.6, 7.7, 7.9 |
| `LLM_ARCHITECTURE.md` | Secondary — LLM use cases, cost estimates, rate limiting | 7.3 |
| `DATA_SOURCES.md` | Secondary — Portuguese data sources, MCDT schema | 7.8 |
| `REGULATORY_COMPLIANCE.md` | Secondary — GDPR, billing requirements, appeal timelines | 7.9 |
| `claims_adjuster_tech_stack_research.md` | Primary — CMS, estimation, BI tools, DMS, communication tools | 7.6 |
| `MODULE_01_POSITIONING.md` Section 1.6 | Secondary — Product Now, Chrome extension, product roadmap | 7.2, 7.7 |
| `home_property_competitive_deep_dive.md` | Secondary — Xactimate ecosystem, US regulation | 7.6, 7.9 |
| `meeting_notes_2026-02-09_claims_workflow.md` | Transcript — integration requirements, Colossus, Vault | 7.6, 7.7 |
| `Five_Sigma_vs_Shift_Technology_Deep_Research.md` | Secondary — competitor integration approaches, partnerships | 7.6 |
| `FIELD-INVESTIGATION-LOG.md` | Internal — benchmark learnings, A/B test results | 7.4 |
| `BENCHMARK-AUDIT-FINDINGS.md` | Internal — GOLDEN RULES, prompt architecture | 7.2, 7.4 |
| `caravela-ocr.md` (memory file) | Internal — current accuracy, model details | 7.2 |

---

# Part 8: Data & Flywheel Strategy

# Module 8: Data & Flywheel Strategy

**Status:** DRAFT v1.0
**Last updated:** February 9, 2026
**Feeds:** Pitch deck Slide 8 (moat), investor data room, technical due diligence, partnership negotiations, sales collateral ("your data builds your AI")

---

## 8.1 The Data Moat Thesis

### Three Data Owners, One Gap

The insurance claims data landscape has three dominant holders. Each owns a massive, valuable dataset. None of them owns the dataset that actually matters for automating claims decisions.

| Data Owner | What They Have | What It's Worth | What's Missing |
|-----------|---------------|-----------------|----------------|
| **CCC / Verisk / Solera** | Claim **outcomes** -- what was paid, repair costs, settlement amounts. Every Xactimate estimate ever written. Regional pricing databases. 75-80% US property market share. | $35B+ market cap (Verisk alone) [SOURCE: mysa_product_strategy.md, Part 4b -- "Verisk is a $35B+ market cap public company"] | They know WHAT was decided. They do not know WHY. |
| **Anthropic / OpenAI / Google** | General intelligence -- LLMs that can read policies, parse documents, reason about text. Gemini, Claude, GPT-4o can all do OCR, summarization, structured extraction. | Hundreds of billions in combined valuation | They have no insurance domain data. They cannot tell you whether a specific claim should be covered under a specific carrier's SOP. |
| **Carriers themselves** | Their own historical claims, SOPs, underwriting rules, policy wordings. Institutional knowledge locked in the heads of adjusters with 10-20 years of experience. | Priceless to the carrier -- but siloed, unstructured, and walking out the door with every retirement | They have the data but lack the AI infrastructure to extract, structure, and learn from it. |

[SOURCE: mysa_product_strategy.md, Part 1 -- positioning; Part 4b -- Verisk analysis; Part 4e -- master comparison matrix]

### The Missing Data Category: Decision Reasoning

> "When you go to a restaurant, you see the end result. You see what you order and the end result. That's a claim. That's what they get. They don't know exactly how they got to that end result."
> -- Tiago Brigido, Co-founder [TRANSCRIPT: Feb 7, 2026]

This metaphor is the clearest articulation of the data gap. The entire insurance industry -- $1.5 trillion in annual claims paid globally -- operates on outcome data. What was the settlement? What was the reserve? What was the repair cost? These are the "dishes that arrived at the table."

Nobody captures the recipe. Nobody captures the chef's reasoning. Nobody systematically records:

- **Why** the adjuster determined coverage applied (or didn't)
- **Which** SOP steps led to the reserve amount
- **What** comparable claims the adjuster considered
- **How** the adjuster weighed conflicting evidence
- **When** the adjuster overrode the standard recommendation, and why
- **Whether** the final decision matched the AI recommendation, and if not, what the adjuster changed

This is **decision reasoning data** -- and it constitutes a genuinely new data category in insurance.

[SOURCE: mysa_product_strategy.md, Part 1 -- "The moat is decision ground truth data. Every competitor has claim OUTCOMES (what was paid). Nobody has decision REASONING (why the adjuster decided what they decided)."]

### Why Nobody Else Has It

Decision reasoning data cannot be purchased, scraped, or inferred from historical records. It can only be captured at the moment an expert makes a decision -- and only if the tool the expert is using is designed to capture it.

| Approach | Why It Fails |
|----------|-------------|
| **Mine historical claims databases** | Contains what was paid, not why. A $12,000 settlement tells you nothing about the coverage analysis, the comparable claims considered, or the SOP steps followed. |
| **Interview adjusters retrospectively** | Adjusters process 300-480 claims per year [SOURCE: mysa_product_strategy.md, Part 2a]. They cannot recall the reasoning for individual claims weeks or months later. |
| **Add AI to existing CMS** | Existing systems track case status and documents, not decision reasoning. The architecture assumes rules are code, not knowledge. Adding a chatbot to Guidewire does not capture why the adjuster decided. [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8.1 -- "Their architecture assumes rules are CODE. Adding AI doesn't change that."] |
| **Build from public data** | SOPs are proprietary. Convention system expertise is institutional. Enforcement patterns (what actually gets denied vs. what the contract says) are tacit knowledge. None of this is public. |
| **Use LLMs to generate synthetic reasoning** | An LLM trained on general insurance knowledge can guess at reasoning, but it will not know that Caravela's adjuster team overrides the standard reserve model for water damage claims in Lisbon because of a known plumbing defect pattern in pre-1970 buildings. That knowledge is carrier-specific and experience-derived. |

[SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8 -- competitive moat analysis; mysa_product_strategy.md, Part 4a -- Five Sigma gap analysis ("No decision ground truth capture -- Doesn't systematically capture WHY adjusters decide")]

### The Thesis in One Sentence

**Mysa's data moat is not claim outcomes (CCC/Verisk own those) or general AI capability (OpenAI/Anthropic/Google own that) -- it is the structured, carrier-specific decision reasoning that only exists when an expert adjuster makes a judgment call inside a tool designed to capture it.**

Every claim processed through Mysa generates this data. Every competitor would need to rebuild it from scratch. It compounds. It cannot be bought. It is the moat.

[SOURCE: mysa_product_strategy.md, Part 1 -- flywheel section; Module 1 (MODULE_01_POSITIONING.md), Section 1.1 -- "Data captured: Decision reasoning (WHY the adjuster decided)"]

---

## 8.2 Flywheel Mechanics

### The Five Stages

The data flywheel is not a marketing metaphor. It is the literal mechanism by which Mysa becomes more valuable, more accurate, and harder to displace with every claim processed. Each stage builds on the previous one, and each creates a distinct data asset that feeds the next.

```
Day 1: SOP workflows + document parsing
  |     → Basic recommendations from carrier rules
  |     → Data captured: SOP encodings, parsed document fields
  |
  v
Month 3: Historical claims data ingested
  |     → Better comparable matching, pattern recognition
  |     → Data captured: Historical claims corpus + carrier-specific norms
  |
  v
Month 6: Decision ground truth captured
  |     → Adjuster accepts/modifies/rejects AI recommendations
  |     → Data captured: Decision reasoning annotations
  |
  v
Month 12: Predictive models trained
  |     → Proactive recommendations before adjuster asks
  |     → Data captured: Prediction accuracy feedback
  |
  v
Month 18+: Near-STP for routine claims
        → Minimal human review on standard claims
        → Data captured: Full automation audit trail
```

[SOURCE: mysa_product_strategy.md, Part 1 -- flywheel diagram verbatim; TRANSCRIPT -- "When we come in and we use the historical data, and the out-of-the-box thing, we get 60%. As soon as we start getting better data and training the models, we go to 70 or 80%."]

### Stage 1: Day 1 -- SOP Workflows + Document Parsing

**What happens:** The carrier uploads their standard operating procedures. Mysa's SOP engine parses them and generates decision workflows -- step-by-step guides for how an adjuster should process each claim type per the carrier's own rules.

Simultaneously, Mysa's document parsing engine (built on the Caravela OCR foundation) begins processing incoming claim documents -- EAS forms, invoices, photos, police reports, medical records.

**Data assets created:**
- Carrier SOP encodings (proprietary knowledge base per carrier)
- Parsed document fields and extraction rules
- Convention system mappings (IDS/CIMPAS in Portugal, CIDE in Spain, IRSA in France, CARD in Italy)

**Accuracy at this stage:** ~60% recommendation accuracy. The system knows the carrier's rules but has no carrier-specific historical context. Recommendations are rule-based, not pattern-based.

> "When we come in and we use the historical data, and the out-of-the-box thing, we get 60%."
> -- Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

**Why this already has value:** Even at 60%, Mysa gives new hires the same SOP-guided workflow as a 10-year veteran. The workforce crisis (25% of adjusters retiring in 5 years, 12th fastest-declining profession) means carriers cannot afford to wait for the system to be perfect -- they need onboarding acceleration now. [SOURCE: mysa_product_strategy.md, Part 2a -- workforce demographics]

[SOURCE: mysa_product_strategy.md, Part 5a -- product flow; AI_NATIVE_ARCHITECTURE_SPEC.md, Section 5.3 -- "Phase 1: Bootstrap (Current)"]

### Stage 2: Month 3 -- Historical Claims Data Ingested

**What happens:** Mysa ingests the carrier's historical claims data -- past settlements, reserve histories, denial patterns, appeal outcomes. This is the "annotation as product" stage (detailed in Section 8.4). The carrier's historical data is structured, normalized, and indexed for comparable matching.

> "If you have the historical data, then you can start... give you already an overview of everything that happened so far. And what we think will happen based on historical data, the SOPs, and the documents uploaded so far. So you don't need to review again everything. We already start from a clean point."
> -- Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

**Data assets created:**
- Historical claims corpus (structured from carrier's raw data)
- Comparable claims index (claims matched by type, severity, coverage, geography)
- Carrier-specific norms (average reserves by claim type, typical settlement ranges, expected cycle times)
- Denial pattern database (what gets denied, how often, for what reasons)

**Accuracy at this stage:** ~70%. The system now knows both the rules (SOPs) and the patterns (historical data). Recommendations shift from purely rule-based to pattern-informed. Reserve calculations become anchored to the carrier's actual historical experience.

**Why this matters for the moat:** Historical data ingestion is the cold-start killer. On Day 1, the carrier "unlocks" its own historical data as a structured, searchable, comparable knowledge base. This is immediate, tangible value -- and it creates the switching cost. Once historical data is ingested and structured, re-doing this work from scratch with a competitor is prohibitive.

[SOURCE: mysa_product_strategy.md, Part 1 -- historical data engine; AI_NATIVE_ARCHITECTURE_SPEC.md, Section 5 -- knowledge sources]

### Stage 3: Month 6 -- Decision Ground Truth Captured

**What happens:** This is the critical inflection point. After 6 months of adjusters using Mysa, the system has captured thousands of decision events: every time an adjuster accepted an AI recommendation, modified it, or rejected it entirely.

**Data assets created:**
- Decision reasoning annotations (the new data category from Section 8.1)
- AI vs. human decision divergence patterns (where the AI gets it wrong, and why)
- Carrier-specific enforcement patterns -- what the SOP says vs. what adjusters actually do
- Confidence calibration data (when the AI says 85% confidence, is it right 85% of the time?)

**How it's captured:** At every decision point in the Mysa workflow, the system presents an AI recommendation with a confidence score and cited reasoning. The adjuster then:

```
AI Recommendation presented
  |
  +--- ACCEPT (one click) → Ground truth: AI was right
  |
  +--- MODIFY (adjuster changes parameters) → Ground truth: AI was partially right
  |         What was changed? Why? (optional annotation)
  |
  +--- REJECT (adjuster overrides completely) → Ground truth: AI was wrong
            What did the adjuster decide instead? Why?
```

**Accuracy at this stage:** ~75-80%. The system now learns from its own mistakes. Every modification and rejection is a training signal. The models begin to understand not just what the rules say, but how experienced adjusters actually apply them.

> "As soon as we start getting better data and training the models, we go to 70 or 80%."
> -- Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

**Critical insight:** This is the stage where Mysa's data becomes truly defensible. Historical claims data can be re-ingested by a competitor. SOP encodings can be re-created. But 6 months of adjuster decision reasoning -- the specific ways that Carrier X's team applies Rule Y in Situation Z -- is proprietary, experiential, and impossible to replicate without the same 6 months of production usage.

[SOURCE: mysa_product_strategy.md, Part 5a -- "STEP 7: FEEDBACK LOOP -- Decision Ground Truth Capture"; AI_NATIVE_ARCHITECTURE_SPEC.md, Section 7 -- feedback and learning loops]

### Stage 4: Month 12 -- Predictive Models

**What happens:** With 12 months of decision ground truth data, Mysa transitions from reactive (responding to adjuster queries) to proactive (anticipating what the adjuster needs before they ask).

**Data assets created:**
- Predictive models per carrier, per claim type, per decision step
- Outcome prediction accuracy scores
- Anomaly detection patterns (claims that deviate from expected paths)
- Proactive recommendation triggers

**Capabilities unlocked:**
- **Predictive reserve setting:** "Based on 847 comparable claims at this carrier, the expected reserve is EUR 4,200 with 90% confidence interval EUR 3,100-5,400"
- **Proactive fraud flagging:** "This claim matches 3 of 5 fraud indicators seen in 23 previous cases that were confirmed fraudulent"
- **Decision pre-population:** "For this claim type, adjusters at your carrier accept the standard coverage determination 94% of the time. Pre-filled for your review."
- **Cycle time prediction:** "Claims of this type and complexity typically resolve in 14 days. This one is at day 11 with 2 open items."

**Accuracy at this stage:** ~85-90%. Models are carrier-specific, trained on that carrier's actual decisions, and continuously learning. This is the stage where Mysa begins delivering measurable ROI in reserve accuracy and claims cycle time reduction.

[SOURCE: mysa_product_strategy.md, Part 1 -- flywheel Month 12; Part 5b -- Reserve Agent and Fraud Signal Agent specifications]

### Stage 5: Month 18+ -- Near-STP

**What happens:** Routine claims -- those matching well-established patterns with high model confidence -- can be processed with minimal human review. The adjuster becomes an exception handler rather than a routine processor.

**Data assets created:**
- STP eligibility models (which claims can safely be auto-processed)
- Human review trigger patterns (what makes a claim require human attention)
- Full automation audit trail (required by EU AI Act for high-risk AI systems)

**The STP gap this solves:**

Convention systems in the EU promise 60-70% straight-through processing for motor claims. Actual STP rates are approximately 10%. The gap -- 50+ percentage points -- is caused by data quality at intake. Garbage in, garbage out.

> "Convention lookup is trivial -- it's a database query. The bottleneck is getting clean, structured data FROM the EAS form INTO the convention system."
> [SOURCE: mysa_product_strategy.md, Part 6b -- convention systems analysis]

By Month 18, Mysa has solved both sides of this gap:
1. **Intake quality:** OCR + document AI has been trained on thousands of carrier-specific documents
2. **Decision quality:** Models have learned the carrier's actual decision patterns, not just the theoretical SOPs

**Accuracy at this stage:** 90%+ on routine claims. Complex claims (multi-party, large loss, potential fraud) remain human-decided but AI-pre-populated.

**The endgame data asset:** At this stage, Mysa possesses the most valuable dataset in claims insurance -- not just outcomes, not just rules, but the complete decision graph: what data came in, what rules applied, what the AI recommended, what the adjuster decided, and what the final outcome was. This is the training data for the next generation of claims AI.

[SOURCE: mysa_product_strategy.md, Part 1 -- flywheel Month 18+; Part 6b -- STP gap analysis ("EU convention systems promise 60-70% STP for motor claims. Actual STP is ~10%.")]

### Flywheel Compounding: Why Each Stage Accelerates the Next

The flywheel is not linear -- it compounds. Each stage produces data that makes the next stage arrive faster and work better.

| From Stage | To Stage | Compounding Effect |
|-----------|---------|-------------------|
| Stage 1 (SOPs) | Stage 2 (Historical) | SOP encodings tell the system what to look for in historical data. Without SOPs, historical ingestion is undirected. |
| Stage 2 (Historical) | Stage 3 (Ground Truth) | Historical comparables make AI recommendations better from Day 1 of ground truth capture, so adjusters trust and engage with recommendations more, generating more ground truth data. |
| Stage 3 (Ground Truth) | Stage 4 (Predictive) | More ground truth = more training signal = faster convergence to accurate predictions. A carrier with 50K claims/year generates ground truth 10x faster than one with 5K. |
| Stage 4 (Predictive) | Stage 5 (Near-STP) | Better predictions = higher confidence scores = more claims eligible for STP = less adjuster time per claim = adjusters handle more claims = more ground truth generated per adjuster. |
| Stage 5 (Near-STP) | Stage 1 (new carrier) | STP proof points from Carrier A become sales material for Carrier B. Cross-carrier patterns (anonymized) give new carriers a head start -- the flywheel feeds itself. |

[SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 7 -- feedback and learning loops; mysa_product_strategy.md, Part 1 -- flywheel analysis]

---

## 8.3 Datasets: Connect vs Build

Not all data needs to be created from scratch. Some datasets already exist and should be connected to; others are genuinely new and must be built. The distinction is strategic: "connect" datasets are commodities (available to competitors too), while "build" datasets are proprietary moats.

### Datasets to Connect (External, Available)

| Dataset | Source | What It Contains | How Mysa Uses It | Competitive Access |
|---------|--------|-----------------|-----------------|-------------------|
| **CCC pricing data** | CCC Intelligent Solutions | US auto repair costs, parts pricing, labor rates | Input to Cost Analysis agent (Decision Sub-Step 4) | Available to any licensee -- not a moat |
| **Xactimate estimates** | Verisk | Property repair cost estimation -- scopes, materials, labor | Integration for Assessment step. "How can we integrate with them? I want this integrated with them." [TRANSCRIPT: Feb 7, 2026] | 75-80% US market share. Must integrate, not compete. [SOURCE: mysa_product_strategy.md, Part 4b] |
| **Audatex/Solera estimates** | Solera | EU motor repair cost estimation | EU equivalent of Xactimate. Required for repair assessment in EU markets. | Standard EU market data |
| **NAIC data** | National Association of Insurance Commissioners | US insurer financials, complaint ratios, market share | Carrier segmentation, market intelligence. Used to identify and prioritize mid-market targets ($100-500M GWP). | Public data -- available to everyone |
| **Convention databases** | IDS/CIMPAS (Portugal), CIDE/CICOS (Spain), IRSA (France), CARD (Italy) | Fault determination rules, inter-insurer settlement protocols | Core wedge product. Convention matching is deterministic but requires structured input data (which Mysa's OCR provides). | Rules are published. The expertise in implementing them is the moat -- not the rules themselves. [SOURCE: mysa_product_strategy.md, Part 6b -- "Convention lookup is trivial -- it's a database query"] |
| **LexisNexis enrichment** | LexisNexis Risk Solutions | Claimant history, prior claims, address verification, identity data | Fraud detection signal enrichment. Input to Fraud Signal Agent (Decision Sub-Step 6). | Available via API to licensed parties |
| **ICD-10 code databases** | CMS/CDC | ~78,000 procedure codes, diagnosis codes, coding guidelines | Medical claims parsing, BI adjuster support, healthcare-related claims | Public data -- freely available. [SOURCE: DATA_SOURCES.md -- ICD-10 International Sources] |
| **ADSE reference pricing** | Portuguese public sector | ~3,000 MCDT codes with prices, pre-auth requirements | Portuguese market baseline pricing. Public sector reference for private insurer comparison. | Public -- available to any Portuguese market participant. [SOURCE: DATA_SOURCES.md -- ADSE Tabela] |
| **Insurer portal data** | Individual carrier portals | Carrier-specific rules, submission requirements, deadline windows | Knowledge Layer ingestion. Semi-structured, scraped + manual capture, updated weekly. | Available to anyone with portal access -- but structuring it at scale is the work. [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 5 -- Knowledge Sources] |

[SOURCE: mysa_product_strategy.md, Part 5c -- technology stack and integrations; DATA_SOURCES.md -- full data source inventory; AI_NATIVE_ARCHITECTURE_SPEC.md, Section 5.1 -- knowledge sources table]

### Datasets to Build (Proprietary, Defensible)

These are the datasets that only Mysa can create. They are the moat.

| Dataset | How It's Created | Why Nobody Else Has It | Defensive Value |
|---------|-----------------|----------------------|----------------|
| **Decision reasoning annotations** | Captured at every decision point: AI recommendation + adjuster action (accept/modify/reject) + adjuster's reasoning. Structured, timestamped, linked to claim data. | Requires a tool designed to capture reasoning in-workflow. Existing CMS systems track status changes, not decision logic. Five Sigma's Clive "doesn't systematically capture WHY adjusters decide." [SOURCE: mysa_product_strategy.md, Part 4a] | **Highest** -- cannot be purchased, retrospectively reconstructed, or synthetically generated. Grows with every claim. |
| **Carrier-specific SOP knowledge** | SOPs uploaded by carrier, parsed by Mysa, converted to decision workflows. Includes proprietary authority levels, escalation thresholds, exception rules. | SOPs are proprietary documents. Each carrier's rules are different. Encoding them requires domain expertise + AI parsing + carrier collaboration. | **High** -- once encoded, switching to a competitor means re-encoding from scratch. "Creates switching costs -- once SOPs are encoded, the carrier is locked in." [SOURCE: mysa_product_strategy.md, Part 1] |
| **Historical claims patterns (structured)** | Carrier's historical claims data ingested, normalized, and indexed for comparable matching. Not the raw data (carrier owns that) -- the structured, searchable, ML-ready version. | Raw data exists at the carrier. The structured, normalized, comparable-indexed version only exists in Mysa after ingestion. | **High** -- re-ingesting and re-structuring historical data with a competitor is months of work. |
| **Enforcement patterns** | Learned from claim outcomes over time: what the SOP says vs. what actually gets approved/denied. Gray areas where enforcement is inconsistent. | Can only be learned from production claim volume over 12-24 months. "CANNOT be bought, only learned." [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8.2 -- Layer 3] | **Very high** -- requires years of claim volume. Time-to-replicate: 2-5 years. [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8.3] |
| **Cross-carrier learning corpus (anonymized)** | Aggregated, anonymized patterns across all Mysa carrier customers. "Clinic A submits to Allianz -> Denied. Clinic B in same situation -> Mysa warns." Patterns flow across carriers without exposing individual data. | Requires network scale -- multiple carriers processing claims through the same platform. | **Highest (at scale)** -- network effect. More carriers = better patterns = better outcomes = more carriers. Time-to-replicate: 3-5 years. [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Sections 7.3 and 8.2 -- Layer 4] |
| **Convention system implementation expertise** | Country-by-country convention system knowledge: IDS/CIMPAS (Portugal), CIDE/ASCIDE/CICOS (Spain), IRSA (France), CARD (Italy). Not the published rules -- the implementation: how to parse EAS forms, map to convention tables, handle edge cases. | Rules are public. Implementation requires processing thousands of real claims through each system. Mysa has built IDS/CIMPAS (91% agreement rate) and is building CIDE, IRSA, CARD. [SOURCE: mysa_product_strategy.md, Part 6b] | **High** -- "Convention system intelligence -- country-by-country, takes years to replicate." [SOURCE: mysa_product_strategy.md, Slide 8 -- Moat] |
| **OCR training corpus** | 44 validated ground truth claims (current). Growing via image augmentation, synthetic form generation, and organic production validation. Target: 350-500+ for fine-tuning. [SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md, Section 7 -- dataset growth strategy] | Form-specific, language-specific (Portuguese diacritics), handwriting-inclusive ground truth does not exist as a public dataset. The closest benchmark (BRESSAY) is Brazilian Portuguese historical documents, not Portuguese insurance forms. | **Medium** -- valuable for OCR accuracy but could theoretically be rebuilt by a determined competitor with access to similar forms. |

[SOURCE: mysa_product_strategy.md, Parts 1, 4a, 4e -- competitive gaps; AI_NATIVE_ARCHITECTURE_SPEC.md, Sections 5, 7, 8 -- knowledge layer, feedback loops, moat analysis; CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md, Sections 7-8 -- dataset strategy]

### The Strategic Distinction

"Connect" datasets are table stakes. Every claims AI company will integrate with CCC, Xactimate, LexisNexis. These integrations are necessary but not differentiating.

"Build" datasets are the moat. Decision reasoning annotations, carrier-specific SOP knowledge, enforcement patterns, and cross-carrier learning are datasets that only exist because adjusters use Mysa to make decisions. They cannot be replicated by a competitor without building the same product, winning the same carriers, and waiting the same months or years for the data to accumulate.

The investor argument: "We integrate with the same data everyone else has. But we also build a dataset nobody else can build -- because we are the only tool in the workflow where the decision happens."

---

## 8.4 Annotation as Product & Strategic Asset

### The Core Insight

Most AI companies treat data annotation as a cost center -- something that must be done before the product works. Mysa treats annotation as the product itself. When a carrier comes onboard, the first thing that happens is their historical data gets annotated. This is not pre-work for the real product; it IS the real product delivering immediate value.

### (a) Solving Cold Start: Historical Data Unlocks Day 1 Value

Every AI product faces the cold-start problem: the system needs data to be useful, but it cannot collect data until users find it useful enough to adopt.

Mysa's cold-start solution is elegant: the carrier's own historical data.

> "If you have the historical data, then you can start... give you already an overview of everything that happened so far. And what we think will happen based on historical data, the SOPs, and the documents uploaded so far. So you don't need to review again everything. We already start from a clean point."
> -- Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

**How it works:**

```
Day 0: Carrier signs contract
  |
  v
Week 1-2: Historical data ingestion
  |  - Carrier exports 2-5 years of claims data from CMS
  |  - Mysa normalizes, structures, indexes
  |  - Comparable claims matching enabled
  |  - Carrier-specific norms calculated (avg reserve, settlement ranges, cycle times)
  |
  v
Week 3-4: SOP encoding
  |  - Carrier provides SOPs (PDFs, manuals, internal docs)
  |  - Mysa parses into decision workflows
  |  - Authority levels, escalation thresholds, exception rules encoded
  |
  v
Week 5+: GO LIVE with ~60-70% recommendation accuracy
     - Historical comparables drive recommendations
     - SOP workflows guide adjuster decisions
     - Every new decision improves the system further
```

A new carrier "unlocks" their own data on Day 1. They do not wait months for Mysa to learn -- Mysa learns from their past to serve their present.

[SOURCE: mysa_product_strategy.md, Part 1 -- historical data engine section; AI_NATIVE_ARCHITECTURE_SPEC.md, Section 5.3 -- knowledge acquisition strategy]

### (b) Creating Switching Costs: Re-annotating from Scratch Is Prohibitive

Once a carrier's historical data has been ingested, normalized, and indexed in Mysa -- and once 6-12 months of decision reasoning has been captured -- switching to a competitor requires:

| Switching Cost | Effort to Replicate |
|---------------|-------------------|
| Re-ingesting 2-5 years of historical claims data | 2-4 weeks of data engineering |
| Re-encoding all SOPs into new system's format | 4-8 weeks of domain work |
| Losing 6-12 months of decision reasoning data | **Cannot be replicated** -- that data only exists in Mysa |
| Losing carrier-specific enforcement patterns | **Cannot be replicated** -- learned from production outcomes |
| Re-training all adjusters on new workflows | 2-4 weeks of change management |
| Re-calibrating confidence thresholds and trust levels | 3-6 months of production usage |

The first two items are painful but achievable. The middle two are impossible to replicate -- that decision reasoning data is gone if the carrier leaves Mysa (or at minimum, would need to be regenerated from scratch over another 6-12 months with a new tool). The last two are organizational friction that makes switching even more costly.

Net effect: after 12 months, switching costs are measured in years, not weeks.

[SOURCE: mysa_product_strategy.md, Part 1 -- "Creates switching costs -- once SOPs are encoded, the carrier is locked in"; AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8.3 -- time-to-replicate estimates]

### (c) The Sales Argument: "We Give YOU Tools to Build YOUR AI on YOUR Data"

This is the critical difference between Mysa's positioning and the incumbents'. Mysa does not extract value from the carrier's data -- it helps the carrier extract value from their own data.

**The pitch to VP Claims:**

> "Your adjusters have 10 years of institutional knowledge. 25% of them are retiring in 5 years. Today, that knowledge walks out the door when they leave. With Mysa, every decision they make gets captured, structured, and used to train your system. Your data builds your AI. You own the knowledge -- we provide the infrastructure."

**Why this matters in insurance specifically:**

Insurance carriers are among the most data-protective organizations in the world. They handle PII, PHI, financial data, and proprietary underwriting models. Any tool that appears to extract their data for use by competitors will be rejected immediately.

Mysa's architecture addresses this directly:
- Carrier-specific models are trained on carrier-specific data
- Cross-carrier learning uses anonymized patterns only (see Section 8.7)
- The carrier's raw data never leaves their Mysa instance
- Decision reasoning annotations belong to the carrier

This is not just a privacy compliance feature -- it is a sales enabler. The conversation shifts from "give us your data so our AI can learn" to "we give you tools to build your own AI on your own data."

[SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 7.3 -- privacy model ("Clinic-specific data: Private to clinic. Patterns and rules: Aggregated, anonymized, shared. No PHI ever leaves clinic boundary.")]

### (d) The Quality Flywheel: 44 Claims to Normalization Rules to Accuracy

The Caravela OCR project provides a concrete, measurable example of how annotation drives product quality.

**The sequence:**

```
44 claims manually annotated with ground truth
  |
  v
Benchmark system identifies systematic errors:
  - 30% of errors from A/B column confusion
  - 16% from address parsing
  - 10% from date/number format mismatches
  |
  v
70+ normalization rules created from error patterns:
  - House number normalization
  - Date format standardization
  - Portuguese diacritic handling
  - Address component parsing
  |
  v
Accuracy improves: 79.9% -> 81.5% normalized
  (44 claims, 2990 fields, normalizedMatch())
  |
  v
Each new annotated claim refines rules further
  - More edge cases captured
  - More normalization patterns discovered
  - Training dataset grows toward 350-500+ (fine-tuning threshold)
```

[SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md -- Section 4 ("WHERE OUR ERRORS COME FROM"), Section 7 ("Dataset Growth Strategy"); caravela-ocr.md memory file -- "44 claims with GT, normalizedMatch(), 81.5%"]

This is not hypothetical. 44 annotated claims directly produced 70+ specific normalization rules that directly improved accuracy by 1.6 percentage points. Each additional annotated claim adds to this corpus. The path forward is clear:

| Dataset Size | Expected Capability | Source |
|-------------|-------------------|--------|
| 44 claims (current) | Prompt engineering + normalization rules. 81.5% accuracy. | Internal benchmark, Feb 8, 2026 |
| 100-200 claims | Fine-tuning viable. "Google's recommended starting range." | CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md, Section 7 |
| 200-1,000 claims | "Sweet spot for document extraction." Significant accuracy gains expected. | Multiple sources cited in CARAVELA assessment |
| 1,000+ claims | Carrier-specific fine-tuned models. 90%+ accuracy ceiling within reach. | Industry benchmarks |

[SOURCE: CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md, Section 7 -- "The Real Blocker: 44 Examples Is Too Few"]

### (e) A New Data Category Nobody Else Has

Section 8.1 established that decision reasoning data is a new category. The annotation-as-product model is how that category gets populated. Every carrier that onboards Mysa contributes to this category through two channels:

1. **Historical annotation:** Past claims data is structured and indexed, creating a retrospective decision context (what happened, in what sequence, with what outcome)
2. **Ongoing annotation:** Every adjuster decision in Mysa is a forward-looking annotation (what the AI recommended, what the adjuster decided, and why)

The cumulative effect across carriers is a dataset that has never existed in insurance: a structured corpus of expert decision reasoning, carrier by carrier, claim type by claim type, decision step by decision step. This is the training data for the next generation of claims AI -- and Mysa is the only path to generating it.

[SOURCE: mysa_product_strategy.md, Part 1 -- "Mysa captures the HOW -- and that's the training data nobody else has"; Part 5a -- "STEP 7: FEEDBACK LOOP -- Decision Ground Truth Capture"]

---

## 8.5 Legal Framework for Data Operations

### The Regulatory Landscape

Mysa processes some of the most sensitive data categories in existence: personal identifiable information (PII), protected health information (PHI) in bodily injury claims, financial data, and proprietary carrier business rules. Operating across the EU and (eventually) US markets requires a rigorous legal framework.

### Data Processing Agreements (DPAs)

Every carrier engagement requires a DPA that specifies:

| DPA Element | Mysa's Position | Legal Basis |
|------------|----------------|-------------|
| **Data controller** | The carrier. Mysa is the data processor. | GDPR Article 28 -- processor must act only on controller's instructions |
| **Processing purposes** | Claims decision support, model training (carrier-specific), anonymized pattern aggregation | GDPR Article 6(1)(b) -- performance of contract; Article 6(1)(f) -- legitimate interest |
| **Data categories** | Claim details, policy data, adjuster decisions, document content | Specified per carrier based on claim types processed |
| **Sub-processors** | Cloud infrastructure (GCP/AWS EU-region), LLM providers (Gemini/Claude for inference) | GDPR Article 28(2) -- sub-processor authorization required |
| **Data location** | EU-resident. Encrypted at rest and in transit. | GDPR Article 44+ -- cross-border transfer restrictions |
| **Retention** | Active carrier: full data retained. Post-termination: carrier data returned/deleted within 90 days. Anonymized aggregated patterns retained. | GDPR Article 5(1)(e) -- storage limitation |
| **Breach notification** | 72 hours to carrier; carrier notifies supervisory authority | GDPR Article 33 |

[SOURCE: REGULATORY_COMPLIANCE.md -- GDPR/RGPD requirements; mysa_product_strategy.md, Part 5c -- "Data storage: Encrypted, EU-resident, GDPR Article 22 compliant"]

### Anonymization Strategy

Cross-carrier learning (Section 8.7) requires robust anonymization. Mysa's approach:

**What gets anonymized:**
- All PII (claimant names, addresses, policy numbers, license plates)
- Carrier identity (patterns shared as "Carrier in [country], [size tier]")
- Specific monetary amounts (normalized to percentages of category average)
- Dates (shifted to preserve relative timing but obscure actual dates)

**What gets shared (anonymized):**
- Decision patterns (coverage determination logic by claim type)
- Denial rate patterns by claim category and decision step
- Enforcement patterns (what actually gets denied vs. contract language)
- Reserve accuracy patterns (initial reserve vs. final settlement distributions)
- STP eligibility patterns (characteristics of claims successfully auto-processed)

**Anonymization standard:** k-anonymity (k >= 5) for any shared pattern. No pattern is shared if it could be traced to fewer than 5 carriers. Differential privacy noise applied to statistical aggregates.

> "Clinic-specific data: Private to clinic. Patterns and rules: Aggregated, anonymized, shared. No PHI ever leaves clinic boundary."
> [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 7.3 -- privacy model]

### Model Training Rights

This is the most commercially sensitive area. Clear contractual terms are required.

| Training Scope | Default Position | Negotiable? |
|---------------|-----------------|-------------|
| **Carrier-specific model training** | Mysa trains carrier-specific models on that carrier's data. Carrier benefits directly. | Non-negotiable -- this IS the product. |
| **Cross-carrier pattern learning** | Anonymized patterns used to improve general models. Carrier benefits from aggregate intelligence. | Opt-out available but strongly discouraged. Carriers who opt out get slower improvement cycles. |
| **Foundation model feedback** | Mysa does NOT feed carrier data back to LLM providers (Google, Anthropic). All training happens on Mysa's infrastructure. | Non-negotiable -- carriers will not accept data flowing to third-party model providers. |
| **Post-termination model residue** | Carrier-specific models are deleted. General patterns derived from anonymized data are retained (legally defensible under aggregation doctrine). | Standard in SaaS -- Salesforce, Palantir, and similar platforms retain aggregated learnings. |

[SOURCE: mysa_product_strategy.md, Part 5c -- "Data storage: Encrypted, EU-resident, GDPR Article 22 compliant"; Part 5d -- human-in-the-loop requirement; REGULATORY_COMPLIANCE.md -- GDPR requirements]

### Carrier Data Ownership

**Principle: The carrier owns their data. Mysa owns the models and infrastructure.**

| Data Type | Owner | Mysa's Rights |
|-----------|-------|--------------|
| Raw claims data | Carrier | Process as data processor. Return or delete on termination. |
| SOP documents | Carrier | Parse and encode. Return or delete on termination. |
| Decision reasoning annotations | Carrier | Train carrier-specific models. Anonymize for cross-carrier patterns. |
| Structured/normalized data | Carrier | Derived from carrier's raw data. Return or delete on termination. |
| Carrier-specific trained models | Joint (Mysa architecture + carrier data) | Carrier gets model outputs. Mysa retains architecture IP. Models deleted on termination. |
| Anonymized aggregate patterns | Mysa | Retained post-termination. Derived from k-anonymized cross-carrier data. |
| OCR training data | Mysa (if Mysa-annotated) / Carrier (if carrier-provided) | Mysa-annotated ground truth (e.g., the 44 Caravela claims) is Mysa IP. Carrier-provided annotations are carrier IP. |

### EU AI Act Compliance

The EU AI Act (Regulation 2024/1689) classifies insurance claims AI as high-risk under Annex III -- AI systems used in contexts affecting access to essential services. Requirements for high-risk AI systems:

| AI Act Requirement | Mysa's Approach |
|-------------------|----------------|
| **Human oversight** (Article 14) | Human-in-the-loop at every decision point. "It's mandatory to always have a human step." [TRANSCRIPT: Jeremy, Feb 7, 2026] |
| **Transparency** (Article 13) | Every AI recommendation includes confidence score, cited reasoning, and referenced SOP section |
| **Record-keeping** (Article 12) | Full audit trail: AI recommendation + adjuster action + timestamp + claim context |
| **Data governance** (Article 10) | Training data quality management, bias monitoring, representativeness checks |
| **Conformity assessment** (Article 43) | Required before market placement. Must demonstrate compliance with all Chapter 2 requirements |
| **Post-market monitoring** (Article 72) | Continuous monitoring of system performance, accuracy drift, and bias metrics |

**Regulatory moat:** Compliance is expensive and time-consuming. Competitors building on top of legacy architecture will need to retrofit human oversight and audit trails. Mysa has these built into the architecture from Day 1 -- "Human-in-the-loop is a FEATURE, not a limitation." [SOURCE: mysa_product_strategy.md, Part 5d]

[SOURCE: mysa_product_strategy.md, Part 5d -- "GDPR Article 22 prohibits fully automated decisions with legal effect. EU AI Act classifies claims AI as high-risk"; MODULE_01_POSITIONING.md, Section 1.1 -- "The EU AI Act is expected to classify insurance claims AI as 'high-risk'"]

### GDPR Compliance for Training Data

Specific GDPR considerations for using claims data to train AI models:

| GDPR Article | Application to Mysa | Compliance Approach |
|-------------|---------------------|-------------------|
| **Article 6 -- Lawful basis** | Processing claims data for AI model training | Contractual necessity (Article 6(1)(b)) for carrier-specific models. Legitimate interest (Article 6(1)(f)) for anonymized aggregate models. |
| **Article 9 -- Special categories** | Health data in BI claims, potential racial/ethnic data | Explicit consent or substantial public interest. BI claims data processed only with carrier DPA authorization. |
| **Article 22 -- Automated decisions** | AI recommendations that affect claim outcomes | Human-in-the-loop ensures no purely automated decisions. Adjuster always makes final call. |
| **Article 25 -- Data protection by design** | System architecture | Privacy by design: data minimization, purpose limitation, pseudonymization built into the data pipeline |
| **Article 35 -- DPIA** | High-risk processing of large-scale sensitive data | Data Protection Impact Assessment required before deployment with each new carrier |

[SOURCE: REGULATORY_COMPLIANCE.md -- GDPR/RGPD section; mysa_product_strategy.md, Part 5c -- data storage requirements]

---

## 8.6 Mid-market vs Small: Different Data Needs

### The Segmentation Reality

Mysa's target market spans a wide range of carrier sizes, geographies, and regulatory environments. A EUR 150M French carrier and a EUR 50M Portuguese mutual have fundamentally different data infrastructure, volume, and needs. The data strategy must account for this.

### By Carrier Size

| Dimension | Caravela Tier (EUR 100-200M GWP) | Small Carrier (EUR 50-100M GWP) | Large Carrier (EUR 200M-1B GWP) |
|-----------|----------------------------------|--------------------------------|--------------------------------|
| **Claims volume** | 30K-60K claims/year | 10K-30K claims/year | 60K-200K claims/year |
| **Data infrastructure** | Basic CMS, possibly Guidewire/Duck Creek. Some Excel. | Minimal -- possibly homegrown or heavily manual. "This spreadsheet is from one large Portuguese group with 40+ clinics, $100m in revenue. They spent millions building a submission tool. They're still on spreadsheets." [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Appendix D] | Enterprise CMS (Guidewire, Duck Creek). Dedicated IT team. Some in-house data science. |
| **Historical data quality** | Moderate -- structured in CMS but may have inconsistencies, missing fields, legacy format issues | Low -- scattered across spreadsheets, paper files, and basic databases. Significant cleanup needed. | High -- well-structured, comprehensive. But locked in enterprise systems with complex export processes. |
| **Data science capability** | Zero. "No data science team." [SOURCE: MODULE_01_POSITIONING.md, Section 1.2] | Zero. May not even have dedicated IT. | Some -- 2-10 person team. But focused on underwriting/pricing, not claims decision AI. |
| **SOP maturity** | SOPs exist but may be informal or inconsistently followed. | SOPs may be tribal knowledge, not documented. | Detailed, documented SOPs. Multiple layers of approval and compliance. |
| **Flywheel speed** | Ground truth accumulation: ~50-100K decision events/year. Meaningful predictive models by Month 9-12. | Slower: ~10-30K decision events/year. Predictive models by Month 15-18. | Fast: ~60-200K decision events/year. But enterprise procurement slows deployment by 12-18 months. |
| **Mysa data work needed** | Standard ingestion pipeline. 4-6 weeks to go live. | Heavy lift: data cleanup, SOP documentation assistance, possibly digitization of paper records. 8-12 weeks to go live. | Complex integration: enterprise CMS connectors, security reviews, data governance compliance. 12-24 weeks to go live. |

[SOURCE: mysa_product_strategy.md, Part 3a -- carrier segmentation; MODULE_01_POSITIONING.md, Section 1.2 -- carrier segmentation table]

### By Geography and Regulation

| Dimension | Portugal | Spain | France | Italy |
|-----------|----------|-------|--------|-------|
| **Convention system** | IDS/CIMPAS | CIDE/ASCIDE/CICOS | IRSA | CARD |
| **Convention data format** | EAS (European Accident Statement) + CIMPAS digital submission | EAS + CICOS digital platform | EAS (constat amiable) + IRSA manual lookup | CAI (Constatazione Amichevole) + CARD mandatory portal |
| **Motor GWP** | ~EUR 1.8B (2023) | EUR 13.2B (2024, +8.9%) | EUR 28.1B (2024, +7.3%) | ~EUR 14.8B (2023) |
| **Mid-market carriers** | 25-30 | 15-25 (80-100 total operating) | 20-30 (246 FFA members, 660 ACPR-supervised) | 10-15 (38 write RC Auto) |
| **Claims volume** | ~100-200K motor claims/year (market total) | 2.5M claims/year via CICOS | 7.4M claims/year (confirmed) | ~2M claims paid (confirmed) |
| **Data privacy regulation** | GDPR (RGPD) + CNPD (national authority) | GDPR + AEPD (national authority) | GDPR + CNIL (national authority, strictest in EU) | GDPR + Garante Privacy (national authority) |
| **Language considerations** | Portuguese diacritics (accents on a, e, o, i, u, c-cedilla). Handwritten forms common. | Spanish diacritics. Bilingual regions (Catalan, Basque, Galician). | French diacritics. Strict language requirements for official documents. | Italian diacritics. Complex bureaucratic document formats. |
| **Specific data challenges** | Small market = faster to cover but limited training data volume. 44 ground truth claims from Caravela. | Largest convention volume (2.5M/year). CICOS digital platform = more structured data available. | Simplest fault model (13 cases, only 0%/50%/100%). Mutual-heavy market structure = sometimes resistant to external tech. | Most complex form (CAI). "Most complex form. 2M claims paid." [SOURCE: mysa_product_strategy.md, Part 6b] |
| **Mysa data readiness** | IDS/CIMPAS built. OCR engine live. 91% convention agreement rate. | CIDE next to build. CICOS API integration needed. | IRSA is simpler (13 cases) but market is large and competitive. | CARD is mandatory but complex. Integration with IVASS portal required. |

[SOURCE: mysa_product_strategy.md, Part 6b -- convention systems by country (full table); Part 3a -- carrier counts and market sizing]

### Concrete Example: EUR 150M French Carrier vs EUR 50M Portuguese Mutual

**Carrier A: French mid-market insurer, EUR 150M GWP, 40K motor claims/year**

- **Data state:** Guidewire ClaimCenter deployed 3 years ago. Historical data well-structured. IRSA convention matching semi-automated. 15 adjusters.
- **What Mysa provides:** Decision layer on top of Guidewire via API integration. IRSA convention matching (13 cases -- simpler than Portuguese IDS). Historical data ingestion from Guidewire export.
- **Data volumes:** 40K claims/year = ~80K decision events/year (2 per claim average). Predictive models viable by Month 10.
- **CNIL considerations:** France's CNIL is the strictest data protection authority in the EU. DPIA required before deployment. Explicit consent requirements for any data used beyond primary processing purpose. Cross-carrier pattern sharing requires CNIL-compliant anonymization. Training data documentation must be thorough.
- **Flywheel timeline:** Day 1 to Near-STP in ~15 months.

**Carrier B: Portuguese mutual, EUR 50M GWP, 12K motor claims/year**

- **Data state:** Homegrown CMS, partially on spreadsheets. Historical data exists but inconsistent. IDS/CIMPAS conventions handled manually.
- **What Mysa provides:** Full stack -- OCR, convention matching, decision workflows. Historical data requires significant cleanup before ingestion. SOP documentation may need to be created (not just encoded).
- **Data volumes:** 12K claims/year = ~24K decision events/year. Predictive models viable by Month 18.
- **CNPD considerations:** Portuguese CNPD is less prescriptive than CNIL but GDPR applies equally. Smaller carrier = simpler DPA.
- **Flywheel timeline:** Day 1 to Near-STP in ~20 months (slower due to lower volume and data cleanup needs).

**Key implication for Mysa's data strategy:** The product must handle both extremes -- the well-structured Guidewire export and the messy spreadsheet import. Data ingestion cannot be a one-size-fits-all pipeline; it needs configurable normalization per carrier data quality level.

[SOURCE: mysa_product_strategy.md, Part 3a -- "For the mid-market ones like Caravela, they want us"; Part 6b -- convention system details; MODULE_01_POSITIONING.md, Section 1.2 -- ICP segmentation]

---

## 8.7 Network Effects & Switching Costs

### The Four Layers of Lock-in

Mysa's competitive moat is not a single asset -- it is four interlocking layers that compound over time. Each layer makes it harder for a carrier to switch and harder for a competitor to replicate.

```
LAYER 1: SOP Encoding (Months 0-2)
  |  Carrier's proprietary rules encoded into Mysa workflows
  |  Switching cost: 4-8 weeks to re-encode with competitor
  |
  v
LAYER 2: Historical Data (Months 1-3)
  |  Carrier's past claims structured, normalized, indexed
  |  Switching cost: 2-4 weeks + loss of normalization quality
  |
  v
LAYER 3: Decision Ground Truth (Months 3-12)
  |  Thousands of adjuster decisions annotated with reasoning
  |  Switching cost: CANNOT be replicated -- 6-12 months of production data lost
  |
  v
LAYER 4: Trained Models (Months 6-18)
  |  Carrier-specific predictive models trained on Layers 1-3
  |  Switching cost: Model quality resets to zero. Months to retrain.
  |
  v
LAYER 5: Cross-Carrier Network (Months 12+)
     Anonymized patterns from all Mysa carriers
     Switching cost: Individual carrier loses access to aggregate intelligence
```

[SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8.2 -- defensibility layers; mysa_product_strategy.md, Part 1 -- moat hierarchy]

### Layer-by-Layer Time to Replicate

| Layer | Asset | Time to Replicate by Competitor | Evidence |
|-------|-------|-------------------------------|----------|
| 1. Architecture | Agent-native, SOP-driven decision engine | 6-12 months | "Engineering effort" [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8.3] |
| 2. Basic rule sets | Insurer rules, convention mappings | 3-6 months | "Public info + manual work" [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8.3] |
| 3. Deep workflow knowledge | Carrier-specific SOP implementations, edge cases, exception handling | 12-24 months | "Requires field work" [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8.3] |
| 4. Enforcement patterns | What actually gets denied/approved vs. what the contract says | 2-5 years | "Requires claim volume" [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8.3] |
| 5. Cross-carrier learnings | Anonymized patterns across multiple carriers | 3-5 years | "Requires network scale" [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8.3] |

**The stacking effect:** A competitor entering the market today faces 6-12 months to build the architecture, then 3-6 more months for basic rules, then 12-24 more months for deep knowledge, then 2-5 more years for enforcement patterns. By the time they have what Mysa has today, Mysa will have 3-5 additional years of cross-carrier network effects.

### Cross-Carrier Learning: The Network Effect

The most powerful long-term moat is cross-carrier learning. This is where Mysa transcends being a per-carrier tool and becomes a platform with true network effects.

**How it works:**

```
Carrier A (Portugal, motor):
  Claims processed through Mysa
  Decision patterns captured
  |
  v
Anonymization layer:
  - Remove all PII
  - Remove carrier identity
  - Normalize monetary amounts to % of category average
  - Apply k-anonymity (k >= 5)
  |
  v
Aggregate pattern library:
  "Portuguese motor carriers, EUR 100-200M tier, water damage claims:
   - 73% approve on first review
   - 18% require additional documentation
   - 9% deny (top reasons: pre-existing damage, policy exclusion)
   - Average reserve: 112% of initial estimate
   - Fraud signal false positive rate: 14%"
  |
  v
Carrier B (Spain, motor) onboards Mysa:
  Before processing a single claim,
  Carrier B gets aggregate intelligence from Portuguese carriers
  Cold start is warmer because the network has data
```

[SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Section 7.3 -- "Knowledge flows ACROSS clinics (anonymized): Denial patterns, Successful fixes, Enforcement quirks, Gray area resolutions"]

**Why this creates a defensible network effect:**

| Network Effect Mechanism | How It Works | Defensive Value |
|------------------------|-------------|----------------|
| **More carriers = better aggregate intelligence** | Each new carrier adds decision patterns to the anonymized corpus. New carriers get a warmer cold start. | Competitors with fewer carriers have worse aggregate intelligence. |
| **More claims/carrier = faster flywheel** | Higher-volume carriers generate ground truth faster, improving models that benefit all carriers. | First-mover carriers with high volume set the pace. |
| **Cross-country patterns** | A coverage pattern learned in Portuguese motor claims may apply in Spanish motor claims (similar convention systems). | Competitors limited to a single market cannot learn cross-country patterns. |
| **Cross-line patterns** | Fraud signals learned in motor claims may apply in property claims (same claimant behavior patterns). | Competitors limited to a single line of business miss cross-line intelligence. |
| **Self-reinforcing adoption** | Better aggregate intelligence = better out-of-box accuracy for new carriers = easier sales = more carriers = better aggregate intelligence. | The flywheel feeds itself. Classic network effect. |

### Why the Moat Compounds Over Time

The critical investor insight: Mysa's moat is not static -- it accelerates.

**Year 1: Weak moat (replicable)**
- SOP encoding for 3-5 carriers
- Historical data ingestion
- Basic convention system matching
- A competitor with good engineers could replicate this

**Year 2: Moderate moat (defensible)**
- 12+ months of decision ground truth per carrier
- Enforcement patterns beginning to emerge
- Carrier-specific predictive models
- A competitor would need 12-18 months to reach this point

**Year 3: Strong moat (prohibitive to replicate)**
- 20-50 carriers across 4+ countries
- Cross-carrier network effects active
- Predictive models accurate enough for near-STP on routine claims
- Convention system expertise across IDS, CIDE, IRSA, CARD
- A competitor would need 2-3 years AND equivalent carrier count

**Year 5: Dominant moat (structural advantage)**
- Hundreds of carriers
- Cross-country, cross-line pattern library
- Property + motor decision intelligence
- EU + US data
- Decision reasoning corpus with millions of annotated decisions
- This is a new category of data asset. It does not exist anywhere else in the world.

[SOURCE: mysa_product_strategy.md, Part 1 -- "better data -> better recommendations -> more trust -> more data"; Part 4e -- "Historical data engine: Core moat"; AI_NATIVE_ARCHITECTURE_SPEC.md, Section 8 -- competitive moat analysis]

### The Exit Argument

For investors, the data moat has a specific implication for exit strategy:

> "We start with a simple, provable product -- EAS digitization for EU motor. This builds our OCR + document AI + decision logic capabilities. We expand to property coverage AI -- the same technology applied to a bigger problem. We capture decision ground truth data from every adjuster interaction. Over time, our models get smarter, and the gap between Mysa (carrier-specific, SOP-driven, decision-focused) and generic copilots (broad, template-based, task-focused) widens."
> [SOURCE: mysa_product_strategy.md, final summary]

The data flywheel creates increasing returns to scale. A Mysa with 100 carriers is not just 10x more valuable than a Mysa with 10 carriers -- it is exponentially more valuable because of cross-carrier learning, richer aggregate patterns, and faster model improvement for every new carrier.

CCC acquired EvolutionIQ for $730M [SOURCE: mysa_product_strategy.md, Part 4d] -- an AI claims guidance company for auto casualty with outcome prediction data. Mysa's decision reasoning data is a more fundamental asset than outcome prediction because it captures the process, not just the result. The acquirer (whether a CCC, Verisk, Guidewire, or strategic buyer) would be buying not just a product but an entirely new data category.

---

## Sources

| Source | Type | Sections Used |
|--------|------|--------------|
| `mysa_product_strategy.md` Parts 1, 3a, 4a-4e, 5a-5d, 6b, 9b-9c | Primary -- flywheel, moat, competitive analysis, product architecture, market sizing | 8.1-8.7 |
| `AI_NATIVE_ARCHITECTURE_SPEC.md` Sections 5, 7, 8 | Primary -- knowledge layer, feedback loops, competitive moat | 8.1, 8.2, 8.4, 8.5, 8.7 |
| `CARAVELA-COMPETITIVE-ASSESSMENT-2026-02-07.md` Sections 4, 7, 8 | Primary -- OCR accuracy, annotation data, dataset growth strategy | 8.4 |
| `DATA_SOURCES.md` | Secondary -- data source inventory, ADSE/ICD-10 references | 8.3 |
| `REGULATORY_COMPLIANCE.md` | Secondary -- GDPR/RGPD requirements, appeal timelines | 8.5 |
| `MODULE_01_POSITIONING.md` Sections 1.1, 1.2, 1.4 | Context -- positioning, ICP, value proposition | 8.1, 8.6 |
| Feb 7, 2026 Granola call -- Restaurant metaphor, historical data, mid-market strategy | Transcript | 8.1, 8.2, 8.4 |
| Feb 7, 2026 Granola call -- Xactimate integration, flywheel accuracy | Transcript | 8.2, 8.3 |
| Feb 8, 2026 Granola call -- Strategy review, accuracy targets | Transcript | 8.4 |
| Feb 9, 2026 Granola call -- Claims workflow, EU vs US, SOP encoding | Transcript | 8.5, 8.6 |
| EU AI Act (Regulation 2024/1689), Annex III | Legal -- high-risk AI classification | 8.5 |
| GDPR (Regulation 2016/679), Articles 6, 9, 22, 25, 28, 33, 35 | Legal -- data processing, automated decisions, DPAs | 8.5 |
| `caravela-ocr.md` (memory file) | Internal -- current accuracy metrics | 8.4 |

---

# Part 9: Go-to-Market

# Module 9: Go-to-Market

**Status:** DRAFT v1.0
**Last updated:** February 9, 2026
**Feeds:** Pitch deck slides 10-11, fundraising narrative, sales playbook, investor Q&A, partnership strategy

---

## 9.1 Why This Rollout Order

Mysa's go-to-market is a five-phase expansion built on a single principle: **each phase creates the precondition for the next.** This is not a geographic wishlist. It is a sequence where every step reduces the risk of the step that follows.

### The Logic Chain

```
Smallest market (Portugal)
  --> fastest feedback loops, fewest edge cases, prove the product works
    --> convention expertise (CIMPAS/IDS) becomes a transferable technical wedge
      --> design partner (Caravela) produces live metrics and an LOI
        --> Southern EU motor (Spain, France, Italy) shares the same convention architecture
          --> same carriers write property (80-95% overlap) = upsell, not new acquisition
            --> Northern EU expands the same playbook to larger markets
              --> US entry leverages proven product on the biggest TAM
```

**Step 1 -- Smallest market = fastest feedback.** Portugal has ~25-30 motor writers and ~47 active non-life insurers. The IDS/CIMPAS convention system covers ~100% of the market with a 91% inter-insurer agreement rate. This means fewer edge cases, faster iteration, and a controlled environment to prove that OCR + convention matching + decision support works in production. You cannot debug a product across 660 French insurers. You can debug it across 25 Portuguese motor writers.

**Step 2 -- Convention expertise = technical wedge.** Once Mysa encodes CIMPAS/IDS, the same architecture transfers to CIDE (Spain), IRSA (France), and CARD (Italy). Each convention system is different in specifics but identical in structure: standardized accident data in, deterministic fault determination out. The technical work of building the first convention system is 80% of the work for all of them. No competitor has built any of them.

**Step 3 -- Design partner = proof.** Caravela is not a customer. It is a design partner that gives Mysa live data, real adjuster workflows, and measurable STP improvement. The output is not revenue -- it is an LOI, benchmark metrics, and a case study that opens every subsequent sales conversation in Europe.

**Step 4 -- Same buyers = expansion.** The VP Claims at a Portuguese motor carrier is the same persona as the VP Claims at a Spanish motor carrier, a French motor carrier, or an Italian motor carrier. The SOPs differ. The convention system differs. The decision problem is identical: coverage, liability, reserves, fraud. Mysa sells the same product with a different convention module.

**Step 5 -- Same carriers = property upsell.** 80-95% of carriers that write motor also write property. The adjuster workflow is ~80% identical (same 6 decision sub-steps). Property adds +60-70% revenue per carrier at zero new customer acquisition cost. This is the move that turns a wedge TAM into a venture-scale TAM.

---

## 9.2 Phase 1: Portugal (Caravela)

### Why Portugal First

| Factor | Detail |
|--------|--------|
| **Co-founder network** | Tiago has practitioner-level relationships in Portuguese insurance. Caravela is the design partner -- not a cold outreach target. |
| **Smallest Southern EU market** | ~€1.8B motor GWP, ~5.8M light vehicles, ~25-30 motor writers, 47 active non-life insurers. Small enough to learn fast, large enough to prove the product. |
| **Best-performing convention system** | IDS/CIMPAS has a 91% inter-insurer agreement rate and 1.94-day average decision time. This is the cleanest convention data in the EU -- the ideal first test case. |
| **Standardized forms** | Portuguese EAS (European Accident Statement) forms are well-documented and standardized. Caravela's OCR engine already processes them at 81.5% normalized accuracy. |

### The Design Partner: Caravela Seguros

| Metric | Value |
|--------|-------|
| GWP (2024) | **€188M** |
| Employees | 149 |
| Total claims/year | **~57K** (42K motor + ~15K property) |
| Portuguese non-life ranking | 7th |
| Growth trajectory | 10x in 10 years |
| Property growth | +31% (fastest-growing line) |
| Data science team | **None** -- cannot build in-house |

Caravela is the archetype of the Mysa buyer: large enough to have real claims volume (57K/year), small enough to lack a data science team (149 employees), growing too fast to scale with headcount alone (10x in a decade), and operationally sophisticated enough to know they need technology.

### The Commercial Motion

> "I want an LOI [from Caravela], and we say we're doing it in free beta tester. For six months. This is the cost."
> -- Jeremy Blehaut [TRANSCRIPT: Feb 7, 2026]

**Timeline:**

| Step | Duration | Output |
|------|----------|--------|
| Free beta | 6 months | Weekly syncs, live claims processing, STP rate measurement, adjuster feedback |
| LOI conversion | Month 6 | Letter of Intent with pricing commitment |
| Paid contract | Month 7+ | €50K-€100K/year (design partner rate -- discounted from standard €100K-€200K Professional tier) |

**Success metric:** Process 100+ Portuguese motor claims through the full pipeline. Measure STP rate improvement vs Caravela's baseline (~10% today, target 40-50%).

### Adjacent Portuguese Targets

Once Caravela is live, Mysa has a case study for the rest of the Portuguese mid-market:

| Carrier | Est. GWP | Notes |
|---------|----------|-------|
| CA Seguros | ~€200-210M | 8th in non-life, displaced by Caravela |
| Mapfre PT | ~€190-210M | 9th, surge with Bankinter partnership |
| Aegon Santander | ~€170-190M | 10th |
| Victoria | ~€130-150M | 11th, strong in health |
| UNA | ~€120-140M | 12th, motor +26% growth |

**Target for Phase 1:** Caravela live + 2-4 additional Portuguese mid-market carriers in pipeline by month 6.

### The ROI Case (Caravela-Specific)

Caravela processes ~42K motor claims/year. At an STP improvement from 10% to 40-50%:
- 12,600-16,800 additional claims processed with minimal human intervention
- At ~45 min saved per claim = 9,450-12,600 hours saved/year
- At €50/hour loaded cost = **€472K-€630K saved/year**
- Mysa charges €50K-€100K/year (design partner rate) = **5-12x ROI**

---

## 9.3 Phase 2: Southern EU Motor

### Why Southern EU Second

Southern EU motor markets (Spain, France, Italy) share three properties that make them the natural second step after Portugal:

1. **Convention system transferability.** Spain (CIDE/ASCIDE/CICOS), France (IRSA), and Italy (CARD) all use structured convention systems for motor claims. Mysa's convention matching architecture -- built for CIMPAS in Phase 1 -- transfers directly. The data models differ, the engineering pattern is the same.

2. **Same ICP.** Mid-market carriers in Spain, France, and Italy look like Caravela: €100-200M GWP, 100-300 employees, no data science team, buying not building. The VP Claims buyer has the same pain points, the same budget range, the same 1-2 decision-maker purchasing process.

3. **Massive combined TAM.** Southern EU motor is €57.9B in GWP with 54-93 carriers in the Caravela tier (€100-200M) and 141-159+ in the small tier (€50-100M). This is where the wedge becomes a real business.

### Country-by-Country

#### Spain -- CIDE/ASCIDE/CICOS

| Metric | Value |
|--------|-------|
| Motor GWP | **€13.2B** (2024, +8.9% YoY) |
| Insured vehicles | 34M |
| Total operating insurers | 176 (187 RAEA-registered) |
| Motor writers | ~80-100 |
| Caravela-tier carriers (€100-200M) | **8-10** |
| Small-tier carriers (€50-100M) | **25-35** |
| Convention | CIDE/ASCIDE/CICOS -- Tabla de Culpabilidad (fault table) + CICOS digital platform |
| Convention volume | **2.5M claims/year processed via CICOS** |

**Why Spain second (not France):** Largest convention claim volume in Southern EU (2.5M/year via CICOS). The CICOS digital platform already exists -- Mysa integrates with it rather than replacing it. Language proximity to Portugal. And the Caravela case study translates directly: "We improved STP by 30 points at a Portuguese carrier your size."

**Named carrier targets:**

| Carrier | Est. GWP | Notes |
|---------|----------|-------|
| Pelayo | ~€375M (mutua) | 844K auto policies, 2.42% motor share. Mutual structure = independent buyer. |
| Admiral/Balumba | ~€100-150M motor | UK-owned direct writer, +13.4% growth. Tech-forward. |
| Patria Hispana | ~€100-130M | Centennial company, +12.9% growth. Traditional but growing. |
| Mutua Tinerfena | ~€80-120M | Regional Canary Islands mutual. Independent decision-maker. |
| Linea Directa | €200M+ | Slightly above Caravela tier but buy-not-build profile. |

**Competition note:** Bdeo has 7-8 of the top 10 Spanish auto insurers -- but Bdeo is visual AI (photo/video damage assessment), not decision support. Bdeo and Mysa occupy different layers of the stack. Potential integration partner, not competitor.

**Target:** 5-10 Spanish mid-market carriers by month 9.

#### France -- IRSA

| Metric | Value |
|--------|-------|
| Motor GWP | **€28.1B** (2024, +7.3% YoY) |
| Insured vehicles | 45.5M |
| Total ACPR-supervised organizations | **660** (246 FFA members) |
| Motor writers | ~100-120 |
| Caravela-tier carriers (€100-200M) | **30-60** |
| Small-tier carriers (€50-100M) | **100+** |
| Convention | IRSA -- 13 standardized cases, outputs only 0%, 50%, or 100% fault |
| Convention volume | ~80% of material motor claims; **7.4M total claims/year** |

**Why France is the biggest opportunity in Phase 2:** France has the largest absolute count of Caravela-tier carriers in Southern EU (30-60 in the €100-200M range, plus 100+ in the €50-100M range). Most are autonomous mutuelles -- independent entities with their own claims operations and purchasing authority. The IRSA convention is the simplest fault model in Europe (13 cases, deterministic output). And France's motor claims costs rose 4.3% in 2024, creating cost-reduction urgency.

**Named carrier targets:**

| Carrier | Est. GWP | Notes |
|---------|----------|-------|
| Thelem Assurances | €453M total (~€150-200M motor) | 1.15M contracts. **Closest French analog to Caravela.** |
| L'Olivier Assurance | ~€220-260M | Online auto pure-play. Tech-native buyer. |
| Direct Assurance (AXA sub) | ~€300-400M | Slightly larger. Subsidiary = faster procurement than parent. |
| ~30-60 small mutuelles | €82-200M each | ACPR 2nd quartile. Many are autonomous, multi-line with motor books. Independent buyers. |

**Target:** 5-15 French carriers by month 12.

#### Italy -- CARD

| Metric | Value |
|--------|-------|
| Motor GWP | **~€14.8B** (2023) |
| Insured vehicles | ~40M |
| Total insurers | ~85 national (IVASS-registered) |
| RC Auto writers | **38** |
| Caravela-tier carriers (€100-200M) | **10-15** |
| Small-tier carriers (€50-100M) | **8-12** |
| Convention | CARD -- mandatory for 2-vehicle claims, <9% permanent disability |
| Convention volume | **2M claims paid**, avg €2,105/claim (+4.2%) |

**Why Italy is the highest-pain market:** The CARD convention is mandatory and the most complex in Southern EU (civil code + CAI form). Italian carriers have the highest willingness to pay for tools that reduce convention processing friction. UnipolSai dominates, but below the top 3, the market is fragmented among mid-market players.

**Named carrier targets:**

| Carrier | Est. GWP | Notes |
|---------|----------|-------|
| HDI Assicurazioni | €716M non-life (~€160-200M motor) | Closest Italian analog to Caravela. |
| Prima Assicurazioni | €50-200M motor | Online insurer, tech-forward. |
| Quixa (AXA sub) | €50-200M motor | Digital-first, subsidiary procurement. |
| Verti (MAPFRE sub) | €50-200M motor | Digital-first. |
| Linear (UnipolSai sub) | €50-200M motor | Digital-first subsidiary. |

**Target:** 5-10 Italian carriers by month 12.

### Phase 2 Combined Targets

| Country | Caravela-Tier (€100-200M) | Small (€50-100M) | Total Target Carriers |
|---------|--------------------------|-------------------|-----------------------|
| Spain | 8-10 | 25-35 | **~33-45** |
| France | 30-60 | 100+ | **~130-160+** |
| Italy | 10-15 | 8-12 | **~18-27** |
| **Southern EU (excl. Portugal)** | **48-85** | **133-147+** | **~181-232+** |

**Revenue target for Phase 2:** 15-25 paying carriers across Southern EU, €750K-€2.5M ARR (Professional tier average: €100K-€150K/year).

---

## 9.4 Phase 3: Property (Same Buyers)

### Why Property Before Northern EU

The conventional startup playbook says "expand geographically, then add product lines." Mysa reverses this. **Property comes before Northern EU expansion** because it is an upsell, not a new sale.

### The Same-Buyer Argument

**80-95% of carriers that write motor also write property.** This is validated across all 16 EU countries and the US. At a Caravela-tier carrier, the VP Claims who bought Mysa for motor also owns property claims. The CFO who approved the motor budget approves the property budget. The adjusters who use Mysa for motor often handle property claims too.

| Dimension | Motor | Property | Overlap |
|-----------|-------|----------|---------|
| Buyer persona | VP Claims / CCO | VP Claims / CCO | **Same person** |
| Budget authority | Claims operations | Claims operations | **Same budget** |
| Decision sub-steps | 6 (coverage, policy, repair, cost, reserve, fraud) | 6 (coverage, policy, repair, cost, reserve, fraud) | **Same framework** |
| Adjuster workflow | Intake, structure, triage, investigate, decide, document | Intake, structure, triage, investigate, decide, document | **~80% identical** |
| Core difference | Convention system matching (who is at fault?) | Coverage determination (is this covered?) | **One module swap** |

### What Changes for Property

The decision engine architecture stays the same. The 6 sub-steps stay the same. What changes is one module: instead of convention system matching (deterministic fault lookup), property requires **coverage determination** (policy interpretation + causation analysis).

**Convention matching (motor):** Read EAS data, match against CIMPAS/IRSA/CARD/CIDE rules, output fault percentage. Deterministic. Solved problem once data is clean.

**Coverage determination (property):** Read policy document, match claim facts against coverage clauses and exclusions, determine "is this covered?" Requires interpreting "sudden vs gradual" for water damage, "named peril vs open peril" for storm claims, concurrent causation doctrine. This is harder -- and the competitive landscape is emptier.

### The Revenue Math

Adding property to existing motor customers:

| Scenario | Motor-Only TAM | Motor + Property TAM | **Uplift** |
|----------|---------------|---------------------|------------|
| EU mid-market only | €50-100M | €80-170M | **+60-70%** |
| EU + US mid-market | €100-250M | €160-425M | **+60-70%** |
| Full addressable | €200-650M | €320M-1.1B | **+60-70%** |

**+60-70% revenue uplift at zero new customer acquisition cost.** This is the single most capital-efficient move in Mysa's roadmap.

### Property Market by Geography

#### Southern EU Property

| Country | Property GWP | Claims/Year | Dominant Peril | Carrier Overlap with Motor |
|---------|-------------|------------|----------------|---------------------------|
| Portugal | ~€0.44B (Multirriscos) | ~200-300K est. | Wildfires, storms | Very high |
| Spain | **€6.1B** (Hogar) | **~4M+** | **Water damage (38.2%)** | Very high |
| France | **€13.8B** (MRH) | **4.6M** | **Water damage (44%)** | Very high |
| Italy | ~€3.5-4.0B | ~1-2M | Earthquakes, floods | Very high |
| **Total** | **~€24-28B** | **~10-12M** | | |

**Water damage is the "fender bender" of property.** 38-44% of all home claims in Spain and France are water damage. Highly repetitive, standardizable, and frequent enough to generate training data fast. Water damage is to property what two-car collisions are to motor -- the volume play where AI decision support has the highest ROI.

#### Property Decision AI -- The Empty Competitive Landscape

$3B+ has been invested in the physical side of property claims (photos, measurements, materials, estimation). Almost zero in the intellectual side (is this covered? what caused it? what does the policy say?).

| Company | What They Do | Funding | Decision Support? |
|---------|-------------|---------|------------------|
| Hover | 3D property from smartphone photos | $142M | NO -- measurement only |
| EagleView | Aerial imagery, roof models | ~$2.8B (PE) | NO -- visual data only |
| Nearmap (+ itel) | Aerial imagery + material pricing | $730M (Thoma Bravo) | NO -- estimation data |
| CAPE Analytics | Geospatial AI property risk | $75M (acquired by Moody's) | NO -- underwriting only |
| ZestyAI | Property risk intelligence | $50M | NO -- underwriting only |
| Xactimate/XactAI | Estimation + admin AI | Public (Verisk $40B+) | NO -- estimation efficiency |
| **Crawford CoverAI** | Policy interpretation | Corporate | **Closest -- but reabsorbed into Crawford TPA, no causation analysis** |
| **Wamy** | Claims AI workforce | Undisclosed | **Brand new (Dec 2025), pre-traction** |

Coverage determination AI is virtually empty. Nobody is building AI that determines "is this water damage covered? Was this sudden or gradual?" Mysa enters this space with the same decision engine architecture proven on motor, the same carrier relationships, and no meaningful competition.

### Phase 3 Target

- Upsell property module to 10-15 existing motor customers
- First property-specific pilots with carriers where property is the larger line (French multi-line mutuelles)
- Water damage claims as the initial property use case (highest frequency, most standardizable)

---

## 9.5 Phase 4: Northern EU

### Why Northern EU After Property

Northern EU motor is a larger premium market than Southern EU (€70-78B vs €57.9B) but has fewer mid-market carriers in the Caravela tier and a more mixed convention landscape. Entering Northern EU requires:

1. Convention expertise from 3-4 Southern EU systems (built in Phases 1-2)
2. A proven product with measurable results (built from Caravela + Southern EU customers)
3. Property capability (built in Phase 3) -- because Northern EU carriers write both lines and will expect a multi-line product

Going to Northern EU before having property capability means selling a motor-only tool to carriers that process both motor and property claims. Going after property means selling a complete decision engine.

### The Northern EU Landscape

| Country | Motor GWP | Convention-Like System? | Caravela-Tier (€100-200M) | Small (€50-100M) |
|---------|----------|------------------------|--------------------------|-------------------|
| **Germany** | **~€30B** | Teilungsabkommen (bilateral only, not standardized) | **15-25** | **20-35** |
| Netherlands | ~€5.9-6.2B | DSA (new, launched 2024) | 3-5 | 5-8 |
| Belgium | ~€4.3-4.5B | RDR (Convention Reglement Direct) | 5-8 | 8-12 |
| Austria | ~€4.3B | None formal | 2-4 | 3-5 |
| Switzerland | ~€7.2-8.2B | None formal | 3-5 | 5-8 |
| Ireland | ~€1.3B | None | 2-4 | 3-5 |
| Sweden | ~€2.6-2.9B | Trafikskadenamnden | 3-4 | 4-6 |
| Denmark | ~€2.0-2.4B | None formal | 2-3 | 3-5 |
| Finland | ~€1.2-1.4B | Traffic Insurance Centre | 2-3 | 2-3 |
| Norway | ~€2.7-2.8B | None formal | 2-3 | 3-4 |
| Poland | ~€6.5B | UFG coordination | 3-5 | 4-6 |
| Czech Republic | ~€2.1-2.3B | None formal | 2-3 | 3-4 |
| **Total** | **~€70-78B** | | **~42-72** | **~63-101** |

### Germany: The Prize

Germany is the single largest motor market in Europe (~€30B GWP) with 15-25 Caravela-tier carriers and 20-35 small-tier carriers. It is also the largest EU property market (~€15.5-17B property GWP). Germany alone represents a meaningful expansion of Mysa's addressable market.

**Germany does not have a standardized convention system.** The Teilungsabkommen are bilateral agreements between individual insurers, not an industry-wide protocol like CIMPAS or IRSA. This means Mysa's convention matching wedge is weaker in Germany. But by Phase 4, Mysa's value proposition has evolved beyond convention matching into a full decision engine with SOP-driven workflows, coverage determination, reserve recommendation, and fraud detection. The convention module becomes one feature, not the entire product.

### Markets with Convention-Like Systems (Partial Wedge)

| Country | System | Similarity to Southern EU Conventions |
|---------|--------|--------------------------------------|
| Belgium | RDR (Convention Reglement Direct) | High -- direct compensation protocol similar to IDS |
| Netherlands | DSA (Direct Settlement Agreement, launched 2024) | Medium-High -- new system, carriers adapting, Mysa can help |
| Sweden | Trafikskadenamnden (Traffic Damage Board) | Medium -- advisory body, not binding rules |
| Finland | Traffic Insurance Centre | Medium -- coordination mechanism |

Belgium and the Netherlands represent a partial wedge: their convention-like systems mean Mysa can lead with convention matching expertise (like Southern EU) rather than requiring the full decision engine sell.

### Markets Without Convention Systems (General Decision Engine Sell)

Austria, Switzerland, Ireland, Denmark, Norway, Czech Republic -- and to a large extent Germany -- have no standardized convention system. In these markets, Mysa sells on the general decision engine value proposition: SOP-driven workflows, coverage determination, reserve accuracy, adjuster productivity. The convention wedge is absent. Product-market fit proven in Southern EU + property capability must carry the sale.

### Northern EU Property Opportunity

Northern EU property is a massive market with high carrier overlap:

| Country | Property GWP | Motor/Property Carrier Overlap |
|---------|-------------|-------------------------------|
| Germany | ~€15.5-17B | Very high (except HUK-Coburg motor-only) |
| Netherlands | ~€4.5-5.5B | Very high |
| Belgium | ~€2.4-2.5B | Very high |
| Sweden | ~€3.5-4.0B | Very high |
| Norway | ~€2.5-3.0B | Very high |
| Denmark | ~€3.0-3.5B | Very high |
| **Total** | **~€30-33B** | |

Germany's property market is particularly compelling: profitable only 4 of the last 20+ years, water damage costs exceeding €4.5B/year, and a growing cat exposure from climate change. German carriers need claims efficiency tools for property.

### Phase 4 Target

- Enter 3-4 Northern EU markets simultaneously (Germany + Benelux as priority)
- 10-20 carriers across Northern EU by end of Phase 4
- Motor + property from day one in each market (no motor-only Phase 1 repeat)

---

## 9.6 Phase 5: US Mid-market

### Why US Last

The US market is the largest insurance market in the world (~$1.06T total P&C DWP). It is also the most competitive, the most concentrated in auto, and the most different from the EU in terms of claims architecture. Entering the US last is not a concession -- it is a strategic sequence.

### The US Challenges

| Challenge | Detail |
|-----------|--------|
| **No convention system** | US motor and property claims have no equivalent of CIMPAS/IRSA/CARD/CIDE. The convention wedge does not apply. |
| **Auto is extremely concentrated** | Top 5 US auto insurers = 63.6% market share (GEICO, Progressive, State Farm, Allstate, USAA). Mid-market auto opportunity is limited. |
| **50-state regulatory variation** | Each state has different insurance regulations, coverage requirements, and claims rules. Supporting all 50 states is a multi-year effort. |
| **Entrenched estimation monopoly** | Verisk/Xactimate owns ~80% of US property estimation. CCC/Mitchell dominate auto. Integration is mandatory, not optional. |
| **More competitor activity** | Five Sigma (70% US), Hi Marley, Assured, FurtherAI, Avallon -- US has more funded claims AI companies than EU. |

### Why US Property First (Not Auto)

| Dimension | US Auto | US Homeowners |
|-----------|---------|---------------|
| Market size | $359B DWP | $172.7B DWP |
| Top 5 concentration | **63.6%** (extremely concentrated) | **45.7%** (less concentrated) |
| Mid-market carriers ($100-500M) | Limited -- big 5 dominate | **~60-80 carriers** |
| Claims/year | ~35M | ~4.4-4.5M |
| Average claim size | ~$5,000 | **$17,059** (3.4x auto) |
| Decision complexity | Lower (fault determination) | Higher (coverage + causation) |
| Mysa advantage | Low -- no convention wedge, concentrated market | **High -- coverage determination is Mysa's core capability by Phase 5** |

US homeowners is less concentrated than auto, has larger average claim sizes (higher per-claim pricing opportunity), and the core decision problem (coverage determination, causation analysis) is exactly what Mysa built for EU property in Phase 3. The product transfers directly.

### The TPA Channel

The US market has a buyer segment that barely exists in Europe: **Third-Party Administrators (TPAs).**

| Buyer Type | Count (Material Size) | Why They Buy |
|-----------|----------------------|-------------|
| P&C-focused TPAs | ~500-800 | Process claims for carriers. Adjuster shortage + leakage pressure. Budget for per-claim tools. |
| MGAs with claims authority | ~330-550 | Fastest-growing segment (16% CAGR). Need claims tech but have no legacy systems. |
| Independent adjusting firms | ~53,000 businesses ($11.7B market) | Workforce is their product -- augmentation = survival. |

TPAs are a distribution channel. A TPA that adopts Mysa processes claims for multiple carriers -- each carrier becomes a potential direct customer. And TPAs prefer per-claim pricing (low barrier, pay-as-you-go), which is Mysa's landing pricing model.

### Named US Mid-Market Targets

| Carrier | DWP | Notes |
|---------|-----|-------|
| Erie Insurance | ~$3.3B total | Tech-forward, invested in AI startups. Strong in homeowners. |
| Cincinnati Financial | ~$1.6B | Multi-line, mid-market profile despite size. |
| Amica Mutual | ~$1.2B | "AI Trailblazer" -- partnered with ZestyAI. Open to claims AI. |
| Donegal Insurance Group | $100-500M | Classic Caravela-tier US analog. |
| Secura Insurance | $100-500M | Midwest regional, buy-not-build. |
| Shelter Insurance | $100-500M | Midwest mutual, independent buyer. |
| Westfield Insurance | $100-500M | Multi-line, tech-interested. |
| State farm bureaus (KY, NC, TX) | Varies | Independent entities despite "farm bureau" name. |
| Hippo (insurtech) | Growing | Digital-native, needs claims efficiency as they scale. |
| Kin (insurtech) | Growing | Homeowners-focused insurtech, high claims tech openness. |
| SageSure (MGA) | Growing | MGA with claims authority, fast-growing. |

### The US Sell: General Decision Engine

Without the convention wedge, Mysa sells in the US on:

1. **Coverage determination** -- "sudden vs gradual" for water damage, "named peril vs open peril" for storm claims. Built and proven on EU property in Phase 3.
2. **SOP-driven workflows** -- encode each carrier's or TPA's procedures into AI-guided decision flows.
3. **Reserve accuracy** -- AI-calculated reserves with P&L impact. CFO-level selling point.
4. **Adjuster productivity** -- 3x claims handled per adjuster. Same value proposition as EU.
5. **Xactimate integration** -- works with the estimation tool that 80% of US property adjusters already use.

### Phase 5 Target

- 3-5 US pilot customers (mid-market carriers or TPAs), property-first
- First US revenue by month 12-14
- TPA channel as primary distribution strategy
- Xactimate integration as non-negotiable prerequisite

---

## 9.7 Why Motor + Property Together

### The Structural Argument

Motor and property are not two different products. They are two configurations of the same product.

| Component | Motor | Property | Shared? |
|-----------|-------|----------|---------|
| Intake parsing (OCR, email, documents) | EAS forms, repair estimates, photos | Claim forms, contractor estimates, photos | **YES -- same engine** |
| Data structuring | Structured claim data fields | Structured claim data fields | **YES -- same engine** |
| Triage | Complexity scoring, desk vs field routing | Complexity scoring, desk vs field routing | **YES -- same engine** |
| Investigation support | Call recording, guided investigation, document gen | Call recording, guided investigation, document gen | **YES -- same engine** |
| **Decision: liability/fault** | **Convention matching (CIMPAS/IRSA/CARD/CIDE)** | **Not applicable** | **MOTOR ONLY** |
| **Decision: coverage** | Basic (policy check) | **Complex (coverage determination + causation)** | **PROPERTY MODULE** |
| Cost analysis | Audatex/Solera (EU), CCC/Mitchell (US) | Xactimate (US), fragmented (EU) | Different integrations, same logic |
| Reserve calculation | Historical comparables, P&L impact | Historical comparables, P&L impact | **YES -- same engine** |
| Fraud detection | Pattern matching, red flags | Pattern matching, red flags | **YES -- same engine** |
| Document generation | Per SOP, per decision | Per SOP, per decision | **YES -- same engine** |
| SOP compliance | Carrier-specific rules | Carrier-specific rules | **YES -- same engine** |

**~80% of the adjuster workflow is identical between motor and property.** The difference is one module: convention matching (motor) vs coverage determination (property). Everything else -- intake, triage, investigation, reserves, fraud, documents, SOP compliance -- is the same.

### The Persona Argument

The same three personas buy and use Mysa for both lines:

- **Adjuster** uses Mysa for motor claims Monday, property claims Tuesday. Same interface, different modules.
- **VP Claims** buys Mysa for motor. Six months later, asks "can we use this for property too?" The answer is yes, same platform, add one module.
- **CFO** sees reserve accuracy improvement on motor. Wants the same improvement on property. Same P&L dashboard, same reserve models, different claim types.

### The Buyer Argument

80-95% carrier overlap means the expansion motion is:

1. Land with motor (convention wedge in EU, general decision engine in US)
2. Prove value on motor claims (STP improvement, reserve accuracy, adjuster productivity)
3. Expand to property claims at the same carrier (same buyer, same budget, same platform)
4. Revenue per carrier increases 60-70% with no new customer acquisition cost

This is land-and-expand at its most efficient: same buyer, same platform, same adjuster, different claim type.

---

## 9.8 Why EU Then US

### The Convention System Wedge

Convention systems are Mysa's single greatest competitive advantage in the first 12-18 months. They exist only in Europe. They require deep, country-specific domain knowledge to encode. No US-based competitor has built them or has any reason to.

| Convention | Country | What It Does | Why It Matters for Mysa |
|-----------|---------|-------------|------------------------|
| IDS/CIMPAS | Portugal | Direct compensation protocol, 91% agreement rate | Fastest to build, cleanest data, design partner |
| CIDE/ASCIDE/CICOS | Spain | Fault table + digital platform, 2.5M claims/year | Largest volume, existing digital infrastructure |
| IRSA | France | 13 standardized cases, deterministic fault (0/50/100%) | Simplest model, largest market |
| CARD | Italy | Mandatory for 2-vehicle claims, complex civil code | Highest pain = highest willingness to pay |

Building convention matching takes deep insurance domain expertise + country-specific regulatory knowledge + technical execution. This combination is rare. Once built, it creates a defensible moat: a competitor entering EU motor must invest 12-18 months replicating what Mysa already has.

### The Fragmented Mid-Market

The EU mid-market is more fragmented than the US mid-market. This is an advantage for a startup.

| Metric | EU (16 countries) | US |
|--------|-------------------|-----|
| Total carriers | ~2,141+ undertakings | ~4,116 P&C entities |
| Caravela-tier carriers | **~96-165** | ~200-350 |
| Market concentration (top 5) | Varies by country (20-60%) | 51.4% (auto: 63.6%) |
| AI claims tool adoption | **~5-10%** | ~15-25% |
| Mid-market openness | **90-95% untouched** | 75-85% open |

90-95% of EU mid-market carriers have no AI claims tools. The US is more competitive (Five Sigma, Hi Marley, Assured all active). Starting in the EU means selling into a market with less competition, faster sales cycles (1-2 decision-makers), and a unique technical wedge.

### The "Pay First, Recover Later" Architecture

EU insurance operates on a fundamentally simpler claims architecture than the US:

- **EU:** "Pay first, recover later." The insurer pays its own policyholder, then subrogate against the at-fault party's insurer. Claims flow is linear.
- **US:** "Deny then defend." The insurer may deny the claim and let the claimant challenge. Multi-party disputes are common. Litigation-heavy.

The EU architecture is simpler to automate because the decision flow is more predictable: coverage check, convention matching, reserve, pay. The US architecture involves more branching logic: coverage check, investigation, denial possibility, litigation risk assessment, negotiation, settlement. Building the decision engine on the simpler EU architecture first means fewer edge cases, faster iteration, and a more robust product by the time it enters the more complex US market.

### The Design Partner Advantage

Caravela is in Portugal. The co-founder has practitioner-level relationships in Portuguese insurance. This is not replicable in the US. Starting in the EU means starting with a warm design partner relationship that produces real data, real feedback, and a real case study. Starting in the US means cold outreach to carriers in a more competitive market.

### EU Revenue Pays for US Entry

EU revenue from Phases 1-4 funds the US expansion in Phase 5. Mysa does not need to raise additional capital specifically for US entry if EU revenue is on track. The EU business finances its own expansion.

---

## 9.9 Pricing & Channel

### Pricing Philosophy

**Landing:** Per-claim pricing. Low barrier to entry. Carrier pays only for what they use. No upfront commitment. This is how you get a mid-market carrier with a €100K software budget to say yes in 3 months instead of 12.

**Expansion:** Platform pricing. Annual contract. Predictable revenue. This is how you get a carrier that started on per-claim to commit to €100K-€200K/year once they see the ROI.

Most carriers start per-claim and migrate to platform as they scale. This is by design.

> "100% we can get from the tiniest 50K a year for this. And for the biggest 1,000,000."
> -- Jeremy Blehaut [TRANSCRIPT: Feb 7, 2026]

### Pricing Tiers (Anchored to Caravela Economics)

**Reference point:** Caravela (€188M GWP, ~57K claims/year). At €100K/year = 0.05% of GWP. At €3/claim = €171K/year = 0.09% of GWP. Both are trivial relative to the potential savings (€472K-€750K/year from STP improvement alone).

| Tier | Target | # Carriers (4 Southern EU Countries) | Annual Contract | Per-Claim | Est. Claims/Year |
|------|--------|--------------------------------------|----------------|-----------|-----------------|
| **Design Partner** | Caravela (beta) | 1 | Free 6 months, then €50K-€100K/year | N/A | ~57K |
| **Micro** | <€50M GWP | ~100-150 motor writers | €10K-€30K/year | €5-8/claim | ~5-15K |
| **Starter** | €50-100M GWP | ~141-159 | €30K-€100K/year | €3-5/claim | ~15-30K |
| **Professional** | **€100-200M GWP (Caravela tier)** | **~54-93** | **€50K-€200K/year** | **€2-4/claim** | **~30-60K** |
| **Growth** | €200M-€500M GWP | ~20-30 | €200K-€500K/year | €2-3/claim | ~60-150K |
| **Enterprise** | €500M-€1B GWP | ~10-17 | €500K-€2M/year | Custom | ~150K+ |

**Per-claim pricing decreases as volume increases** -- this incentivizes carriers to route more claims through Mysa, which builds the data flywheel faster.

**Property add-on:** +40-60% on the base motor price for carriers that add property. This reflects the +60-70% revenue uplift while giving carriers a multi-line discount incentive.

### US-Specific Pricing

| Buyer | Pricing Model | Range |
|-------|--------------|-------|
| Mid-market carrier ($100-500M DWP) | Platform + per-claim hybrid | $50K-$500K/year |
| TPA | Per-claim (preferred by TPAs) | $3-8/claim (higher than carrier per-claim because TPAs have lower volume per relationship) |
| MGA with claims authority | Per-claim or platform | $30K-$200K/year |

### Channel Strategy

#### Phase 1-3: Direct Sales (EU)

- **Primary channel:** Direct sales by founders (Tiago leads domain conversations, Jeremy leads product demos)
- **Rationale:** Mid-market carriers in EU have 1-2 decision-makers. The sale is consultative, not transactional. Founders understand the product and domain better than any salesperson for the first 15-25 customers.
- **Target:** First 2-3 sales reps hired after 10 paying customers (proof that the sales motion is repeatable)

#### Phase 4-5: Direct + Broker/TPA Channel (EU + US)

- **Direct:** Continue for carriers in the Professional tier and above
- **TPA channel (US):** TPAs process claims for multiple carriers. A TPA that adopts Mysa becomes a distribution partner -- every carrier whose claims they process is exposed to Mysa. This is the primary US distribution strategy.
- **Broker/consultant channel:** Insurance brokers and consultants (Aon, Marsh, WTW at the large end; regional brokers at the mid-market) influence carrier purchasing decisions. Building broker relationships creates inbound pipeline.

#### Insurance Conference Sales Motion

Insurance is a conference-heavy industry. Key events:

| Conference | Geography | Audience | Timing |
|-----------|-----------|---------|--------|
| ITC (InsureTech Connect) | US + EU | Insurtech, carriers, investors | October (Vegas), June (Europe) |
| IICF (Insurance Industry Charitable Foundation) events | US | Carrier executives | Various |
| Insurtech Insights | EU (London) | European insurtech ecosystem | March |
| RIMS | US | Risk managers, large buyers | April |
| National insurance association events per country | EU (per country) | Local carrier executives | Various |

Convention system expertise is a natural conversation starter at European insurance events. "We built the only AI that reads EAS forms and matches against CIMPAS/IRSA/CARD/CIDE" is a demo-worthy hook.

### Revenue Model Summary

```
LANDING (Per-Claim)                    EXPANSION (Platform)
  |                                       |
  | Low barrier                           | Predictable revenue
  | Pay-as-you-go                         | Annual contract
  | 3-month sales cycle                   | Higher ACV
  | Proves ROI on real claims             | Multi-line (motor + property)
  |                                       | SOP encoding = switching costs
  |                                       |
  v                                       v
  Motor claims (convention wedge)  --->   Motor + Property + Full decision engine
  €2-8/claim                              €50K-€2M/year

  CARRIER JOURNEY:

  Trial (per-claim, motor only)
    --> Paid (per-claim, motor)
      --> Platform (annual, motor)
        --> Multi-line (annual, motor + property)
          --> Expansion (annual, motor + property + advanced analytics)
```

---

## Sources

| Source | Type | Sections Used |
|--------|------|--------------|
| `mysa_product_strategy.md` Parts 3c-3f | Primary -- market data, carrier counts, pricing, property analysis | 9.1-9.4, 9.7, 9.9 |
| `mysa_product_strategy.md` Part 6 | Primary -- EU motor first attack, convention systems, rollout | 9.1-9.3, 9.8 |
| `mysa_product_strategy.md` Part 7 | Primary -- product roadmap phases | 9.2-9.6 |
| `mysa_product_strategy.md` Part 9 | Primary -- fundraising narrative, TAM, competitor adoption | 9.3, 9.5, 9.6, 9.8 |
| `market_landscape_overview.md` | Primary -- full market data, carrier profiles, competitive landscape | 9.1-9.9 |
| `INTERNATIONAL_EXPANSION.md` | Secondary -- expansion order, country assessments | 9.3, 9.5 |
| `fos/MODULE_01_POSITIONING.md` | Cross-reference -- ICP, personas, value proposition, carrier segmentation | 9.1, 9.2, 9.7 |
| Feb 7, 2026 Granola call | Transcript -- Caravela LOI, pricing, mid-market strategy | 9.2, 9.9 |
| Feb 8, 2026 Granola call | Transcript -- strategy review, TAM | 9.1, 9.4 |
| Feb 9, 2026 Granola call | Transcript -- workflow analysis, EU vs US, product architecture | 9.7, 9.8 |
| EIOPA, BaFin, ACPR, IVASS, ASF, DGSFP, DNB, FSMA, NAIC, AM Best, Conning | Regulatory filings -- carrier counts, market sizes | 9.2-9.6 |

---

# Part 10: Business Model & Unit Economics

# Module 10: Business Model & Unit Economics

**Status:** DRAFT v1.0
**Last updated:** February 9, 2026
**Feeds:** Pitch deck slides 10-12, financial model, investor data room, pricing page, sales proposals

---

## 10.1 Revenue Stream: Decision Engine (Primary)

This is the core product and the core revenue stream. The decision engine -- the 6 expert judgment steps that consume 60-70% of adjuster time -- is what nobody else has built and what carriers will pay the most for.

### Revenue Model: Dual Pricing

Carriers choose between per-claim pricing and platform licensing. Most start per-claim (low barrier, pay-as-you-go) and migrate to platform pricing as they scale.

> "100% we can get from the tiniest 50k a year for this. And for the biggest 1,000,000."
> -- Jeremy Blehaut [TRANSCRIPT: Feb 7, 2026]

[SOURCE: mysa_product_strategy.md, Part 3e -- pricing model; CLAUDE ANALYSIS on per-claim vs platform pricing]

**Per-Claim Pricing:**

| Tier | Per-Claim Price | Typical Annual Volume | Implied Revenue |
|------|----------------|----------------------|----------------|
| Micro (<EUR50M GWP) | EUR5-8/claim | ~5-15K claims/year | EUR25K-120K/year |
| Starter (EUR50-100M GWP) | EUR3-5/claim | ~15-30K claims/year | EUR45K-150K/year |
| Professional / Caravela tier (EUR100-200M GWP) | EUR2-4/claim | ~30-60K claims/year | EUR60K-240K/year |
| Growth (EUR200M-500M GWP) | EUR2-3/claim | ~60-150K claims/year | EUR120K-450K/year |
| Enterprise (EUR500M-1B GWP) | Custom | ~150K+ claims/year | Custom |

[SOURCE: mysa_product_strategy.md, Part 3e -- pricing tiers anchored to Caravela economics]

**Platform Licensing (Annual Contract):**

| Tier | Annual Contract Value | Target Carrier Size |
|------|----------------------|-------------------|
| Micro | EUR10K-30K/year | <EUR50M GWP |
| Starter | EUR30K-100K/year | EUR50-100M GWP |
| Professional | EUR50K-200K/year | EUR100-200M GWP |
| Growth | EUR200K-500K/year | EUR200M-500M GWP |
| Enterprise | EUR500K-2M/year | EUR500M-1B GWP |

[SOURCE: mysa_product_strategy.md, Part 3e]

**Why this works:** At a Caravela-sized carrier (EUR188M GWP, ~57K claims/year), a EUR100K/year platform license equals 0.05% of GWP. At EUR3/claim, that is EUR171K/year or 0.09% of GWP. Both are trivial relative to the potential savings (EUR562K-750K/year from STP improvement alone).

[SOURCE: mysa_product_strategy.md, Part 3e -- Caravela reference economics]

### What the Decision Engine Includes

Per-claim or platform pricing covers access to the full 6-step decision workflow:

| Step | What Mysa Does | Time Impact |
|------|---------------|-------------|
| 1. Coverage verification | AI reads policy, matches claim facts, highlights applicable coverage and exclusions | 15-30 min --> 2 min review |
| 2. Policy report checking | AI validates completeness, flags gaps, identifies contradictions | 10-20 min --> 1 min review |
| 3. Repair assessment | AI compares scope against comparable claims, flags anomalies | 15-25 min --> 3 min review |
| 4. Cost analysis | AI pulls comparable data, identifies outliers, calculates expected range | 10-20 min --> 2 min review |
| 5. Reserve calculation | AI calculates reserve with confidence interval, shows P&L impact | 10-15 min --> 2 min review |
| 6. Fraud detection | AI pattern-matches against fraud signals, scores risk, recommends SIU referral | 5-10 min --> automated flagging |

[SOURCE: mysa_product_strategy.md, Part 1 -- decision sub-steps and time estimates]

**Total decision time:** 65-120 minutes today --> 10-15 minutes with Mysa (4-8x improvement on the decision step).

---

## 10.2 Revenue Stream: Intake & Document Processing (Secondary)

### Why Intake Is a Revenue Stream (Not Just a Feature)

> "I think what is wrong with companies, and I think our value is here, but you cannot start here. Because it's garbage in garbage out. So if you already have a lot of garbage in, you need to start by fixing that."
> -- Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

The decision engine requires clean, structured data. Carriers do not have it. Mysa must fix "garbage in" as a prerequisite to delivering decision value -- and that fix is independently valuable enough to charge for.

[SOURCE: mysa_product_strategy.md, Part 2e -- garbage in garbage out; CLAUDE ANALYSIS on intake as data pipeline]

### Intake Pricing: Two Buyer Types

**A. Carrier Document Processing**

Carriers need incoming claim documents (EAS forms, invoices, photos, police reports, medical records) parsed, structured, and validated before decisions can begin. Current state: manual data entry, 20-30 minutes per document set, error-prone.

| Capability | Current Process | Mysa Process |
|-----------|----------------|-------------|
| EAS form extraction | Manual data entry (20-30 min, error-prone) | OCR extraction (2 min, 81.5% accuracy) |
| Convention matching | Manual lookup after data entry | Instant deterministic matching from structured data |
| Document completeness | Adjuster eyeballs it, misses gaps | AI flags missing fields, auto-generates follow-up requests |
| Data structuring | Typed into CMS by hand | Auto-populated structured data, validated against business rules |

[SOURCE: mysa_product_strategy.md, Part 6c -- EAS process comparison; caravela-ocr.md -- 81.5% accuracy]

**Pricing model:** Bundled into the per-claim or platform pricing above. Document processing is the data pipeline -- it feeds the decision engine. Charging separately risks creating a perception that Mysa is "just another intake tool." Bundling keeps the narrative on decisions.

**B. Broker Intake Flow (Standalone Revenue Opportunity)**

Brokers submit claims on behalf of policyholders. Today this is email-based, unstructured, and creates the "garbage in" problem at source.

| Capability | Description |
|-----------|-------------|
| White-labeled FNOL forms | Carrier-branded intake forms for brokers |
| Email-to-claim creation | Chrome extension / email parser creates structured claims from broker emails |
| AI gap analysis | Flags missing information before submission, reducing back-and-forth |
| Auto-outreach | Draft SMS/email to policyholder requesting missing info |

[SOURCE: mysa_product_strategy.md, Part 1 -- broker FNOL flow; Part 5a -- product flow architecture]

**Pricing model:** Per-submission fee or bundled into carrier platform license. When a carrier licenses Mysa, broker intake is included (it improves the carrier's data quality). Standalone broker tools could be offered as a lighter entry point for carriers not yet ready for the full decision engine.

### Cost to Deliver

LLM processing cost for the full Mysa stack (gap filling, pattern learning, second opinion, email parsing, appeal drafting, clinical suggestions, contract parsing):

**~$6.50/month per 100 claims**

| Use Case | Calls/Month (per 100 claims) | Avg Tokens | Cost |
|----------|------------------------------|-----------|------|
| Gap Filling | 200 | 500 | $0.50 |
| Pattern Learning | 30 | 2,000 | $0.60 |
| Second Opinion | 50 | 1,500 | $3.00 |
| Email Parsing | 100 | 500 | $0.25 |
| Appeal Drafting | 10 | 2,000 | $1.00 |
| Clinical Suggestions | 150 | 500 | $0.38 |
| Contract Parsing | 5 | 3,000 | $0.75 |
| **Total** | | | **~$6.50/month** |

[SOURCE: LLM_ARCHITECTURE.md -- cost estimation table]

**At scale (Caravela: ~57K claims/year = ~4,750 claims/month):**
- LLM cost: ~$309/month = ~$3,700/year
- At EUR100K/year platform pricing: LLM cost is **~3.7% of revenue**
- At EUR3/claim pricing (EUR171K/year): LLM cost is **~2.2% of revenue**

This is an exceptionally high gross margin business. LLM costs are negligible relative to revenue.

---

## 10.3 Unit Economics: Per Adjuster

This is the math the VP Claims runs when deciding whether to buy.

### Current State (Without Mysa)

| Metric | Value | Source |
|--------|-------|--------|
| Fully loaded cost per adjuster | ~$110K/year | mysa_product_strategy.md, Part 2a; TRANSCRIPT |
| Caseload | ~125 open claims at any time | mysa_product_strategy.md, Part 2a |
| Claims closed per year | 300-480 | mysa_product_strategy.md, Part 2a |
| Cost per closed claim | $230-$370 | mysa_product_strategy.md, Part 2a |
| Time on decisions per claim | 65-120 minutes | mysa_product_strategy.md, Part 1 |
| Time on admin / data entry | 30-40% of total time | mysa_product_strategy.md, Part 2c |
| Annual attrition | 20% at carriers, 33% at TPAs | mysa_product_strategy.md, Part 2a |
| Knowledge loss per departure | ~6 years institutional knowledge | mysa_product_strategy.md, Part 2a |

[SOURCE: mysa_product_strategy.md, Part 2a -- adjuster economics]

### With Mysa: 3x Productivity

| Metric | Current | With Mysa | Change |
|--------|---------|-----------|--------|
| Claims closed/year per adjuster | 300-480 | 900-1,440 | **3x** |
| Cost per closed claim | $230-$370 | $75-$125 | **-67%** |
| Decision time per claim | 65-120 min | 10-15 min | **4-8x faster** |
| New hire time to productivity | ~6 years to full expertise | Weeks (SOP-guided workflows) | **Massive** |

[SOURCE: mysa_product_strategy.md, Part 2c -- 3x productivity math]

### Per-Adjuster Savings Calculation

```
Current cost per adjuster:                    $110,000/year
Current claims closed:                        300-480/year
Current cost per claim:                       $230-$370

With Mysa (3x throughput):
  Same adjuster now closes:                   900-1,440 claims/year
  Cost per claim:                             $75-$125
  Savings per claim:                          $155-$245

Total savings per adjuster:                   $45,000-$120,000/year
```

**The pitch:** Every adjuster on Mysa saves the carrier $45K-$120K per year in cost-per-claim efficiency. A 20-adjuster claims team saves $900K-$2.4M/year. Mysa costs EUR50K-200K/year for a Caravela-tier carrier. That is a **4.5-48x ROI on the labor economics alone** -- before reserve accuracy and STP improvements.

[SOURCE: mysa_product_strategy.md, Part 2c -- savings calculation]

### For a Mid-Tier TPA (200 Adjusters)

| Metric | Value |
|--------|-------|
| Current cost (200 adjusters x $110K) | $22M/year |
| Claims processed (200 x 390 avg) | ~78,000/year |
| With Mysa (3x): same team processes | ~234,000 claims/year |
| OR: reduce headcount by 2/3 for same volume | Save ~$14.7M/year |
| Realistic savings (blend of both) | **$9-24M/year** |

[SOURCE: mysa_product_strategy.md, Part 2c -- TPA savings calculation]

---

## 10.4 Unit Economics: Per Carrier

This is the math the CFO runs. Two value drivers: adjuster productivity (Section 10.3 above) and STP improvement.

### STP (Straight-Through Processing) Improvement

STP = claims resolved with minimal human intervention. Convention systems (EU motor) promise 60-70% STP. Actual delivery: ~10%. The gap is data quality at intake.

[SOURCE: mysa_product_strategy.md, Part 2b -- STP gap; MODULE_01_POSITIONING.md, Section 1.2]

**The STP math (Caravela-sized carrier, ~50K motor claims/year):**

```
Current STP rate:                             ~10%
Target STP rate with Mysa:                    40-50%
Delta:                                        30-40 percentage points

Additional claims processed via STP:          15,000-20,000/year
Time saved per STP claim:                     ~45 min
Total hours saved:                            11,250-15,000 hours/year
At EUR50/hour loaded cost:                    EUR562,500-EUR750,000 saved/year

Mysa charges:                                 EUR100K-200K/year
ROI on STP improvement alone:                 3-7x
```

[SOURCE: mysa_product_strategy.md, Part 6c -- STP improvement calculation]

### ACV by Carrier Tier

| Tier | GWP Range | Est. Claims/Year | Target ACV | Per-Claim Equivalent |
|------|----------|-----------------|-----------|---------------------|
| Micro | <EUR50M | ~5-15K | EUR10K-30K | EUR2-6/claim |
| Starter | EUR50-100M | ~15-30K | EUR30K-100K | EUR2-3/claim |
| **Professional (Caravela tier)** | **EUR100-200M** | **~30-60K** | **EUR50K-200K** | **EUR2-3/claim** |
| Growth | EUR200M-500M | ~60-150K | EUR200K-500K | EUR1.3-8/claim |
| Enterprise | EUR500M-1B | ~150K+ | EUR500K-2M | Custom |

[SOURCE: mysa_product_strategy.md, Part 3e]

### Combined ROI: Caravela-Tier Carrier

This is what the CFO sees in the sales proposal.

```
CARRIER PROFILE
  GWP:                                        EUR188M (Caravela reference)
  Motor claims/year:                          ~42,000
  Property claims/year:                       ~15,000
  Total claims:                               ~57,000/year
  Adjusters:                                  ~20-30 (estimated for 149-employee carrier)

MYSA ANNUAL COST
  Platform license:                           EUR100K-200K/year
  As % of GWP:                                0.05-0.11%

SAVINGS: STP IMPROVEMENT (motor only)
  STP rate improvement:                       10% --> 40-50%
  Additional STP claims:                      12,600-16,800/year
  Hours saved:                                9,450-12,600 hours/year
  Value at EUR50/hr:                          EUR472,500-EUR630,000/year

SAVINGS: ADJUSTER PRODUCTIVITY
  Per-adjuster savings:                       $45K-$120K/year
  For 25 adjusters:                           $1.1M-$3.0M/year (~EUR1.0M-EUR2.8M)

SAVINGS: RESERVE ACCURACY
  5% improvement in reserve accuracy:         EUR500K-EUR750K freed capital or avoided losses/year
  (Caravela lost EUR18M in one year from weather + poor reserve management)

TOTAL ANNUAL VALUE TO CARRIER
  STP savings:                                EUR472K-630K
  Productivity savings:                       EUR1.0M-2.8M
  Reserve accuracy:                           EUR500K-750K
  TOTAL:                                      EUR2.0M-4.2M/year

ROI
  Mysa cost:                                  EUR100K-200K/year
  Return:                                     EUR2.0M-4.2M/year
  ROI:                                        10-42x
```

[SOURCE: mysa_product_strategy.md, Parts 2a, 2c, 2d, 6c -- combined from adjuster economics, STP calculation, reserve accuracy; TRANSCRIPT -- Caravela EUR18M loss]

**Note:** The 10-42x ROI range is wide because it combines three value drivers with their own ranges. Even at the conservative end (3-7x ROI on STP alone), the investment is justified. The CFO presentation should lead with STP savings (most concrete, easiest to measure) and layer productivity and reserves as additional upside.

---

## 10.5 Pricing Tiers

### Tier Summary

| Tier | Target Carrier | GWP Range | Annual Contract | Per-Claim Overlay | EU Carrier Count (16 countries) | What They Get |
|------|---------------|----------|----------------|------------------|-------------------------------|--------------|
| **Micro** | Regional mutuals, niche writers | <EUR50M | EUR10K-30K/year | EUR5-8/claim | ~243-372+ | Decision engine (motor only), standard SOP templates, email support |
| **Starter** | Small multi-line carriers | EUR50-100M | EUR30K-100K/year | EUR3-5/claim | ~204-260+ | + Property module, custom SOP encoding, dedicated onboarding |
| **Professional** | Caravela-tier carriers | EUR100-200M | EUR50K-200K/year | EUR2-4/claim | ~96-165 | + Full decision engine (motor + property), convention systems, broker FNOL, priority support |
| **Growth** | Large multi-line carriers | EUR200M-500M | EUR200K-500K/year | EUR2-3/claim | ~30-47 | + Multi-country, API access, custom integrations, dedicated CSM |
| **Enterprise** | Major carriers approaching EUR1B | EUR500M-1B | EUR500K-2M/year | Custom | ~16-19 | + Full customization, on-premise option, SLA guarantees, dedicated team |

[SOURCE: mysa_product_strategy.md, Part 3e -- pricing tiers; market_landscape_overview.md, Section 2 -- carrier counts]

### Design Partner Pricing

| Partner | Terms | Rationale |
|---------|-------|-----------|
| Caravela | Free for 6 months, then EUR50K-100K/year | Design partner builds the product with us. Their data + feedback is worth more than revenue in Phase 1. |

[SOURCE: mysa_product_strategy.md, Part 3e -- design partner row]

### Pricing as % of GWP

A useful sanity check. Insurance technology spend is typically 0.1-0.5% of GWP for mid-market carriers.

| Tier | Low End (% GWP) | High End (% GWP) | Assessment |
|------|-----------------|------------------|-----------|
| Micro (EUR30K on EUR40M GWP) | 0.05% | 0.075% | Well within budget |
| Starter (EUR100K on EUR75M GWP) | 0.04% | 0.13% | Reasonable |
| Professional (EUR200K on EUR150M GWP) | 0.03% | 0.13% | Trivial relative to savings |
| Growth (EUR500K on EUR350M GWP) | 0.06% | 0.14% | Standard enterprise software |
| Enterprise (EUR2M on EUR750M GWP) | 0.07% | 0.27% | Justified by ROI |

All tiers sit comfortably below 0.3% of GWP. Given the 3-42x ROI demonstrated in Section 10.4, pricing has significant room to increase as the product matures and value proof accumulates.

### Per-Claim Pricing: When to Lead With It

Per-claim pricing is better for:
- **Landing new customers** -- low barrier, no large upfront commitment
- **TPAs** -- per-claim is the natural unit (they process claims for others)
- **Pilots and proof-of-concept** -- pay for what you use, prove value before committing
- **Volume-variable carriers** -- seasonal or catastrophe-driven claim volumes

Platform pricing is better for:
- **Revenue predictability** -- for Mysa and for the carrier's budget planning
- **High-volume carriers** -- per-claim gets expensive above ~60K claims/year at EUR3/claim
- **Multi-line carriers** -- bundling motor + property into one license

**Recommendation:** Offer both. Let the carrier choose. Most will start per-claim and migrate to platform as they scale.

[SOURCE: mysa_product_strategy.md, Part 3e -- CLAUDE ANALYSIS on per-claim vs platform pricing]

### Revenue Expansion: Property Upsell

Adding property to an existing motor customer increases revenue by 60-70% per carrier with zero new customer acquisition. 80-95% of carriers writing motor also write property.

[SOURCE: market_landscape_overview.md, Section 3 -- motor vs property; mysa_product_strategy.md, Part 9b]

| Carrier | Motor Revenue | + Property Revenue | Combined |
|---------|-------------|-------------------|---------|
| Micro | EUR10K-30K | +EUR6K-21K | EUR16K-51K |
| Starter | EUR30K-100K | +EUR18K-70K | EUR48K-170K |
| Professional | EUR50K-200K | +EUR30K-140K | EUR80K-340K |
| Growth | EUR200K-500K | +EUR120K-350K | EUR320K-850K |
| Enterprise | EUR500K-2M | +EUR300K-1.4M | EUR800K-3.4M |

---

## 10.6 Financial Projections

### [REQUIRES FOUNDER INPUT]

This section requires founder decisions on the following inputs before projections can be modeled:

**Revenue Projections -- Inputs Needed:**

| Input | Why It Matters | Notes |
|-------|---------------|-------|
| Year 1 revenue target | Sets hiring/spend plan | Design partner (Caravela) is free for 6 months. First paying customer timing drives this. |
| Year 1-3 carrier acquisition pace | 2 carriers/quarter? 5? 10? | Determines sales hiring, onboarding capacity, and infrastructure investment. |
| Average ACV assumption | EUR75K? EUR100K? EUR150K? | Depends on whether early customers are Starter or Professional tier. |
| Property upsell timeline | Month 8-14 per Module roadmap | Accelerates revenue 60-70% per carrier. Critical to model. |
| US market entry timing | Year 2? Year 3? | Changes TAM and required investment significantly. |

**Cost Projections -- Inputs Needed:**

| Input | Why It Matters | Notes |
|-------|---------------|-------|
| Current monthly burn rate | Determines runway from any raise | Pre-revenue burn = founders + infrastructure. |
| Current runway | How long until revenue or next raise needed | Critical for fundraising timeline. |
| Headcount plan (6/12/18 months) | Largest cost line | Engineering, sales, customer success, domain expertise. |
| Infrastructure costs | Cloud, LLM APIs, data storage | LLM costs are ~$6.50/month per 100 claims -- scales linearly. |
| Office / operational costs | If any | Remote-first reduces this significantly. |

**Projection Framework (to be completed with founder inputs):**

| Metric | Year 1 | Year 2 | Year 3 |
|--------|--------|--------|--------|
| Carriers (paying) | [TBD] | [TBD] | [TBD] |
| Average ACV | [TBD] | [TBD] | [TBD] |
| ARR | [TBD] | [TBD] | [TBD] |
| Headcount | [TBD] | [TBD] | [TBD] |
| Monthly burn | [TBD] | [TBD] | [TBD] |
| Gross margin | >90% (LLM costs are <4% of revenue) | >90% | >90% |
| Net burn | [TBD] | [TBD] | [TBD] |

**What we do know:**
- LLM cost per 100 claims: ~$6.50/month (scales linearly)
- At a Caravela-sized carrier (57K claims/year), LLM cost is ~$3,700/year vs EUR100K+ revenue = >96% gross margin on AI infrastructure
- The business is SaaS with recurring revenue -- no physical goods, no hardware
- Customer acquisition is direct sales to 1-2 decision-makers at mid-market carriers (3-6 month cycle)

---

## 10.7 Fundraising Plan

### [REQUIRES FOUNDER INPUT]

**Founder Signals from Calls:**

> "I think we need to raise as much money as ClaimSorted [EUR11.4M]"
> -- Tiago Brigido [TRANSCRIPT]

> "Further AI series A level [$30M]... on seed."
> -- Jeremy Blehaut [TRANSCRIPT]

[SOURCE: mysa_product_strategy.md, Part 9c -- pitch slide 12]

These are aspirational anchors, not decisions. This section requires founder alignment on:

**Decisions Needed:**

| Decision | Options | Considerations |
|----------|---------|---------------|
| Target raise amount | EUR2-5M (seed) vs EUR5-15M (large seed / Series A) | Depends on ambition timeline. Smaller raise = faster close, less dilution. Larger raise = faster hiring, multi-country expansion. |
| Use of funds allocation | Engineering / Sales / Operations / Buffer | Typical seed: 60% engineering, 20% sales, 10% operations, 10% buffer. |
| Timeline to raise | Q2 2026? Q3 2026? | Depends on current runway and Caravela traction milestones. |
| Equity allocation | Founder split, ESOP, investor % | Standard: 15-20% ESOP, 15-25% to seed investors. Must be decided before term sheet. |
| Investor profile | EU insurtech specialists? US generalist VCs? Angels? | EU investors understand the market. US investors validate the TAM story. |
| Valuation expectations | Pre-money based on comparable raises | ClaimSorted: EUR11.4M raised. Five Sigma: ~$20M raised. FurtherAI: $30M raised. Shift: $320M raised. These set the floor for what's possible in the category. |

**What the raise should fund (framework):**

| Priority | Investment | Rationale |
|----------|-----------|-----------|
| 1 | Engineering team (3-5 engineers) | Build the decision engine beyond OCR. SOP workflow engine, multi-country convention systems, property module. |
| 2 | First sales hire | Dedicated to EU mid-market carriers. Co-founders cannot sell and build simultaneously at scale. |
| 3 | Customer success (1 hire) | Onboarding carriers requires deep domain knowledge + technical support. |
| 4 | Infrastructure | Cloud, LLM APIs, data storage, security/compliance tooling. |
| 5 | Runway buffer | 18-24 months minimum to reach meaningful ARR milestone. |

**The TAM story for investors (validated):**

| Stage | TAM | Timeline | Narrative |
|-------|-----|----------|-----------|
| Wedge | EUR2.7-18.6M (Southern EU, Caravela tier, motor only) | Year 1 | Proves the product works |
| Year 2-3 | EUR80-170M (all EU mid-market, motor + property) | Year 2-3 | Real SaaS business |
| Year 3-5 | EUR160-425M (EU + US mid-market, both lines) | Year 3-5 | Venture-scale |
| Vision | EUR320M-1.1B (full addressable + expansion) | Year 5+ | IPO-scale |

[SOURCE: mysa_product_strategy.md, Part 9b -- TAM progression]

**The honest TAM narrative:**

"We start with EU motor -- the convention system wedge that nobody else has. Within 6 months, the same carrier pays us for property too (same AI, bigger problem, same buyer). By year 3, we're in the US with the same product. The market is ~11-28M claims/year in our target segment alone, 80-95M globally. And 90%+ of mid-market carriers have ZERO AI claims tools today."

[SOURCE: mysa_product_strategy.md, Part 9b -- TAM narrative]

---

## Key Numbers Summary (For Pitch Deck)

| Metric | Value | Source |
|--------|-------|--------|
| **Per-claim price** | EUR2-10/claim | Part 3e |
| **Platform price** | EUR50K-2M/year | Part 3e |
| **LLM cost per 100 claims** | ~$6.50/month | LLM_ARCHITECTURE.md |
| **Gross margin** | >96% (on AI infrastructure) | Calculated: $3,700 LLM cost vs EUR100K+ revenue |
| **Adjuster loaded cost** | ~$110K/year | Part 2a |
| **Claims per adjuster (current)** | 300-480/year | Part 2a |
| **Claims per adjuster (with Mysa)** | 900-1,440/year | Part 2c |
| **Cost per claim reduction** | $230-370 --> $75-125 (-67%) | Part 2c |
| **Savings per adjuster** | $45K-120K/year | Part 2c |
| **STP improvement** | 10% --> 40-50% | Part 6c |
| **STP savings (50K claims)** | EUR562K-750K/year | Part 6c |
| **Combined ROI (Caravela-tier)** | 10-42x | Section 10.4 calculation |
| **Addressable carriers (primary)** | 96-165 (EU Caravela tier) | market_landscape_overview.md |
| **Addressable carriers (full)** | 1,530-2,400 (EU + US all tiers) | Part 9b |
| **Target segment claims** | ~11-28M claims/year | market_landscape_overview.md |
| **Property upsell** | +60-70% revenue per carrier | Part 9b |
| **Market openness (EU mid-market)** | 90-95% untouched by AI claims tools | market_landscape_overview.md |

---

## Sources

| Source | Type | Sections Used |
|--------|------|--------------|
| `mysa_product_strategy.md` Part 1 | Primary -- decision sub-steps, time estimates | 10.1, 10.3 |
| `mysa_product_strategy.md` Part 2a-2e | Primary -- adjuster economics, STP gap, reserve accuracy, garbage-in problem | 10.2, 10.3, 10.4 |
| `mysa_product_strategy.md` Part 3e | Primary -- pricing model, tiers, Caravela economics | 10.1, 10.4, 10.5 |
| `mysa_product_strategy.md` Part 6c | Primary -- STP improvement calculation | 10.4 |
| `mysa_product_strategy.md` Part 9b-9c | Primary -- TAM, pitch deck, fundraising signals | 10.4, 10.7 |
| `LLM_ARCHITECTURE.md` | Secondary -- LLM cost per 100 claims | 10.2 |
| `market_landscape_overview.md` | Secondary -- carrier counts, market sizing, competitive landscape | 10.4, 10.5 |
| `MODULE_01_POSITIONING.md` | Cross-reference -- ICP, value proposition, adjuster demographics | 10.3 |
| Feb 7, 2026 Granola call | Transcript -- pricing ("50k to 1M"), Caravela EUR18M loss, mid-market strategy | 10.1, 10.4, 10.7 |
| Feb 8-9, 2026 Granola calls | Transcript -- productivity calculations, SOP workflows, fundraising anchors | 10.3, 10.7 |

---

# Part 11: Risk & Regulatory

# Module 11: Risk & Regulatory

**Status:** DRAFT v1.0
**Last updated:** February 9, 2026
**Feeds:** Investor data room, board risk register, founder decision-making, regulatory compliance roadmap

---

## 11.1 Competitive Risks

This section is deliberately blunt. These are the companies that could kill Mysa or make it irrelevant. The question for each is not "are they a threat?" but "how much time do we have, and what specifically would they need to build to close the gap?"

### Verisk / XactAI — Existential Risk (2-3 Year Horizon)

**What they are:** $40B+ public company. Xactimate has 75-80% market share in US property estimation. 4.5B+ data points. XactAI launched September 2025 — AI tools bundled free inside Xactimate Pro (photo labels, transcription summaries, admin automation).

**Why they're dangerous:** Verisk has the distribution (every property adjuster already uses Xactimate), the data (every estimate ever written), and the capital to build whatever they want. If they decide to build a real decision engine inside Xactimate — coverage analysis, triage, reserve recommendation — they could own this overnight. The decision layer is a natural expansion from estimation. They don't need to sell anything new; they just turn on a feature.

**Why they haven't done it yet:** XactAI today is features, not decisions. Photo labels and transcription summaries are admin automation, not expert judgment. Building a decision engine requires understanding coverage law, carrier-specific SOPs, and convention systems — none of which Verisk has. Their DNA is estimation (what does it cost?) not decision (should we pay?). CCC sued Tractable for 5 years over competitive behavior — Verisk defends its moat, it doesn't build adjacent products quickly.

**Honest assessment:** This is the existential risk. Verisk moving from features to platform would compress Mysa's entire US property thesis. The mitigation is time and geography: start in EU where Verisk has zero presence, build the convention system moat they can't replicate, and establish carrier relationships before they move. If Verisk announces a decision engine in 2027, Mysa needs to already be embedded in 20+ carriers with switching costs.

**Threat timeline:** 2-3 years before they could ship something meaningful. Their internal culture and regulatory caution slow product cycles. But watch XactAI feature releases quarterly — any move toward coverage analysis is the early warning signal.

[SOURCE: home_property_competitive_deep_dive.md, Section 19; market_landscape_overview.md — competitor table; competitive_landscape_reality_check.md — "XactAI = admin features only"]

### Shift Technology — EU Threat (12-18 Month Horizon)

**What they are:** $320M raised. 25+ countries, 135 customers (mostly large carriers). Started in fraud detection. Launched "Shift Claims" in September 2025 — agentic AI for the full claims lifecycle. AXA Switzerland reports 60% automation rate, 30% faster handling, >99% accuracy.

**Why they're dangerous:** Shift is the most dangerous EU competitor. They already serve large EU carriers. They have brand recognition, compliance infrastructure, and multi-country operations. Their September 2025 pivot from fraud-only to full claims automation puts them directly in the path of anyone building claims AI in Europe.

**What they don't have:** Convention matching (IRSA, CARD, CIDE, IDS). SOP-driven workflows (they use generic playbooks). EAS data quality processing. Their 60% automation rate at AXA is task automation (workflow routing, document handling), not decision automation (coverage, liability, reserves). They start downstream of the convention decision — after the data is already in the system. They serve enterprise carriers, not mid-market.

**Honest assessment:** If Shift decides to build EAS processing + convention matching as part of Shift Claims, they could close Mysa's EU motor gap within 12-18 months. The bet is that fixing what happens BEFORE the system (EAS capture to structured data to convention match) is a document AI problem, not a workflow automation problem, and Shift won't prioritize it because their customers are enterprise carriers who already have decent data quality. But this is a bet, not a certainty.

**Threat timeline:** They could build convention support in 12-18 months if they chose to. The question is whether they will — their roadmap appears focused on scaling workflow automation, not niche convention systems.

[SOURCE: home_property_competitive_deep_dive.md, Section 20; competitive_landscape_reality_check.md — Shift analysis; mysa_product_strategy.md, Part 9d — investor objection table]

### Five Sigma / Clive — Direct Competitor (Now)

**What they are:** ~$20M raised. Multi-agent AI adjuster copilot ("Clive") that works on any CMS. $10.1M revenue. 180% year-over-year growth. 70% US, 30% EU. Landed Starr Insurance (Jan 2026) — a meaningful mid-market/specialty win. 6 generic AI agents.

**Why they're dangerous:** Five Sigma is the closest direct competitor. Same thesis (AI for adjusters), similar buyer (mid-market carriers), growing fast. Clive's multi-agent architecture mirrors Mysa's planned agent system. They have traction, revenue, and a working product.

**What they don't have:** Convention systems. Carrier-specific SOP workflows (generic playbooks instead). Decision ground truth capture. EU convention matching. Their product is a CMS + copilot stack — a bigger sale, longer cycle, higher switching cost. They're selling a full platform replacement, not a decision layer that sits on top of existing systems.

**Honest assessment:** Five Sigma at 180% growth will be a $30M revenue company in 18 months. If they build convention support and carrier-specific SOPs, they're Mysa with a 2-year head start. The differentiation today is real (decision engine vs CMS copilot, EU conventions, SOP encoding). But "they don't have X yet" is a temporary advantage. Mysa must be in market and building switching costs before Five Sigma builds what they're missing.

**Threat timeline:** Active now. Watch for EU expansion announcements and convention system features.

[SOURCE: competitive_landscape_reality_check.md — Five Sigma analysis; home_property_competitive_deep_dive.md, Section 19; market_landscape_overview.md — funded competitor table]

### CCC + EvolutionIQ — Adjacent Threat (2-3 Year Horizon)

**What they are:** CCC is a $7B+ public company. Acquired EvolutionIQ for $730M (closed Q1 2025). EvolutionIQ is an AI claims guidance platform — tells adjusters what to do next on injury claims. CCC launched "Medhub for Casualty" in Q3 2025 (medical record synthesis for auto casualty adjusters). IX Cloud Platform connects 35,000+ businesses. $45-50M revenue from EvolutionIQ in year one.

**Why they're dangerous:** CCC is moving from "here's the estimate" to "here's what the adjuster should do." That's the same direction as Mysa. $730M acquisition signals they're serious about owning the adjuster workflow. 7 of top 15 disability carriers. They have the data (35,000 businesses), the distribution, and the capital.

**What they don't have:** EU presence. Property/commercial coverage. Convention systems. Their moat is the 35,000-business US auto network, which doesn't transfer to property or to Europe. EvolutionIQ is auto casualty + workers' comp — structurally different from motor or property decisions.

**Honest assessment:** CCC is a US auto casualty company moving into adjuster guidance. They're dangerous if they expand into property or EU, but both would require building new products from scratch. The $730M EvolutionIQ acquisition makes them the "smart money" validation that this category matters — which helps Mysa's fundraising narrative. But if CCC builds or acquires EU capability, they could enter the market with overwhelming resources.

**Threat timeline:** 2-3 years for meaningful EU or property expansion. They're focused on integrating EvolutionIQ and scaling auto casualty.

[SOURCE: competitive_landscape_reality_check.md — CCC analysis; home_property_competitive_deep_dive.md, Section 19]

### Wamy — Unknown Threat (Emerging)

**What they are:** Launched from stealth December 2025. Claims to validate coverage using AI. "Claims AI workforce" positioning. Funding undisclosed. Pre-traction.

**Why they might be dangerous:** If Wamy is building coverage determination AI — reading policies, matching against claim facts, determining "is this covered?" — that's Mysa's core value proposition. Brand new means they could be building with modern architecture and no legacy baggage.

**What we know they don't have:** Traction. Customers. Revenue. Convention systems. EU presence (appears US-only). Demonstrated accuracy on real claims. Everything is claims and positioning at this stage.

**Honest assessment:** Wamy is a question mark, not a confirmed threat. They could be building exactly what Mysa is building, or they could be another intake automation startup with better marketing copy. The risk is that they raise significant capital on the coverage determination thesis before Mysa establishes itself. Monitor closely but don't overreact.

**Threat timeline:** 6-12 months to see if they get traction. Watch for funding announcements and customer logos.

[SOURCE: mysa_product_strategy.md, Part 8 — coverage determination competitive landscape; market_landscape_overview.md — "Wamy pre-traction"]

---

## 11.2 Technical Risks

### OCR Accuracy Ceiling

**Current state:** 81.5% normalized accuracy on Portuguese motor EAS forms using Gemini 3 Flash Preview with x3 voting and GOLDEN RULES for field normalization. 44 claims with ground truth.

**The risk:** OCR accuracy may plateau below the threshold needed for automated convention matching. EAS forms include handwritten text, inconsistent formatting, multi-language content, and poor scan quality. Moving from 81.5% to the 95%+ needed for reliable STP is a non-linear challenge — the last 15% is exponentially harder than the first 80%.

**Why it matters:** Convention systems are deterministic lookup tables. They work perfectly with clean data and fail completely with dirty data. If Mysa can't reliably extract EAS fields, the entire EU motor STP thesis breaks. The STP gap (10% actual vs 60-70% theoretical) exists precisely because of data quality — Mysa is betting it can solve what the industry has failed to solve for decades.

**Specific failure modes:**
- Handwritten checkboxes misread (fault determination flips entirely on one checkbox)
- Vehicle registration numbers misread (wrong vehicle, wrong insurer, wrong convention)
- Date fields ambiguous (DD/MM vs MM/DD across EU countries)
- Multiple EAS versions across countries with different field layouts

### Coverage Determination Reliability

**The risk:** Coverage decisions require interpreting policy language against claim facts. Policy language is intentionally ambiguous ("sudden and accidental," "wear and tear," "maintenance exclusion"). LLMs can misinterpret exclusion clauses, miss endorsements, or hallucinate coverage that doesn't exist. A wrong coverage determination has direct financial and legal consequences — wrongful denials lead to lawsuits, wrongful approvals lead to leakage.

**Why it matters:** Coverage determination is the highest-value decision Mysa automates. If the AI gets it wrong even 5% of the time, carriers won't trust it. Worse, if it gets it wrong in a systematic way (always missing a specific exclusion), it creates pattern-of-practice liability.

### Convention System Complexity Across Countries

**The risk:** Each EU country has its own convention system with different rules, different forms, different arbitration processes, and different edge cases. Portugal uses IDS/CIMPAS. France uses IRSA. Italy uses CARD. Spain uses CIDE/ASCIDE/CICOS. Germany has its own system. Building reliable convention matching for one country is hard. Building it for six is a multi-year engineering effort.

**Why it matters:** Mysa's EU expansion thesis requires multi-country convention support. Each country requires country-specific regulatory knowledge, language support, form variations, and insurer association relationships. This is a compounding engineering cost, not a one-time build. Slow multi-country rollout means slower revenue growth and more time for competitors to build their own convention support.

### LLM Hallucination Risk in Legal/Financial Decisions

**The risk:** Large language models hallucinate — they generate plausible but factually incorrect output. In a claims decision context, hallucinations include: citing policy clauses that don't exist, applying legal standards from the wrong jurisdiction, calculating reserves based on non-existent comparable claims, or recommending coverage based on a misread exclusion.

**Why it matters:** Claims decisions have legal and financial consequences. A hallucinated coverage determination that leads to a wrongful denial could trigger bad-faith litigation. A hallucinated reserve recommendation could cause material P&L error. Human-in-the-loop mitigates but doesn't eliminate this risk — adjusters under time pressure may rubber-stamp AI recommendations, especially as trust in the system builds.

**Specific concern:** As LLM accuracy improves and adjusters trust the system more, the risk of rubber-stamping increases. The tool is most dangerous when it works well 98% of the time — the 2% failure mode becomes invisible.

---

## 11.3 Market Risks

### Mid-Market Budget Constraints

**The risk:** Caravela-tier carriers (€100-200M GWP) have real budget for technology (€50K-200K/year is 0.03-0.2% of GWP), but they're not enterprise buyers. Budget approval processes are simpler — but budgets are also tighter. Economic pressure, rising reinsurance costs, or a bad claims year can freeze discretionary technology spending. Mid-market carriers may want Mysa but defer purchasing until "next year."

**Why it matters:** Mysa's pricing model assumes carriers will spend €50K-200K/year on claims AI. If mid-market budget constraints mean the actual spend is €20K-50K, unit economics break. Per-claim pricing helps (lower barrier) but also means revenue scales slowly.

### Long Sales Cycles Even for Mid-Market

**The risk:** Even at mid-market carriers with 1-2 decision-makers, insurance technology sales cycles run 3-6 months. Carriers are risk-averse by nature — they sell risk management. New technology adoption requires proof-of-concept, pilot, security review, and procurement. "Fast" in insurance is still slow compared to SaaS.

**Why it matters:** As a pre-revenue startup with limited runway, 3-6 month sales cycles mean Mysa needs 6-12 months of runway beyond first serious sales engagement to reach revenue. Each lost deal costs 3-6 months of sales effort with zero revenue.

### Carrier Consolidation

**The risk:** The European insurance market is consolidating. Larger carriers acquire mid-market carriers, reducing the total addressable buyer count. Acquired carriers typically adopt the parent's technology stack — eliminating them as independent buyers. Example: Generali's acquisition strategy across Southern Europe has already absorbed multiple Caravela-tier carriers.

**Why it matters:** Mysa's TAM calculation assumes 96-165 Caravela-tier carriers across 16 EU countries. If 20-30% are acquired by enterprise carriers who build in-house over the next 3-5 years, the addressable market shrinks materially.

### Economic Downturn Reducing Claims Spend

**The risk:** In a recession, insurers cut costs — and technology budgets are the first to go. Claims volume may drop (fewer cars on the road, less construction, less discretionary activity). Carriers may decide to "do more with less" using existing tools rather than invest in new ones.

**Counterpoint:** Workforce crisis persists regardless of economic cycle. Adjusters retiring don't come back when the economy recovers. This creates a structural need that economic cycles can delay but not eliminate.

### Concentration Risk — Caravela as Only Design Partner

**The risk:** Caravela is Mysa's only design partner and only source of real claims data. If Caravela deprioritizes the partnership, changes leadership, gets acquired, or simply decides they don't need Mysa, the company loses its only development feedback loop and its only proof of product-market fit.

**Why it matters:** Every product decision, every accuracy benchmark, and every sales pitch currently depends on one carrier's data and one carrier's endorsement. "We're live with a Portuguese carrier" is the entire proof point. If that proof point disappears, there's nothing behind it.

---

## 11.4 Regulatory: EU

### GDPR Article 22 — Automated Decision-Making

**What it says:** GDPR Article 22 gives data subjects the right not to be subject to decisions based solely on automated processing that produce legal effects or similarly significant effects. Claims decisions that affect financial outcomes (what gets paid, how much, whether a claim is denied) produce legal effects.

**What it means for Mysa:**
- Fully automated claims decisions are prohibited unless explicit consent is obtained, the decision is necessary for a contract, or authorized by member state law with safeguards
- Even with consent, data subjects have the right to obtain human intervention, express their point of view, and contest the decision
- Mysa's human-in-the-loop architecture is not optional — it's legally mandated
- AI recommendations that adjusters routinely rubber-stamp may be challenged as "de facto automated decisions" — the human review must be meaningful, not performative

**Compliance approach:** Human-in-the-loop is built into the architecture from Day 1. Every AI recommendation requires explicit adjuster action (accept, modify, reject). Decision audit trails document human involvement at each step. This is a regulatory moat — competitors who build automation-first will need to retrofit human oversight.

### EU AI Act — High-Risk Classification

**What it says:** The EU AI Act (Regulation 2024/1689) classifies AI systems used in insurance contexts that affect access to essential services as "high-risk" under Annex III. Claims AI falls under this classification.

**Requirements for high-risk AI systems:**
- Conformity assessment before market placement
- Technical documentation (system design, development process, capabilities, limitations)
- Data governance (training data quality, relevance, representativeness)
- Human oversight mechanisms
- Accuracy, robustness, and cybersecurity standards
- Transparency — users must be informed they're interacting with an AI system
- Post-market monitoring and incident reporting
- Registration in the EU AI database

**What it means for Mysa:**
- Conformity assessment is a meaningful cost and timeline burden (legal, technical documentation, third-party audit)
- Data governance requirements affect how training data (adjuster decisions) is collected, stored, and used
- Transparency requirements mean carriers and claimants must know when AI is involved in decisions
- Post-market monitoring means ongoing accuracy tracking and incident reporting
- US competitors entering EU will face the same burden — this is a barrier to entry for Shift, Five Sigma, CCC, and others not already EU-compliant

**Timeline:** The AI Act entered into force August 2024. High-risk provisions apply from August 2026. Mysa must have conformity assessment completed before commercial launch in EU.

### Per-Country Insurance Regulators

Each EU country has its own insurance regulator with specific requirements for claims processing, data handling, and technology use.

| Country | Regulator | Key Requirements |
|---------|-----------|-----------------|
| **Portugal** | ASF (Autoridade de Supervisao de Seguros e Fundos de Pensoes) | 20 business day response deadline. IDS/CIMPAS convention system. Portuguese language requirements. ASF complaint process after 20 days non-response. |
| **Spain** | DGSFP (Direccion General de Seguros y Fondos de Pensiones) | CIDE/ASCIDE/CICOS convention systems. Spanish language requirements. Specific pre-authorization frameworks. |
| **France** | ACPR (Autorite de Controle Prudentiel et de Resolution) | IRSA convention system. French language requirements. Strict data localization preferences. CNIL (data protection authority) enforcement of GDPR. |
| **Italy** | IVASS (Istituto per la Vigilanza sulle Assicurazioni) | CARD convention system. Italian language requirements. Specific claims handling timelines. |
| **Germany** | BaFin (Bundesanstalt fur Finanzdienstleistungsaufsicht) | German language requirements. Strict data protection enforcement. Own convention system. |

**What it means for Mysa:** Each country expansion requires regulatory review, language localization, convention system integration, and potentially country-specific conformity documentation. This is a compounding compliance cost that slows expansion but also creates a moat — each country's regulatory barrier must be crossed by every competitor individually.

### Data Residency

**The risk:** GDPR requires that personal data (including claims data) be stored and processed within the EU or in countries with adequate data protection (as determined by the European Commission). Some member states have stricter preferences or requirements for financial/insurance data.

**What it means for Mysa:**
- All claims data must be stored on EU-resident servers (Supabase/infrastructure must be EU-hosted)
- LLM API calls that send claims data to US-based providers (e.g., Google Gemini, OpenAI) may violate data residency requirements — depends on data processing agreements and server locations
- Encryption in transit and at rest is mandatory
- Data retention periods (5-10 years for medical/claims records) must be documented and enforced

---

## 11.5 Regulatory: US

### State-by-State Insurance Regulation

**The landscape:** Insurance in the US is regulated at the state level, not federal. 50 states + DC, each with its own insurance commissioner, regulations, and requirements. The NAIC (National Association of Insurance Commissioners) provides model laws and guidelines, but adoption varies by state.

**What it means for Mysa:**
- Claims handling timelines differ by state (some require acknowledgment within 15 days, some within 30)
- Settlement practices vary (some states mandate specific claims documentation, some don't)
- AI in insurance regulation is evolving — Colorado's SB 21-169 requires testing for unfair discrimination in AI insurance models. Other states are following
- No single compliance framework covers all states — multi-state carriers need state-by-state compliance

**Practical impact:** US expansion requires legal review per state. The regulatory burden is different from EU (no single "AI Act" equivalent) but equally fragmented. Mysa's initial US strategy should focus on a cluster of states with similar regulations rather than attempting nationwide coverage.

### Data Privacy Laws

**The landscape:** No federal data privacy law equivalent to GDPR. California (CCPA/CPRA), Virginia (VCDPA), Colorado (CPA), Connecticut (CTDPA), and other states have their own privacy laws. Health data may be subject to HIPAA depending on the claim type (bodily injury, workers' comp).

**What it means for Mysa:**
- Claims data handling must comply with applicable state privacy laws
- Bodily injury claims involving medical records trigger additional privacy requirements
- Consumer rights (access, deletion, opt-out) vary by state
- Less restrictive than GDPR overall, but more fragmented

### "Deny Then Defend" Legal Framework

**The landscape:** US insurance operates under a fundamentally different legal philosophy than EU. In the EU, the insurer pays the policyholder first and recovers through convention systems. In the US, insurers may deny claims and let the claimant challenge the denial. This creates a litigation-heavy environment where bad-faith denial lawsuits are a major risk.

**What it means for Mysa:**
- AI-recommended denials carry higher legal risk in the US than in the EU
- Audit trails and decision documentation are critical for bad-faith defense
- Adjusters may be more cautious about AI recommendations (fear of personal liability)
- The compliance/legal buyer persona is more important in US sales than EU
- Mysa's value proposition in the US leans more toward "consistent, defensible decisions" than "faster decisions"

### How US Differs from EU Approach

| Dimension | EU | US |
|-----------|----|----|
| **Primary regulation** | GDPR + AI Act + country regulators | State-by-state, no federal AI law (yet) |
| **Automated decision rules** | Article 22 — explicit prohibition with exceptions | No equivalent prohibition — but state unfair practices laws apply |
| **AI-specific regulation** | AI Act high-risk classification | Emerging (Colorado, NYC Local Law 144, proposed federal bills) |
| **Data residency** | EU-resident required | No federal requirement |
| **Claims philosophy** | Pay first, recover later (convention) | Deny then defend |
| **Litigation risk** | Lower — convention systems reduce disputes | Higher — bad-faith lawsuits common |
| **Compliance cost** | High upfront (conformity assessment) | High ongoing (50-state monitoring) |

---

## 11.6 Operational Risks

### Key-Person Risk — 2 Founders

**The risk:** Mysa is two people. Tiago holds the insurance domain expertise — convention systems, SOPs, carrier workflows, adjuster operations. Jeremy holds the technical capability — OCR engine, LLM architecture, product development. If either becomes unavailable (health, personal, co-founder conflict), the company loses 50% of its capability with no redundancy.

**Why it matters:** Investors assess key-person risk explicitly. At pre-seed stage, two founders IS the company. There's no team to absorb the loss. Domain + technical is an unusually tight coupling — neither skill is easily replaced.

### Caravela Dependency — Design Partner Concentration

**The risk:** Caravela is the only source of real claims data, the only proof of product-market fit, and the only relationship validating the EU mid-market thesis. The entire product is built on Caravela's data (44 claims with ground truth, IDS convention rules, EAS form structures). Every demo, every benchmark, and every investor conversation references Caravela.

**Specific failure modes:**
- Caravela leadership change deprioritizes the partnership
- Caravela gets acquired by a larger carrier that builds in-house
- Caravela decides the pilot didn't deliver enough value to continue
- Caravela demands exclusivity terms that limit Mysa's ability to serve competitors
- Caravela's claims data is not representative of other EU carriers (Portugal-specific patterns)

### Talent Acquisition in EU

**The risk:** Building an AI claims decision engine requires a rare intersection of skills: LLM engineering, insurance domain knowledge, and multi-language EU expertise. This talent profile barely exists. Recruiting in Portugal/Southern EU is cheaper than US/UK but the talent pool for AI + insurance is smaller.

**Specific challenges:**
- Senior ML engineers in Lisbon: available but competitive (Farfetch alumni, other AI startups)
- Insurance domain experts willing to join a startup: rare (industry is conservative)
- Multi-language capability (Portuguese + Spanish + French + Italian): limits candidate pool further
- Competing with remote offers from US/UK companies paying higher salaries

### Burn Rate Management Pre-Revenue

**The risk:** Mysa is pre-revenue with a product that requires 3-6 month sales cycles even in the best case. LLM API costs are ongoing (Gemini processing per claim), cloud infrastructure costs grow with each carrier onboarded, and hiring even one employee doubles the burn rate.

**Specific concerns:**
- LLM costs: ~$6.50/month per 100 claims at current architecture — manageable at pilot scale, significant at 10+ carrier scale
- Sales timeline: 3-6 months to close even a mid-market deal
- Revenue recognition: per-claim pricing means revenue ramps slowly (not a large upfront contract)
- Runway math: every month of delayed revenue compresses the window for product iteration

---

## 11.7 Mitigation Strategies

### Competitive Risk Mitigations

| Risk | Severity | Likelihood | Mitigation |
|------|----------|------------|------------|
| **Verisk builds decision AI** | Critical | Medium (2-3yr) | Start in EU where Verisk has zero presence. Build convention system moat they can't replicate from the US. Establish 20+ carrier relationships with switching costs before Verisk moves. If Verisk enters, Mysa's EU + convention + SOP data makes it an acquisition target rather than a casualty. |
| **Shift adds convention matching** | High | Medium (12-18mo) | Move faster on convention implementation across Portugal, Spain, France, Italy. Build relationships with insurer associations (IDS, CIDE, IRSA, CARD bodies). Shift's enterprise focus means mid-market carriers are underserved — own that segment before they look down-market. |
| **Five Sigma scales EU** | High | High (now) | Differentiate on decision engine vs CMS replacement (lighter integration, faster deployment). Build convention support Five Sigma lacks. Win Caravela-tier logos before Five Sigma can localize for Southern EU. Publish case studies showing decision-layer value vs generic copilot. |
| **CCC enters EU or property** | Medium | Low (2-3yr) | Monitor CCC quarterly earnings for EU or property expansion signals. Build the property decision layer first (CCC has zero property footprint). If CCC enters EU, they'll start enterprise — Mysa owns mid-market. |
| **Wamy gains traction** | Medium | Low-Medium | Monitor funding, customer announcements, and product demos. If Wamy raises significant capital, accelerate go-to-market timeline. The advantage is Mysa has a working product and a design partner — Wamy has a landing page. |

### Technical Risk Mitigations

| Risk | Severity | Likelihood | Mitigation |
|------|----------|------------|------------|
| **OCR accuracy ceiling** | High | Medium | Multi-model ensemble (Gemini + Claude + GPT) with voting. Field-specific GOLDEN RULES for normalization. Invest in synthetic training data generation. Accept that some fields will need human verification — build UI for efficient human-in-the-loop correction. Target 90%+ on critical fields (checkboxes, vehicle IDs), accept lower on non-critical fields. |
| **Coverage determination reliability** | High | High | Never ship fully automated coverage decisions. Confidence scoring on every recommendation — low-confidence recommendations flagged for mandatory human review. Build coverage determination as carrier-specific rules + LLM reasoning, not pure LLM. Policy clause citation required for every recommendation (verifiable, not hallucinated). |
| **Convention complexity across countries** | Medium | High | Sequence country rollout by convention similarity (IDS and CIDE are structurally similar). Build abstraction layer that separates convention rules from country-specific implementation. Partner with convention system administrators for rule validation. Budget 3-4 months per country for convention integration. |
| **LLM hallucination in decisions** | Critical | Medium | Structured output with required citations (policy clause, comparable claim, SOP step). Retrieval-augmented generation (RAG) from carrier's own policy documents, not general knowledge. Confidence thresholds — recommendations below threshold require human override. Regular accuracy audits against ground truth. Never allow LLM to generate legal language without template verification. |

### Market Risk Mitigations

| Risk | Severity | Likelihood | Mitigation |
|------|----------|------------|------------|
| **Mid-market budget constraints** | Medium | Medium | Per-claim pricing lowers adoption barrier (no large upfront commitment). Start with €2-5 per claim to prove ROI before upselling to platform license. Offer pilot programs with performance guarantees (no ROI, no charge). Target carriers with active hiring pain — budget exists when the alternative is hiring another adjuster at €50-70K/year. |
| **Long sales cycles** | Medium | High | Design partner model (Caravela) bypasses cold sales. Warm introductions through Tiago's insurance network. Broker channel as faster-close distribution (brokers decide in weeks, not months). Build self-serve trial for small carriers/TPAs. Target 3 parallel sales conversations to absorb inevitable delays. |
| **Carrier consolidation** | Low | Medium | Target carriers unlikely to be acquired (mutual insurers, regional specialists). Build relationships with acquiring carriers too — if they acquire a Mysa customer, pitch to expand. Multi-line capability (motor + property) increases switching costs, making Mysa survive acquisitions. |
| **Economic downturn** | Medium | Low-Medium | Position as cost-reduction tool, not growth tool. "Handle the same claims volume with fewer adjusters" sells in downturns. Per-claim pricing scales down with claims volume — carriers don't pay for what they don't use. Workforce crisis persists regardless of economic cycle — adjusters retiring don't come back. |
| **Caravela concentration risk** | High | Medium | Sign a second design partner within 6 months (target: Spanish carrier via CIDE convention). Diversify proof points — run OCR benchmarks on publicly available EAS samples from other countries. Build product features that don't depend on Caravela-specific data. Negotiate a case study / reference agreement with Caravela (written, not verbal). |

### Regulatory Risk Mitigations (EU)

| Risk | Severity | Likelihood | Mitigation |
|------|----------|------------|------------|
| **GDPR Article 22 challenge** | High | Medium | Human-in-the-loop is architectural, not bolted on. Every AI recommendation requires explicit adjuster action. Audit trail documents meaningful human involvement (not rubber-stamping). Provide data subject access and explanation mechanisms. Get GDPR compliance opinion from EU data protection counsel before commercial launch. |
| **EU AI Act conformity** | High | Certain | Begin conformity assessment preparation now — technical documentation, data governance policies, human oversight mechanisms. Budget €30-50K for legal/compliance counsel. Engage a conformity assessment body by Q3 2026. Build accuracy monitoring and incident reporting into the product from Day 1. Conformity assessment completion is a gate for EU commercial launch. |
| **Per-country regulator requirements** | Medium | Certain | Sequence country entry by regulatory complexity (Portugal first — smallest regulator, existing relationship. Spain second. France and Italy third). Hire or contract a regulatory affairs specialist with multi-country EU insurance experience. Budget 2-3 months of regulatory preparation per country. Build modular compliance framework — shared core with country-specific modules. |
| **Data residency requirements** | Medium | Certain | Deploy on EU-resident infrastructure from Day 1 (Supabase EU region, Vercel EU edge). Verify LLM provider data processing agreements — ensure claims data sent to LLM APIs is not stored or used for training. If required, evaluate EU-hosted LLM options (Mistral, or self-hosted models). Encrypt all claims data at rest and in transit. |

### Regulatory Risk Mitigations (US)

| Risk | Severity | Likelihood | Mitigation |
|------|----------|------------|------------|
| **State-by-state regulation** | Medium | Certain | Enter US through 3-5 states with aligned regulations first (cluster approach). Monitor NAIC model law adoption for AI in insurance. Budget for state-by-state legal review. Build state-specific compliance modules into the product. |
| **Data privacy fragmentation** | Medium | Medium | Build to CCPA/CPRA standard (most restrictive major state law) as baseline — provides coverage for most states. Add HIPAA compliance for BI claims with medical records. Monitor new state privacy laws quarterly. |
| **Bad-faith litigation exposure** | High | Medium | Every AI recommendation includes cited policy clause, comparable claim data, and SOP step — creating a defensible audit trail. Position Mysa as "consistent, documented decision-making" — reducing bad-faith risk rather than creating it. Include legal/compliance buyer persona in US sales process. |

### Operational Risk Mitigations

| Risk | Severity | Likelihood | Mitigation |
|------|----------|------------|------------|
| **Key-person risk (2 founders)** | High | Low-Medium | Document institutional knowledge — SOPs, architecture decisions, carrier relationships — in shared knowledge base. Cross-train: Jeremy learns convention system basics, Tiago learns product/tech fundamentals. First hire should partially overlap with one founder's capabilities. Key-person insurance for both founders once funded. |
| **Caravela dependency** | High | Medium | See Caravela concentration risk above. Additionally: structure the design partner agreement with clear milestones, mutual commitments, and IP ownership. Avoid giving Caravela veto power over product direction. Build a product that works for ANY carrier, not just Caravela — test against public data from other markets. |
| **Talent acquisition in EU** | Medium | Medium | Recruit from adjacent domains: fintech ML engineers, legal-tech NLP specialists, ex-Farfetch/Feedzai talent in Lisbon. Offer equity aggressively — pre-seed equity is the primary compensation lever. Remote-first for technical roles to access broader EU talent pool. Partner with University of Lisbon / NOVA SBE for insurance domain interns. |
| **Burn rate pre-revenue** | High | High | Maintain 18+ months runway at all times. LLM cost optimization: batch processing, caching, model selection per task (cheap models for simple tasks, expensive models for complex decisions). Delay hiring until design partner validates product-market fit. Revenue target: first paying customer within 9 months of funding. |

---

## Sources

| Source | Type | Sections Used |
|--------|------|--------------|
| `competitive_landscape_reality_check.md` | Primary — competitive analysis | 11.1, 11.7 |
| `home_property_competitive_deep_dive.md` Sections 19-21 | Primary — competitive deep dive, regulatory | 11.1, 11.2, 11.4 |
| `market_landscape_overview.md` Sections 7-8 | Primary — competitor funding, market openness | 11.1, 11.3 |
| `mysa_product_strategy.md` Part 9d | Primary — investor objections | 11.1, 11.4, 11.5 |
| `mysa_product_strategy.md` Part 5d | Primary — human-in-the-loop | 11.4 |
| `REGULATORY_COMPLIANCE.md` | Primary — Portuguese regulatory framework | 11.4 |
| `MODULE_01_POSITIONING.md` | Context — ICP, product, founder-market fit | 11.3, 11.6 |
| `caravela-ocr.md` (memory) | Internal — accuracy metrics | 11.2 |
| EU AI Act (Regulation 2024/1689) | External — legislation | 11.4 |
| GDPR (Regulation 2016/679), Article 22 | External — legislation | 11.4 |
| Granola transcripts Feb 5-9, 2026 | Transcript — founder calls | 11.1, 11.4, 11.5 |

---

*End of Mysa Founding Operating System v1.0*
