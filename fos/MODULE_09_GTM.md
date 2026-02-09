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
