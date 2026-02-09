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
