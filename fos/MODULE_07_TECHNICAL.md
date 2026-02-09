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
