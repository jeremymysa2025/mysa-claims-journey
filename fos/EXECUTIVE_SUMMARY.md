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
