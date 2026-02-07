# Mysa Claims Journey Discovery

> Product discovery for Mysa — an AI-native claims automation platform. Mapping the complete claims journey across Motor and Home/Property insurance to identify pain points, automation opportunities, and strategic positioning.

---

## How We Work Together (Instructions for Claude)

**This is NOT a "just document what I say" project.** This is collaborative product discovery where Claude is expected to:

### 1. Push Back and Challenge
- Don't accept assumptions at face value — question them
- If something seems wrong or incomplete, say so
- Ask "is that actually true?" and "where does that data come from?"
- Flag when we're making assumptions vs stating facts

### 2. Go Deep on Each Topic
- Don't skim — we research each topic thoroughly before moving on
- Use web searches to find real data, industry reports, actual processes
- Understand the WHY behind each step, not just the WHAT
- Explore edge cases and exceptions — that's where complexity lives

### 3. Jam First, Document Second
- We discuss and debate topics BEFORE writing them into the document
- Research → Discussion → Challenge → Agreement → THEN document
- Don't jump to documentation before we've explored the topic
- It's okay to go back and revise earlier conclusions

### 4. EU vs US Always
- Every topic must consider both markets
- The differences are fundamental — not surface-level
- Flag when we're talking about one market vs the other
- Different automation opportunities exist in each

### 5. Be Honest, Not Validating
- If an idea is bad, say so
- If we're missing something important, point it out
- Don't agree just to be agreeable
- The goal is truth, not confirmation

### 6. Strategic Implications
- Don't just map processes — understand what they mean for Mysa
- Where does pain live? Where is the money? Who has budget?
- What can be automated vs what needs humans?
- Where's the moat?

---

## What This Project Is

We're building a **granular, detailed map of the insurance claims journey** to inform product strategy for Mysa. This isn't a high-level overview — it's a deep dive into:

- **Who does what, when, and why** in a claims process
- **Where the friction, pain, and cost lives** (that's where automation value is)
- **How EU and US markets differ** (fundamentally, not superficially)
- **What can be automated** and what still needs humans
- **Where Mysa fits** in this landscape — with honest competitive analysis

### The Approach

We use a **service blueprint** model because claims aren't linear — they involve:
- Multiple actors (policyholder, insurer, broker, adjuster, repair shop, etc.)
- Parallel activities (things happening simultaneously)
- Decision forks (branching paths based on conditions)
- Handoffs (data and responsibility moving between actors)

### Repository Contents

| File | Description |
|------|-------------|
| `claims_journey_discovery.md` | Main discovery document (~2000+ lines) — the full motor + home journey mapping with research, assumptions, and insights |
| `home_property_competitive_deep_dive.md` | Deep competitive analysis (~2100+ lines) — TPA teardowns, startup landscape, market sizing, strategic theses |
| `competitive_landscape_reality_check.md` | High-level competitive reality check — who's building what, why it hasn't been "solved" |
| `SUMMARY.md` | Co-founder summary — key discoveries, theses, and market sizing |
| `claims_service_blueprint.jsx` | React component for interactive visualization |
| `app/` | Vite React app to run the blueprint locally |
| `README.md` | This file — overview and continuation instructions |

---

## How to Run the Visualization

```bash
cd app
npm install
npm run dev
# Open http://localhost:5173
```

**Blueprint structure:**
- **Rows** = Actors (policyholder, counterparty, police, broker, insurer front office, claims handler, adjuster, etc.)
- **Columns** = Phases (Incident → Scene Mgmt → Documentation → ... → Close)
- **Cells** = What each actor does in each phase
- **Forks** = Decision points (click to see the branching logic)

---

## What We've Discovered and Documented

### Motor Claims Journey (Phases 0-6)

#### Phase 0: Incident (Seconds 0-60)
- Mapped the reality of what happens in the first minute (chaos, not paperwork)
- Shock/adrenaline state, safety assessment
- No documents yet — just dashcam/telematics if they exist

#### Phase 1: Scene Management (Minutes 1-30)
**Fork 1: Anyone Injured?** YES → BI claim path | NO → Material damage only
**Fork 2: Is the Other Party Cooperative?** Cooperative → Exchange info | Uncooperative → Police | Hit and run → Guarantee fund

#### Phase 2: Documentation — The Massive EU/US Divergence
**Fork 3: EU vs US Market**
- EU: European Accident Statement (EAS) — standardized form, ~50% still paper, "brilliant concept, terrible execution"
- US: No equivalent — police reports, competing narratives, 4 recorded statements per fender bender

#### Phase 3: Reconciliation — How Fault Gets Determined
- EU: Convention systems (IRSA, CIMPAS, CID) — pre-computed fault lookup tables
- US: Manual investigation every time — no convention system
- **THE STP REALITY GAP:** 60-70% theoretical STP vs ~10% actual. Bottleneck = data quality.

#### Phase 4: First Contact
**Fork 4: Distribution Channel** (Broker / Agent / Direct)
**Fork 5: Broker Submission Method** (Portal / Email / Phone — all have friction)

#### Phase 5: FNOL
- EU = verification workflow ("here's my EAS")
- US = data collection workflow ("let me tell you what happened")

#### Phase 6: Triage
**Fork 6: Skip Adjuster or Assign?**
- EU: Goal is to skip adjuster — ~10% achieve STP
- US: Every claim gets adjuster — the question is "which one?"

### Home/Property Claims

#### Why Structurally Different
| | Motor | Home |
|---|---|---|
| Counterparty? | YES | Usually NO |
| Agreed document? | EAS (EU) | NONE |
| Core question | WHO caused it? | WAS it covered? |
| Convention system? | EU: Yes | NONE — anywhere |
| EU advantage? | YES (EAS, conventions) | NO |

#### Key Findings
- Desk vs field adjuster shift: 80/20 → 60/40 → trending to 40/60
- TPAs employ 25-35% of adjusters — massive buyer segment
- 3x adjuster productivity opportunity (travel 25-30%, documentation 20-25% = automate)
- AI replacing adjusters is overhyped — augment, not replace (hidden damage, causation, fraud)

### Competitive Deep Dive (22 Sections)

**TPA Competitive Teardown:**
- Sedgwick ($5B, smart.ly intake, Sidekick Agent, JURIS legacy CMS — does NOT license tech)
- Crawford ($1.29B, Turvi/CoverAI coverage review, Contractor Connection 6K+ contractors, WeGoLook)
- Davies ($1B+, ClaimPilot, agentic AI features, 200K+ claims/year)

**The Estimation Monopolies:**
- US Property: Verisk/Xactimate (75-80% market share) + XactAI (Sept 2025, basic AI bundled free)
- EU Motor: Solera/Audatex (4.5B+ images, Qapter AI photo-to-estimate)

**AI Startup Landscape:**
| Company | Focus | Funding | Market |
|---------|-------|---------|--------|
| Five Sigma/Clive | Adjuster copilot on any CMS | $20M | 70% US, 30% EU |
| Shift Technology | Fraud → full claims automation | $320M | 25+ countries |
| Assured | Document intake + triage | Funded | US |
| Sprout.ai | Claims intake automation | Funded | UK, EU, LATAM |
| Tractable | Computer vision motor damage | Funded | UK, EU (Aviva, Admiral) |
| Bdeo | Visual intelligence motor + property | Funded | 20 countries (7/10 Spanish auto) |
| Avallon | AI agents for calls/emails/docs | $4.6M | US |
| ClaimSorted | AI-first TPA | €11.4M | UK, EU, US |

**Market Sizing:**
| | US | EU | Combined |
|---|---|---|---|
| Market size | $1.06T DWP | ~€400-450B GWP | ~$1.5T |
| Total claims/year | ~45-50M | ~55-70M | ~100-120M |
| Addressable buyers | ~1,250 | ~1,020 | ~2,270 |
| TAM (initial sale) | $138-468M | €70-196M | $200-650M |
| TAM (with expansion) | $276-936M | €140-392M | $400M-1.3B |

### Three Strategic Theses (Refined)

**Thesis 1 — EU Motor: Convention STP Gap**
Fix EAS data quality → convention matching → unlock 50+ point STP gap. Nobody builds this. ~250-400 mid-market EU carriers. Risk: Shift Technology.

**Thesis 2 — US: Adjuster Decision Copilot**
AI decision layer between FNOL and estimation — coverage, triage, reserve. Works on any CMS. ~800 buyers. Risk: Verisk builds real AI into Xactimate.

**Thesis 3 — Home/Property (Both Markets): Coverage + Causation AI**
Coverage determination ("sudden vs gradual?") and causation analysis are unaddressed everywhere. EU has NO structural advantage for property. Same problem both sides. Risk: too hard to automate reliably.

**The theses are complementary and can be sequenced.** EU motor STP builds capabilities (OCR, document understanding, decision logic) that transfer to property coverage AI.

---

## Decision Forks Documented

| Fork | Title | Phase | Key Decision |
|------|-------|-------|--------------|
| F1 | Anyone Injured? | Scene Mgmt | BI claim vs material damage |
| F2 | Cooperative? | Scene Mgmt | Clean path vs disputed vs hit-and-run |
| F3 | EU vs US | Documentation | EAS vs competing narratives |
| F4 | First Contact | First Contact | Broker vs Agent vs Direct |
| F5 | Broker Submission | First Contact | Portal vs Email vs Phone |
| F6 | Triage | Triage | Skip adjuster vs assign |
| F7 | Motor vs Home | Cross-LOB | Structural differences |
| F8 | Desk vs Field | Home Triage | Virtual vs on-site inspection |

---

## Assumptions Tracked

All assumptions are logged with status:
- Validated
- Needs validation
- Disproven

**Currently 46 assumptions tracked (A1-A46)** covering EAS paper vs digital split, convention system STP rates, distribution channel percentages, adjuster employment breakdown, AI accuracy requirements, and more.

---

## What's NOT Done Yet

### Motor Claims — Remaining Phases
- **Phase 7: Investigation** — What does the adjuster actually DO? Expert inspections?
- **Phase 8: Assessment** — Damage valuation, repair estimates
- **Phase 9: Decision** — Coverage determination, liability finalization
- **Phase 10: Settlement** — Payment mechanics, negotiation
- **Phase 11: Close** — Subrogation, recovery, file closure

### Other Topics to Explore
- Repair network / direct repair programs
- Subrogation and recovery between insurers
- Fraud detection workflows (SIU deep dive)
- Cross-border claims in EU
- Total loss vs repair decision
- Rental car / mobility during repair
- Customer validation interviews (5-10 per market)

### Other Lines of Business
- **Health Insurance** — Noted as fundamentally different (request-approval workflow, not event-response). Deprioritized but may revisit.

---

## How to Continue This Work

### Starting a New Session

1. Share this README with Claude
2. Reference the relevant docs:
   - `claims_journey_discovery.md` — for journey mapping and phase-by-phase detail
   - `home_property_competitive_deep_dive.md` — for competitive analysis, market sizing, and strategic theses
   - `competitive_landscape_reality_check.md` — for high-level competitive overview
   - `SUMMARY.md` — for quick context on key discoveries
3. State where you want to pick up, for example:
   - "Let's continue with Phase 7 (Investigation) for motor claims"
   - "Let's validate the EU motor thesis with customer interviews"
   - "Let's go deeper on Verisk/XactAI as a competitive threat"
   - "Let's refine the sequencing strategy"
   - "Let's explore repair networks"

### Remember the Working Style
- **Jam first, document second** — Research and debate before writing
- **Push back and challenge** — Question assumptions, ask for evidence
- **Go deep** — Don't skim, explore the topic thoroughly
- **EU vs US always** — Every topic should consider both markets
- **Update everything** — Keep the MD files, blueprint, and assumptions in sync

### Key Open Questions
1. Which thesis to pursue first? EU motor STP or US adjuster copilot?
2. How fast is Verisk moving XactAI from features to platform?
3. Will Shift Technology add EAS processing to Shift Claims?
4. Can coverage determination be automated reliably enough (>95%)?
5. What do mid-market carriers actually spend on claims tech today?
6. How do repair networks and direct repair programs work?
7. What happens in motor phases 7-11 (investigation → settlement)?

---

## Commands Reference

```bash
# Run the visualization
cd app && npm run dev

# Sync blueprint to app after editing the JSX
cp claims_service_blueprint.jsx app/src/App.jsx

# Search across all discovery docs
grep -rn "keyword" *.md
```

---

## Session History

### Session 1 (February 2025)
**Motor claims journey mapping**
- Documented phases 0-6 (Incident → Triage) with EU vs US differences at every phase
- Discovered the STP reality gap (10% actual vs 60-70% theoretical)
- Documented EAS data schema and convention systems
- Created 6 decision forks, 46 assumptions, 12 strategic insights
- Built interactive service blueprint visualization (React app)

### Session 2 (February 2025)
**Home/property claims analysis**
- Documented home/property FNOL process
- Researched adjuster workflow (desk vs field), TPA employment
- Explored EU vs US differences for property (no structural EU advantage)
- Documented 3x adjuster productivity opportunity
- Honest assessment of AI replacing adjusters
- Added assumptions A34-A46, insights #13-20, Forks 7-8
- Created GitHub repo and pushed everything

### Session 3 (February 7, 2026)
**Competitive deep dive + market sizing + strategic theses**
- Deep TPA competitive teardown (Sedgwick, Crawford, Davies — tech stacks, gaps, what they DON'T have)
- Mapped measurement/documentation tools (Hover, CAPE, EagleView, Encircle)
- Analyzed estimation monopolies (Verisk/Xactimate US, Solera/Audatex EU)
- Researched AI startup landscape (Assured, Five Sigma, Shift Technology, Tractable, Bdeo, Sprout.ai, Avallon, ClaimSorted, Afori)
- Deep EU competitive landscape including perito model, convention systems, EU-specific dynamics
- STP reality gap deep dive with convention system analysis across countries
- EU SME insurer market analysis (document intake, parsing, agent management)
- Venture-scale math (STP gap vs property adjuster OS — unit economics, TAM)
- US adjuster workforce crisis analysis
- Evaluated 4 strategic paths
- Analyzed why nobody builds for the hard part of adjusting
- Unbiased opportunity assessment comparing all approaches
- **Complete market sizing** — all buyer types (carriers, TPAs, MGAs, brokers, adjusting firms) for both US and EU
  - US: $1.06T market, ~4,100 carriers, ~45-50M claims/year
  - EU: ~€400-450B market, ~2,141 undertakings, ~55-70M claims/year
  - Combined addressable: ~2,270 companies, $200-650M TAM ($400M-1.3B with expansion)
- **Refined three strategic theses:**
  - Thesis 1: EU Motor — Convention STP gap (EAS data quality → convention matching)
  - Thesis 2: US — Adjuster decision copilot (coverage/triage/reserve AI on any CMS)
  - Thesis 3: Home/Property both markets — Coverage + causation AI (the hardest problem)
- Honest competitive threat analysis (Verisk/XactAI, Shift Technology, Five Sigma/Clive, CCC/EvolutionIQ, Solera/Audatex, Crawford/Turvi, Bdeo, Tractable)
- Sequencing strategy for how the three theses fit together

**Where we left off:**
Motor phases 0-6 mapped. Home/property analyzed. Full competitive landscape documented. Market sized. Three strategic theses refined with honest risk assessment. Next: customer validation, motor phases 7-11, or deeper competitive monitoring.
