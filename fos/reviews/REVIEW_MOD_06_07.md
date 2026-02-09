# Review: Module 6 (Product) & Module 7 (Technical Architecture)

**Reviewer:** Claude Sonnet 4.5
**Date:** February 9, 2026
**Files Reviewed:**
- /Users/jeremyblehaut/mysa-claims-journey/fos/MODULE_06_PRODUCT.md (1331 lines)
- /Users/jeremyblehaut/mysa-claims-journey/fos/MODULE_07_TECHNICAL.md (647 lines)

---

## Module 6: Product — Issues

### 6.1 Unsupported Claims (Minor)

The following statements lack [SOURCE:], [TRANSCRIPT:], or [WEB:] citations:

**Section 6.2 (Decision Sub-Steps):**
- Line 136: "40-80 pages" for policy documents — reasonable estimate but uncited
- Line 158: "15-30 min (manual) --> 2 min review" time savings — no source for baseline time
- Line 186: "10-20 min (manual) --> 1 min review" for policy report checking — uncited baseline
- Line 214: "15-25 min (manual) --> 3 min review" for repair assessment — uncited baseline
- Line 242: "10-20 min (manual) --> 2 min review" for cost analysis — uncited baseline
- Line 274: "10-15 min (manual) --> 1 min review" for reserve calculation — uncited baseline
- Line 308: "5-10 min (manual assessment) --> automated flagging" for fraud detection — uncited baseline

**Assessment:** These time estimates are critical to the value proposition but lack empirical backing. Recommend adding [SOURCE: claims_journey_discovery.md, Phase X] citations or labeling them as [ESTIMATED] if not sourced from discovery research.

**Section 6.5 (Clippy Architecture):**
- Line 528: "Getting API access to any of these takes 6-18 months of partnership negotiation" — no source
- Line 616: "74% of insurers still run some legacy tech" — cited in Module 7 but not here

**Section 6.8 (Human-in-the-Loop):**
- Line 746-752: The "adoption gradient" table (5%, 40-60%, 70-90% adoption rates) — no empirical source. This appears to be hypothetical modeling, which should be labeled as such.

### 6.2 Product Spec Clarity (Strong)

**Could an engineer build from this?** Yes, with caveats.

**Strengths:**
- Section 6.1 (7-Step Pipeline) provides clear system logic per step
- Section 6.2 (6 Decision Sub-Steps) specifies data inputs, system logic, adjuster actions, and time targets for each sub-step
- Section 6.9 (Demo Spec: Adjuster Portal) includes detailed step-by-step flows with "What Shows on Screen," "What to Highlight," and "Technical Requirement" columns — highly actionable
- Section 6.11 (Demo Data & Workflow Specs) provides realistic claim data examples with field-level detail

**Gaps:**
- **No UI/UX wireframes or mockups** — the demo specs describe screens but don't show them
- **No error handling specifications** — what happens when OCR confidence is low? When convention matching is ambiguous? When the adjuster rejects all 6 recommendations?
- **No data validation rules** — what are acceptable ranges for reserve amounts, confidence scores, fraud scores?
- **No API contracts** — if the Chrome extension reads from Guidewire/Duck Creek, what data schema does it expect?

**Recommendation:** Add a Section 6.12: "API & Data Schema Specifications" with JSON schemas for key data structures (claim object, decision object, SOP workflow object).

### 6.3 Jargon Without Definition

**Insurance jargon (first use, not defined in Module 6):**
- "STP" (line 44) — defined in Module 3 as "straight-through processing" but not repeated here
- "FNOL" (line 19) — defined in Module 3 but not in Module 6
- "BI" (line 47) — defined later in the module but first used at line 47 without definition
- "SIU" (line 47) — defined later but first used without definition
- "ACV" (line 209) — Actual Cash Value, defined in parentheses but only at first use in a long paragraph
- "DRP" (line 231) — Direct Repair Program, defined only in parentheses
- "Colossus" (line 237) — referenced as if reader knows what it is (BI valuation tool)

**Technical jargon:**
- "JSON" (line 35) — assumed knowledge
- "Confidence score" (line 65) — concept introduced but not explained (0-100%? 0-1? What does 90% mean?)
- "Reasoning chain" (line 67) — what format? Natural language? Structured?

**Recommendation:** Add a glossary at the start of Module 6 or cross-reference Module 1 definitions more explicitly.

### 6.4 Section Completeness (Complete)

All sections 6.1-6.11 are present and substantive:
- 6.1 Product Flow ✓
- 6.2 The 6 Decision Sub-Steps ✓
- 6.3 SOP-Driven Workflow Engine ✓
- 6.4 The Core Loop ✓
- 6.5 The "Clippy" Architecture ✓
- 6.6 All Personas & How the Product Helps Each ✓
- 6.7 User Journey Maps ✓
- 6.8 Human-in-the-Loop: Why ✓
- 6.9 Demo Spec: Adjuster Portal ✓
- 6.10 Demo Spec: Broker Flow ✓
- 6.11 Demo Data & Workflow Specs ✓

### 6.5 Demo Feasibility (Realistic with Caveats)

**Demo 1: EU Motor — EAS to Settlement ("The Easy Case")**
- **Feasibility:** HIGH
- **Rationale:** Caravela OCR engine already exists (81.5% accuracy on EAS forms). Convention matching is deterministic lookup. Document generation is templating.
- **Caveat:** Real-time OCR visualization (line 821: "populating field by field in real time") requires UI work. Current extraction is batch, not streaming.

**Demo 2: US Property — Water Damage ("The Hard Case")**
- **Feasibility:** MEDIUM
- **Rationale:** Requires policy document parsing (Gemini can do this), photo analysis (achievable), and SOP-driven investigation checklists. The "sudden vs gradual" decision logic (lines 854-860) is complex and would require significant prompt engineering or rule encoding.
- **Caveat:** The "what-if" scenario (line 860: showing denial path) is impressive but doubles demo complexity. Requires stable coverage determination logic that works in both directions.

**Demo 3: Historical Data Flywheel**
- **Feasibility:** LOW (for demo purposes)
- **Rationale:** Requires 147 processed claims and 6 months of data (line 878). This is a post-launch metric, not a demo capability.
- **Recommendation:** Remove from "must show" and keep as "investor deck slide" only.

**Build Requirements Analysis (lines 905-913):**
- Items 1-7 are achievable within 8-12 weeks for a 2-person team
- Item 4 (SOP upload → workflow UI) is the highest-risk item — requires robust LLM parsing with human validation loop
- Item 6 (document generation templates) is straightforward but requires carrier-specific branding/formatting

**Overall Demo Assessment:** Demo 1 is ready to build now. Demo 2 is a 4-6 week stretch goal. Demo 3 should be cut from the demo build and saved as a post-launch case study.

---

## Module 7: Technical — Issues

### 7.1 Unsupported Claims (Minor)

**Section 7.1 (Architecture Philosophy):**
- Line 21: "A large Portuguese healthcare group with 40+ clinics and $100M in revenue 'spent millions building a submission tool. They're still on spreadsheets.'" — This quote has a [SOURCE: AI_NATIVE_ARCHITECTURE_SPEC.md, Appendix D] citation, but it's anecdotal. No validation of the $100M revenue or "millions" spent claim.

**Section 7.2 (Current Stack):**
- Line 78: "81.5% normalized field-level accuracy" — cited properly with memory file reference ✓
- Line 86: "accuracy competitive with Google Document AI (82%) and above Amazon Textract (78%)" — cited properly ✓

**Section 7.4 (OCR & Document Processing):**
- Line 192-201: Error source percentages (30% column confusion, 16% address parsing, etc.) — well-cited from CARAVELA-COMPETITIVE-ASSESSMENT ✓

**Section 7.6 (Integration Map):**
- All integration accessibility claims are cited from research documents ✓

**Assessment:** Module 7 has stronger citation discipline than Module 6. Only the Portuguese healthcare anecdote (line 21) is weakly sourced.

### 7.2 Technical Accuracy (Strong with One Gap)

**Architecture Philosophy (7.1):**
- Agent-native architecture explanation is clear and well-differentiated from "add AI to existing software" approaches ✓
- The atomic tools principle (Section 7.1, lines 52-56) is architecturally sound ✓

**Current Stack (7.2):**
- Stack description matches known Caravela deployment (Next.js, Gemini 3 Flash, Supabase, Vercel) ✓
- Accuracy metrics match benchmark data from memory files ✓
- x3 voting and GOLDEN RULES references are accurate ✓

**OCR Pipeline (7.4):**
- The extraction → voting → normalization flow is technically accurate ✓
- Path to 90%+ roadmap (lines 206-231) is realistic given dataset size constraints ✓
- Mistral OCR elimination (line 232) is well-justified with Reducto benchmark data ✓

**Convention Matching (7.5):**
- Correctly describes convention systems as deterministic lookup, not AI ✓
- Accurately represents the data quality bottleneck, not the lookup itself ✓

**Integration Map (7.6):**
- Open vs. partner-gated vs. locked classifications are accurate ✓
- CCC, Guidewire, Colossus access restrictions match industry reality ✓

**Agentic Approach (7.7):**
- Chrome extension architecture is sound ✓
- Limitations are honestly stated (lines 405-410) ✓

**Data Model (7.8):**
- Knowledge schema (lines 430-503) is well-structured ✓
- Decision ground truth capture is architecturally correct ✓

**Compliance (7.9):**
- GDPR, AI Act, and US state regulation summaries are accurate ✓
- Human-in-the-loop requirement correctly tied to GDPR Article 22 ✓

**Gap: Multi-Agent Architecture Decision (7.3, lines 124-136)**
- Three options presented (single orchestrator, multi-model, LangChain/LangGraph) but no clear recommendation or selection criteria
- **Recommendation:** Add a decision matrix with criteria: complexity, cost, latency, debuggability, time-to-ship. This will guide the CTO hire.

### 7.3 Section Completeness (Complete with Gaps Acknowledged)

All sections 7.1-7.9 are present:
- 7.1 Architecture Philosophy ✓
- 7.2 Current Stack ✓
- 7.3 Production Stack Vision ✓
- 7.4 OCR & Document Processing ✓
- 7.5 Convention Matching Engine ✓
- 7.6 Integration Map ✓
- 7.7 Agentic Approach for Locked Systems ✓
- 7.8 Data Model & Knowledge Layer ✓
- 7.9 EU + US Compliance ✓

**Acknowledged Gaps (FOUNDER INPUT REQUIRED tags):**
- Cloud provider decision (7.3, line 110)
- Multi-agent architecture (7.3, line 124)
- Build vs. wait decision for Chrome extension (7.7, line 411)
- Compliance gaps (7.9, line 619)

**Assessment:** These are legitimate decision points that require founder input, not documentation failures. Well-handled.

---

## Demo Spec Feasibility

### Demo 1: EU Motor — EAS to Settlement

**Feasibility:** HIGH (8-10 weeks to production-ready demo)

| Component | Status | Effort |
|-----------|--------|--------|
| EAS OCR extraction | EXISTS (Caravela engine, 81.5% accuracy) | 1 week integration |
| Convention matching (CIMPAS/Portugal) | EXISTS (deterministic rules) | 1 week integration |
| Missing data flagging | LOGIC EXISTS (completeness validation) | 1 week UI |
| Auto-outreach (SMS) | NEW | 2 weeks (template + SMS API) |
| Reserve recommendation | NEW (statistical model + historical data) | 3 weeks |
| Document generation | NEW (templates) | 2 weeks |
| Adjuster review UI (accept/modify/reject) | NEW | 2 weeks |

**Critical Path:** Reserve recommendation (requires historical claims data analysis) → Document generation → Adjuster UI

**Risk:** Historical data may not exist in sufficient volume for accurate reserve modeling. Fallback: use formula-based reserve calculation per carrier SOP.

### Demo 2: US Property — Water Damage

**Feasibility:** MEDIUM (12-16 weeks to production-ready demo)

| Component | Status | Effort |
|-----------|--------|--------|
| Policy document parsing (HO-3) | NEW (Gemini can do this) | 3 weeks |
| Photo analysis (water damage detection) | NEW | 4 weeks |
| Coverage determination logic | NEW (sudden vs gradual decision tree) | 4 weeks |
| SOP-driven investigation checklist | NEW | 2 weeks |
| Document generation (coverage letter, denial letter) | NEW | 2 weeks |
| "What-if" scenario toggle | NEW | 2 weeks |

**Critical Path:** Coverage determination logic (sudden vs gradual) is the hardest problem. Requires robust prompt engineering or rule encoding.

**Risk:** Coverage determination for "sudden vs gradual" water damage is a complex judgment call. May require extensive testing to achieve acceptable accuracy. Recommend starting with simpler coverage scenarios (excluded driver, lapsed policy) before tackling "sudden vs gradual."

### Demo 3: Historical Data Flywheel

**Feasibility:** LOW (not achievable for demo; requires live data)

**Rationale:** This requires 100+ processed claims and 3-6 months of adjuster interaction data. It's a post-launch metric, not a demo capability.

**Recommendation:** Cut from demo build. Use as "investor deck slide" showing projected improvement over time.

---

## Cross-Module Consistency

### Product Spec (Module 6) vs. Claims Journey (Module 3)

**Alignment Check:**

| Module 6 Section | Module 3 Reference | Consistency |
|------------------|-------------------|-------------|
| 6.1 Product Flow (7 steps) | Module 3, Phases 0-11 | ✓ ALIGNED — Module 6 condenses 12 phases into 7 product steps |
| 6.2 Decision Sub-Steps | Module 3, Phase 9 (Decision) | ✓ ALIGNED — Module 6 expands Phase 9 into 6 sub-steps |
| 6.6 Personas | Module 3, Section 3.1-3.3 | ✓ ALIGNED — all personas from Module 3 appear in Module 6 table |
| 6.11 Triage Decision Logic | Module 3, Phase 6 (Triage) | ✓ ALIGNED — triage checks match Module 3 discovery |
| 6.11 Investigation Activities | Module 3, Phase 7 (Investigation) | ✓ ALIGNED — 13 activities match Module 3 list |
| 6.11 Convention Systems | Module 3, Section 3.1 Phase 3 | ✓ ALIGNED — CIMPAS, IRSA, CARD, CIDE all consistent |

**Minor Inconsistencies:**

1. **Time estimates diverge slightly:**
   - Module 6 (line 113): Investigation time = "1-15 hours (varies)"
   - Module 3 (Phase 7, line 334-336): Investigation time = "1-3 hours (simple PD), 5-15 hours (complex PD), 20-100+ hours (BI)"
   - **Resolution:** Module 3 is more granular. Module 6 should reference Module 3 ranges.

2. **STP rate claims:**
   - Module 6 (line 50): "Auto triage: I have 20-30%"
   - Module 3 (line 146): "Actual STP is only ~10%"
   - **Resolution:** These refer to different things. Module 6 quote is about triage automation (20-30% auto-routed correctly), Module 3 is about end-to-end STP (10%). Not inconsistent, but could be clarified.

### Product Spec (Module 6) vs. Technical Spec (Module 7)

**Alignment Check:**

| Module 6 Claim | Module 7 Support | Consistency |
|---------------|------------------|-------------|
| 6.1: "Caravela OCR engine" | 7.4: OCR pipeline described, 81.5% accuracy | ✓ ALIGNED |
| 6.2: "6 decision sub-steps" | 7.8: Decision ground truth schema | ✓ ALIGNED |
| 6.3: "SOP upload → workflow generation" | 7.8: InsurerKnowledge schema includes workflows | ✓ ALIGNED |
| 6.5: "Chrome extension / Clippy" | 7.7: Agentic approach for locked systems | ✓ ALIGNED |
| 6.5: "Vault knowledge base" | 7.8: Knowledge layer sources | ✓ ALIGNED |
| 6.9: "Convention matching (CIMPAS)" | 7.5: Convention matching engine | ✓ ALIGNED |
| 6.9: "Historical claims data for reserve calculation" | 7.8: Knowledge acquisition phases | ✓ ALIGNED |

**No significant inconsistencies found.** Module 6 product claims are all technically supported in Module 7.

---

## [PLACEHOLDER] Tags Found

**Result:** NONE

No [PLACEHOLDER] tags found in either module.

---

## [FOUNDER INPUT REQUIRED] Tags Found

**Module 7 (Technical Architecture):**

1. **Section 7.3, Line 110:** Cloud Provider Decision
   - Options: GCP (europe-west), AWS (eu-west-1), Supabase + Vercel
   - Recommendation provided: GCP for 6-12 months, AWS for enterprise later
   - **Status:** DECISION READY — clear options and recommendation

2. **Section 7.3, Line 124:** Multi-Agent Architecture
   - Options: Single orchestrator, multi-model with router, LangChain/LangGraph
   - Recommendation: "The simplest option that works (single orchestrator)"
   - **Status:** DECISION READY — clear recommendation with evolution path

3. **Section 7.7, Line 411:** Build vs. Wait Decision (Chrome Extension)
   - Options: Build extension early (Months 3-6), pursue API partnerships first, both in parallel
   - Recommendation: "Build the Chrome extension first"
   - **Status:** DECISION READY — clear recommendation with rationale

4. **Section 7.9, Line 619:** Compliance Gaps Requiring Founder Decision
   - Four gaps listed: EU AI Act conformity assessment, DPA template, bias testing framework, SOC 2 / ISO 27001 certification
   - Timeline provided for each
   - **Status:** DECISION DEFERRED — requires legal/compliance budget allocation

**Assessment:** All [FOUNDER INPUT REQUIRED] tags are appropriately used. Three of four have clear recommendations. One (compliance gaps) appropriately defers to legal/budget decisions.

---

## Overall Assessment

### Module 6: Product Specification

**Strengths:**
- Comprehensive product flow (7 steps) with clear system logic per step
- Detailed 6 decision sub-steps with data inputs, system logic, adjuster actions, and time targets
- Realistic demo specs with step-by-step screen descriptions and technical requirements
- Strong persona mapping (11 personas with pain points, solutions, and demo screens)
- User journey maps with emotional outcomes (rare in B2B product specs — excellent)

**Weaknesses:**
- Uncited time savings estimates (15-30 min → 2 min, etc.) — critical to value prop but not sourced
- Adoption gradient percentages (5%, 40-60%, 70-90%) appear hypothetical — should be labeled as such
- No UI/UX wireframes or mockups (described but not shown)
- No error handling, data validation, or API schema specifications
- Jargon (STP, FNOL, BI, SIU) used before definition

**Verdict:** **Demo-ready with minor gaps.** An engineer could start building Demo 1 (EU Motor) immediately. Demo 2 (US Property) requires 2-3 weeks of additional design work for coverage determination logic.

### Module 7: Technical Architecture

**Strengths:**
- Clear agent-native architecture philosophy with well-articulated trade-offs vs. traditional software
- Honest current stack assessment (what exists, what doesn't, what's proven)
- Realistic OCR accuracy roadmap with dataset size constraints acknowledged
- Comprehensive integration map (open vs. partner-gated vs. locked) — critical for sales
- Strong compliance section (GDPR, AI Act, US state regulation) with architectural responses
- All [FOUNDER INPUT REQUIRED] tags have clear recommendations

**Weaknesses:**
- Multi-agent architecture decision (Section 7.3) lacks decision matrix with selection criteria
- No cost modeling (cloud costs, API costs, fine-tuning costs) — important for runway planning
- No CI/CD, testing strategy, or deployment pipeline specifications
- No incident response, monitoring, or SLA specifications

**Verdict:** **Investor/CTO-ready with one gap.** The multi-agent architecture decision should have a decision matrix (complexity vs. cost vs. latency vs. debuggability). Otherwise, this is a strong technical spec.

---

## Recommendations for Revision

### High Priority (Before Investor Deck Finalization)

1. **Module 6, Section 6.2:** Add [SOURCE: claims_journey_discovery.md, Phase X] citations for all time savings estimates OR label them [ESTIMATED] if not empirically sourced.

2. **Module 6, Section 6.8:** Label the adoption gradient table (lines 746-752) as [HYPOTHETICAL MODEL] or provide empirical source.

3. **Module 6, New Section 6.12:** Add "API & Data Schema Specifications" with JSON schemas for claim object, decision object, and SOP workflow object.

4. **Module 7, Section 7.3:** Add a decision matrix for multi-agent architecture with criteria: complexity, cost, latency, debuggability, time-to-ship.

### Medium Priority (Before Demo Build Starts)

5. **Module 6, Section 6.9:** Cut Demo 3 (Historical Data Flywheel) from "must show" and move to "investor deck slide only." It's not achievable for a pre-launch demo.

6. **Module 6, Section 6.9:** Add UI/UX wireframes for at least the adjuster dashboard and the 6 decision sub-step cards.

7. **Module 7, Section 7.3:** Add cost modeling (cloud costs, API costs, fine-tuning costs) to inform runway planning.

### Low Priority (Post-Launch Documentation)

8. **Module 6, Section 6.1:** Add a glossary of insurance and technical jargon at the start of the module.

9. **Module 7, Section 7.3:** Add CI/CD, testing strategy, monitoring, and SLA specifications (required for enterprise sales but not for MVP).

---

## Final Verdict

**Module 6: Product Specification** — 8.5/10
**Module 7: Technical Architecture** — 9/10

Both modules are **investor-ready** with minor citation gaps. Module 6 is **demo-ready** for Demo 1 (EU Motor); Demo 2 (US Property) requires 2-3 weeks of additional design work. Module 7 is **CTO-ready** with one decision matrix gap.

**Overall recommendation:** APPROVE for FOS v1.0 with the high-priority revisions listed above.
