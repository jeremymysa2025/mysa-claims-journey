# Mysa Claims Journey Discovery — Summary for Co-founders

### What We Did
Deep product discovery mapping the complete insurance claims journey for **Motor** and **Home/Property** insurance, followed by exhaustive competitive analysis, market sizing, and strategic thesis development. Not surface-level — we went phase by phase, researching how things actually work, challenging assumptions, and identifying where the real gaps are.

**Output:**
- 2000+ line discovery document with detailed journey mapping (`claims_journey_discovery.md`)
- 2100+ line competitive deep dive with market sizing and strategic theses (`home_property_competitive_deep_dive.md`)
- Competitive landscape reality check (`competitive_landscape_reality_check.md`)
- Interactive service blueprint visualization (React app)
- 46 tracked assumptions
- 20+ strategic insights
- GitHub repo: https://github.com/tiago-brigido/mysa-claims-journey

---

## Key Discovery #1: The STP Reality Gap (Motor)

**The conventional wisdom is wrong.**

Everyone says EU convention systems (IRSA, CIMPAS, CID) auto-resolve 60-70% of motor claims. We dug deeper:

- **Theoretical STP:** 60-70% of claims *could* auto-resolve
- **Actual STP:** Only ~10% achieve straight-through processing
- **The gap:** 50+ percentage points

**Why?** The convention lookup is trivial — it's just a database query matching checkboxes to fault percentages. **The bottleneck is data quality:**
- ~50% of EAS forms are still paper
- Filled out by stressed people with shaking hands
- Messy diagrams, unclear checkboxes, missing fields

**The opportunity:** Whoever fixes data quality upstream unlocks the 50+ point STP gap. The convention system isn't the problem — garbage data going IN is the problem.

---

## Key Discovery #2: EU vs US Are Fundamentally Different

| | **EU** | **US** |
|---|---|---|
| **Documentation** | EAS — single agreed document signed by both | Competing narratives, no joint document |
| **Fault determination** | Convention lookup tables | Human investigation every time |
| **FNOL** | "Here's my EAS" (verification) | "Let me tell you what happened" (data collection) |
| **Adjuster involvement** | Often NO for clean claims | Almost ALWAYS — even for fender benders |

**Implication:** Different automation opportunities. EU = fix data quality to unlock STP. US = reduce adjuster time on the 4 recorded statements per claim.

---

## Key Discovery #3: Home Claims Are Structurally Different

| | **Motor** | **Home** |
|---|---|---|
| Counterparty? | YES | Usually NO |
| Agreed document? | EAS | NONE |
| Question to answer | WHO caused it? | WAS it covered? |
| STP possible? | ~10% (EU) | Very rare |
| Adjuster? | Often skipped (EU) | Almost always needed |

**Unlike motor, EU has no structural advantage for home claims.** No EAS, no convention system. The home/property opportunity is the SAME in both EU and US markets.

**The opportunity is different:** Not "unlock STP" but "make adjusters 3x more productive."

---

## Key Discovery #4: AI Replacing Adjusters Is Overhyped (For Home)

**What AI can do:** Detect visible damage, measure from photos, process documents, flag fraud patterns

**What AI cannot do:**
- See hidden damage (water behind walls, mold, structural)
- Determine causation ("sudden burst" vs "gradual leak" — coverage depends on this)
- Handle complex coverage interpretation
- Current accuracy ~70%, needs >95% for high-risk automation

**Realistic opportunity:** Augment adjusters (3x productivity), not replace them.

---

## Key Discovery #5: The Competitive Landscape Is Crowded But Has Clear Gaps

**The crowded spaces (don't go here):**
- FNOL/intake automation: Assured, FurtherAI, Avallon, Sprout.ai, Strada
- Auto casualty guidance: CCC + EvolutionIQ ($730M acquisition)
- Fraud detection: Shift Technology ($320M raised, 25+ countries)
- Motor damage estimation: Solera/Audatex (EU monopoly), CCC (US auto)
- Property estimation: Verisk/Xactimate (US monopoly, 75-80% market share)

**The confirmed gaps — what nobody has built:**
- EU convention system automation (EAS → structured data → convention match → STP)
- Standalone adjuster decision copilot for property/commercial (coverage, triage, reserve)
- Coverage determination + causation analysis AI (the "was it covered?" decision)
- US + EU in a single product

**Key competitors to watch:**
- **Shift Technology** — Most dangerous EU competitor. Launched "Shift Claims" Sept 2025 with agentic AI. AXA Switzerland reports 60% automation rate.
- **Five Sigma/Clive** — Adjuster copilot on any CMS. $20M raised. Landed Starr Jan 2026. 70% US, 30% EU.
- **Verisk/XactAI** — Bundling basic AI free inside Xactimate. Photo labels and transcription today, but they have the data moat to build more.
- **Crawford/Turvi CoverAI** — AI coverage review, closest to the property decision layer. But proprietary to Crawford's TPA stack.
- **Solera/Audatex** — EU motor estimation monopoly. 4.5B+ images. Could build upstream to fault determination.
- **Bdeo** — Spanish startup, visual intelligence for motor + property. 7 of 10 top Spanish auto insurers. 20 countries.
- **Tractable** — Computer vision for motor damage. Aviva (UK), Admiral Seguros (PT/ES).

---

## Key Discovery #6: The Market Is Bigger Than Expected

### US Market
| Segment | Count | Revenue/Premium |
|---------|-------|----------------|
| P&C Carriers | ~4,100 entities | $1.06T DWP |
| TPAs | ~300-500 significant | $115B market |
| MGAs | ~850-1,000+ | $114B managed premium (16% YoY growth) |
| Brokers/Agencies | ~39,000 independent P&C | $262B revenue |
| Adjusting Firms | ~53,000 businesses | $11.7B market |
| **Total claims/year** | **~45-50M** | **$632B losses + LAE** |

### EU Market
| Segment | Count | Revenue/Premium |
|---------|-------|----------------|
| Insurers | ~2,141 undertakings | ~€400-450B GWP |
| Brokers | ~€261B intermediated GWP | ~€59B revenue |
| TPAs | Growing (Davies, Sedgwick, Crawford) | $91B market |
| MGAs | 650+ | €18B GWP (23% CAGR) |
| **Total claims/year** | **~55-70M** | **~€300-350B claims paid** |

### Combined Addressable Market
- **~2,270 potential buyer companies**
- **~100-120M claims/year across both markets**
- **$200-650M TAM (initial sale), $400M-1.3B with land-and-expand**

---

## The Three Strategic Theses

### Thesis 1: EU Motor — Convention STP Gap
**The opportunity:** Fix EAS data quality to unlock the 50-point gap between theoretical (60-70%) and actual (10%) STP rates.
**The wedge:** EAS digitization (OCR + document understanding) → convention matching → automated settlement.
**The buyer:** ~250-400 mid-market EU insurers (regional mutuals heavy).
**The moat:** Country-by-country convention system expertise.
**The risk:** Shift Technology adds EAS processing to Shift Claims.

### Thesis 2: US — Adjuster Decision Copilot
**The opportunity:** Nobody builds the decision layer between FNOL intake and estimation — coverage, triage, investigation, reserve setting.
**The wedge:** AI decision layer that works on any CMS without ripping out infrastructure.
**The buyer:** ~500-600 mid-market carriers + 50-100 TPAs + 200+ MGAs with claims authority.
**The moat:** Decision ground truth data (capturing WHY adjusters decide what they decide).
**The risk:** Verisk builds real decision AI into Xactimate.

### Thesis 3: Home/Property — Coverage + Causation AI (Both Markets)
**The opportunity:** Coverage determination ("was this sudden or gradual?") and causation analysis are unaddressed. Unlike motor, EU has NO structural advantage here — same problem both sides.
**The wedge:** Coverage recommendation engine with human-in-the-loop.
**The buyer:** Carriers + TPAs (US), carriers directly (EU — perito model).
**The moat:** Historical coverage decision patterns as training data.
**The risk:** Coverage determination may be too hard to automate reliably (policy language interpretation + physical evidence + causation timeline = complex). Crawford/Turvi CoverAI goes standalone.

### How They Sequence
The theses are complementary. EAS digitization (Thesis 1) builds OCR + document understanding + structured decision logic that transfers to property coverage AI (Thesis 3). The US adjuster copilot (Thesis 2) is essentially Thesis 3 with different packaging. The question is which market and which line to land first.

---

## What's Mapped

**Motor (phases 0-6 complete):**
- Incident → Scene Management → Documentation → Reconciliation → First Contact → FNOL → Triage
- 8 decision forks with branching logic
- EU vs US differences at every phase

**Home/Property:**
- FNOL process
- Adjuster workflow (desk vs field)
- TPA landscape (Sedgwick, Crawford, Davies — deep competitive analysis)
- 3x productivity opportunity
- AI limitations honest assessment

**Competitive & Market Analysis (22 sections):**
- TPA competitive teardown (Sedgwick, Crawford, Davies — what they've built, what they haven't)
- Measurement/documentation tools (Hover, CAPE, EagleView, Encircle)
- Estimation monopoly (Verisk/Xactimate US, Solera/Audatex EU)
- AI startup landscape (Assured, Five Sigma, Avallon, Sprout.ai, Shift, Tractable, Bdeo, ClaimSorted, Afori)
- EU competitive landscape + perito model
- STP reality gap deep dive with convention system analysis
- EU SME insurer market (document intake, parsing, agent management)
- Venture-scale math (STP gap vs property adjuster OS)
- US adjuster workforce crisis (12th fastest-declining profession)
- 4 strategic paths evaluated
- Complete market sizing — all buyer types, both markets
- Three contrarian bet theses refined (US, EU motor, home/property)
- Sequencing strategy

**Not yet mapped:**
- Motor phases 7-11 (Investigation → Settlement → Close)
- Repair networks, subrogation, fraud workflows

---

## Next Steps

1. **Validate theses with real customers** — Talk to 5-10 mid-market EU insurers about EAS pain, 5-10 US carriers/TPAs about adjuster decision workflow
2. Continue mapping motor phases 7-11 (investigation, assessment, settlement)
3. Decide sequencing: EU motor STP first? US property copilot first? Both?
4. Build proof-of-concept for the chosen wedge
5. Go deeper on repair networks / direct repair programs
6. Validate STP assumptions with actual insurer data

---

*Full details in the GitHub repo. The README has instructions for continuing the research.*
