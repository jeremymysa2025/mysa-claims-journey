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
- **Where Mysa fits** in this landscape

### The Approach

We use a **service blueprint** model because claims aren't linear — they involve:
- Multiple actors (policyholder, insurer, broker, adjuster, repair shop, etc.)
- Parallel activities (things happening simultaneously)
- Decision forks (branching paths based on conditions)
- Handoffs (data and responsibility moving between actors)

### Repository Contents

| File | Description |
|------|-------------|
| `claims_journey_discovery.md` | Main discovery document (~2000+ lines) — the full journey mapping with research, assumptions, and insights |
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
- **Forks** = Decision points (click 🔍 to see the branching logic)

---

## What We've Discovered and Documented

### Motor Claims — The Primary Focus

#### Phase 0: Incident (Seconds 0-60)
- Mapped the reality of what happens in the first minute (chaos, not paperwork)
- Shock/adrenaline state, safety assessment
- No documents yet — just dashcam/telematics if they exist

#### Phase 1: Scene Management (Minutes 1-30)
**Fork 1: Anyone Injured?**
- YES → Call 112/911 → Police take over → Bodily Injury claim path (totally different animal: higher value, longer lifecycle, lawyers)
- NO → Material damage only → Fork 2

**Fork 2: Is the Other Party Cooperative?**
- COOPERATIVE → Exchange info, fill EAS (EU) or exchange insurance cards (US)
- UNCOOPERATIVE → Call police, no joint statement possible
- HIT AND RUN → Police, guarantee fund path, may never identify other driver

#### Phase 2: Documentation — The Massive EU/US Divergence
**Fork 3: EU vs US Market**

**🇪🇺 Europe: European Accident Statement (EAS)**
- Standardized carbon-copy form across entire EU
- "Brilliant concept, terrible execution" — two stressed people drawing diagrams
- ~50% still on paper
- Single source of truth — both parties sign the same document
- Pre-agreed checkboxes map to convention fault tables

**🇺🇸 United States: No Equivalent**
- Police crash report (narrative text, not structured)
- Each driver's own photos and account
- Two competing narratives — no agreed document
- Up to 4 recorded statements for a single fender bender

**Key insight:** EU produces structurally cleaner data at origin. This is a fundamental difference, not a minor one.

#### Phase 3: Reconciliation — How Fault Gets Determined

**🇪🇺 Europe: Convention Systems**
- CIMPAS (Portugal), IDA/IRSA (France), CID (Italy)
- Pre-computed fault tables — given accident type X, fault = Y/Z
- "Lookup tables for fault" — no investigation needed for matching scenarios
- **THE STP REALITY GAP DISCOVERY:**
  - Theoretical STP potential: 60-70% of claims could auto-resolve
  - Actual STP achieved: Only ~10%
  - **Bottleneck:** Data quality — messy EAS forms, unclear diagrams, paper, missing fields
  - **The convention lookup is trivial** — a simple database query
  - **The opportunity:** Whoever fixes data quality upstream unlocks the 50+ point gap

**🇺🇸 United States: Manual Investigation**
- No convention system for routine claims
- Every disputed claim needs human investigation
- Recorded statements from both drivers (15-30 min each)
- Adjuster reconstructs what happened from competing accounts
- Fault percentage assigned (not binary — can be 80/20, 70/30, etc.)
- Inter-company arbitration if insurers disagree

#### Phase 4: First Contact — Who Does the Policyholder Call?
**Fork 4: Distribution Channel**
- **BROKER** (UK/NL/BE dominant) → Calms, guides, submits FNOL
- **AGENT** (IT/DE/PT/ES dominant, US personal lines)
  - Captive → Direct system access
  - Independent → Directs to insurer
- **DIRECT** (growing everywhere) → Fastest, no intermediary

**Fork 5: How Does Broker Submit to Insurer?**
- **Portal** → Manual rekeying into insurer's system (friction)
- **Email** → Double entry — broker types it, insurer re-keys (more friction)
- **Phone** → Fastest to open, but docs arrive separately

**Key insight:** Broker-to-insurer submission is a data quality bottleneck. All paths have friction.

#### Phase 5: FNOL (First Notice of Loss)
**Fundamental difference:**
- 🇪🇺 EU FNOL = "Here's my EAS, verify my policy" (verification workflow)
- 🇺🇸 US FNOL = "Let me tell you what happened" (data collection workflow)

**EAS Data Schema documented:**
- ~100 fields total
- 17 circumstance checkboxes that map to convention fault tables
- The checkboxes ARE the convention input

#### Phase 6: Triage
**Fork 6: Skip Adjuster or Assign?**

**🇪🇺 EU (goal: skip adjuster)**
- Clean EAS → Convention match → STP (~10% actual)
- Unclear EAS → Clarification call → Maybe adjuster
- Complex/BI → Full investigation

**🇺🇸 US (every claim gets adjuster)**
- No STP path — even simple claims get adjuster time
- The question is "which adjuster?" not "do we need one?"

**Where claims handlers actually spend time:**
- Data extraction & reconciliation: ~30%
- Exception handling: ~25%
- Damage assessment coordination: ~20%
- Validation & compliance: ~15%
- Policy lookup & payment: ~10%

**The first 55% (data extraction + exception handling) is the prime automation target.**

---

### Home/Property Claims — Added for Comparison

#### Why Home Claims Are Structurally Different
| | Motor | Home |
|---|---|---|
| Counterparty? | YES — another driver | Usually NO — you vs the peril |
| Agreed document? | 🇪🇺 EAS | NONE |
| Fault question? | WHO caused it? | WAS it covered? |
| Convention system? | 🇪🇺 Yes | NONE |
| STP possible? | ~10% actual | Very rare |
| Adjuster involvement | 🇪🇺 Often NO | Almost ALWAYS |

#### Claim Types (US 2019-2023)
- Wind & hail: 42.5%
- Water damage: 29.4%
- Fire & lightning: ~5%
- Theft: 0.7%

#### What Home Adjusters Do
**Two parts:**
1. INVESTIGATION — Establish the facts (what happened, was it covered, is it fraud?)
2. VALUATION — Estimate the cost (Xactimate is industry standard, used by 75-80%)

#### Desk Adjuster vs Field Adjuster
- **Desk:** Small claims (<$3K), simple causation, virtual inspection
- **Field:** Large/complex claims, hidden damage possible, on-site inspection

**The shift:**
- Past: Field 80% / Desk 20%
- Today: Field 60% / Desk 40%
- Future: Field 40% / Desk 60%

#### Who Employs Home Adjusters
- Staff adjusters (insurer employees): ~40-50%
- TPA adjusters (Crawford, Sedgwick, Engle Martin): ~25-35%
- Independent adjusters: ~15-25%
- Public adjusters (work for policyholder): ~5%

**Key insight:** TPAs are a massive buyer segment — improving their unit economics is a direct value prop.

#### The 3x Adjuster Productivity Opportunity
Where field adjusters spend time:
- Travel: ~25-30% (biggest lever — eliminate with virtual)
- Documentation & data entry: ~20-25% (automate)
- On-site inspection: ~15-20%
- Report writing: ~10-15% (AI draft generation)
- Xactimate/estimates: ~10-15%
- Communication: ~10-15%

**The opportunity is NOT "replace the adjuster" — it's "make the adjuster 3x more productive."**

#### Can AI Replace Adjusters? (Honest Assessment)
**What AI can do:**
- Damage detection from photos (visible damage)
- Measurement from photos/video (3D scanning)
- Document processing
- Fraud pattern detection

**What AI cannot do well:**
- Hidden damage (water behind walls, mold, structural)
- Causation determination ("was this sudden or gradual?")
- Complex coverage interpretation
- Settlement negotiation
- Fraud investigation

**The accuracy problem:** Current AI ~70%, needs >95% for high-risk automation.

**The fraud problem:** AI is making fraud EASIER (fake photos, receipts, documents). Adversarial dynamic matters.

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

## Key Strategic Insights (20 Total)

### Motor Claims
1. Europe produces structurally cleaner data at origin (EAS)
2. Convention systems are trivial lookups — data quality is the bottleneck
3. The STP reality gap (10% actual vs 60-70% theoretical) IS the opportunity
4. US is incredibly labor-intensive even for simple claims
5. Broker-to-insurer submission is a data quality bottleneck
6. EU FNOL = verification, US FNOL = data collection

### Home Claims
7. Home claims are structurally different — no counterparty, no EAS, no convention
8. Unlike motor, EU has no structural advantage for home
9. Motor automation = fix data quality. Home automation = make adjusters productive.
10. TPAs are a massive buyer segment
11. "Replace adjuster with AI" is overhyped — augment, not replace
12. Hidden damage and fraud risk limit pure automation

---

## Assumptions Tracked

All assumptions are logged with status:
- ✅ Validated
- ⚠️ Needs validation
- ❌ Disproven

**Currently 46 assumptions tracked (A1-A46)** covering:
- EAS paper vs digital split
- Convention system STP rates
- Distribution channel percentages
- Adjuster employment breakdown
- AI accuracy requirements
- And more...

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

### Other Lines of Business
- **Health Insurance** — Noted as fundamentally different (request-approval workflow, not event-response). Deprioritized but may revisit.

---

## How to Continue This Work

### Starting a New Session

1. Share this README with Claude
2. Reference the discovery doc if needed: `claims_journey_discovery.md`
3. State where you want to pick up, for example:
   - "Let's continue with Phase 7 (Investigation) for motor claims"
   - "Let's explore how repair networks work"
   - "Let's validate assumption A4 about convention STP rates"
   - "Let's go deeper on [specific topic]"

### Remember the Working Style
- **Jam first, document second** — Research and debate before writing
- **Push back and challenge** — Question assumptions, ask for evidence
- **Go deep** — Don't skim, explore the topic thoroughly
- **EU vs US always** — Every topic should consider both markets
- **Update everything** — Keep the MD file, blueprint, and assumptions in sync

### Key Open Questions
1. What exactly happens during Investigation phase? Who does what?
2. How do repair networks work? Direct repair programs?
3. How does subrogation/recovery work between insurers?
4. What are the actual STP rates by insurer/market? (validate our assumptions)
5. Where does Mysa fit — upstream data quality or downstream adjuster tools? Or both?

---

## Commands Reference

```bash
# Run the visualization
cd app && npm run dev

# Sync blueprint to app after editing the JSX
cp claims_service_blueprint.jsx app/src/App.jsx

# Search for something in the discovery doc
grep -n "keyword" claims_journey_discovery.md
```

---

## Last Session Summary

**Date:** February 2025

**What we did:**
- Documented home/property insurance FNOL process
- Researched what home adjusters actually do
- Broke down desk vs field adjusters
- Documented TPA employment (Crawford, Sedgwick, Engle Martin)
- Explored EU vs US differences for property claims
- Documented the 3x adjuster productivity opportunity
- Gave honest assessment of AI replacing adjusters
- Added 13 new assumptions (A34-A46)
- Added 8 new strategic insights (#13-20)
- Created Fork 7 (Motor vs Home) and Fork 8 (Desk vs Field)
- Created GitHub repo and pushed everything

**Where we left off:**
Motor phases 0-6 complete, Home FNOL complete. Next logical step is Phase 7 (Investigation) for motor claims, or going deeper on any topic that needs more research.
