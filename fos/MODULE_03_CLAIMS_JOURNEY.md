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
