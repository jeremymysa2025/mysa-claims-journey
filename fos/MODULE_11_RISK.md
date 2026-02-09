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
