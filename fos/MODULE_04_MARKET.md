# Module 4: Market Landscape

**Status:** DRAFT v1.0
**Last updated:** February 9, 2026
**Feeds:** Pitch deck slides 3-6 (market), fundraising data room, sales territory planning, board TAM narratives
**Depends on:** Module 1 (Positioning & ICP), Module 2 (Problem)

---

## Glossary

| Term | Definition |
|------|-----------|
| **GWP** | Gross Written Premiums — the total premium income an insurer writes in a period, before reinsurance deductions. The standard measure of insurer size in the EU. |
| **DWP** | Direct Written Premiums — the US equivalent of GWP. Total premiums written directly by an insurer, excluding assumed reinsurance. |
| **STP** | Straight-Through Processing — claims resolved near-instantly with minimal human review, typically via convention system automation. |
| **Convention System** | Standardized inter-insurer protocol for settling motor claims between two insurers (e.g., IDS in Portugal, IRSA in France, CARD in Italy, CIDE in Spain). Defines deterministic rules for fault allocation. |
| **TPA** | Third-Party Administrator — a company that processes claims on behalf of insurance carriers who outsource their claims operations. |
| **MGA** | Managing General Agent — an intermediary with underwriting authority from a carrier, increasingly also handling claims. |
| **ACV** | Annual Contract Value — the annualized revenue from a single customer contract. |
| **Caravela tier** | Mysa's term for the primary target segment: carriers with €100-200M GWP (or $100-500M DWP in the US). Named after design partner Caravela Seguros (€188M GWP). |
| **P&C** | Property and Casualty — the insurance category covering motor, home/property, commercial, and liability. |
| **Cat / Nat Cat** | Catastrophe / Natural Catastrophe — large-scale insured events (floods, earthquakes, wildfires). Drives spikes in claims volume and cost. |
| **CCS** | Consorcio de Compensacion de Seguros — Spain's state reinsurer for catastrophe risk. |
| **CCR** | Caisse Centrale de Reassurance — France's state reinsurer for natural catastrophe risk (Cat-Nat regime). |
| **KGV** | Kantonale Gebaudeversicherung — Swiss cantonal building insurance monopolies (19 of 26 cantons), limiting the private property insurance market. |

---

## 4.1 Global Overview

### The Opportunity at a Glance

The global motor and property claims market processes an estimated **80-95 million claims per year** across the EU and US alone, backed by approximately **$1.5 trillion in combined premiums** (using approximate EUR/USD parity for simplicity). This is the universe in which Mysa operates. [SOURCE: market_landscape_overview.md, Section 1]

### Total Claims Volume — Motor + Property

| Market | Motor Claims/Year | Property Claims/Year | **Combined** |
|--------|------------------|--------------------------|-------------|
| **EU (16 countries)** | ~25-35M | ~16-20M | **~41-55M** |
| **US** | ~35M | ~4.4-4.5M | **~39.5M** |
| **Global total** | **~60-70M** | **~20-25M** | **~80-95M** |

[SOURCE: market_landscape_overview.md, Section 1 — "Total Claims Volume"]

### Total Premium (GWP / DWP)

| Market | Motor GWP/DWP | Property GWP/DWP | **Combined** |
|--------|----------|-------------------|-------------|
| **EU Southern (PT, ES, FR, IT)** | €57.9B | ~€24-28B | **~€82-86B** |
| **EU Northern/Central (12 countries)** | €70-78B | ~€30-33B | **~€100-111B** |
| **EU Total (16 countries)** | **~€128-136B** | **~€54-61B** | **~€182-197B** |
| **US** | ~$359B (auto) | $172.7B (homeowners) | **~$532B** |
| **Global combined** | | | **~€700B+** |

[SOURCE: market_landscape_overview.md, Section 1 — "Total Premium (GWP/DWP)"]

### Motor vs Property: Two Lines, One Market

Motor insurance is the larger line by premium volume, but property is the faster-growing opportunity — particularly in the EU, where mandatory nat cat schemes are expanding coverage and increasing claims volumes. The critical structural insight is that **80-95% of carriers that write motor also write property** — the buyer list is essentially the same. [SOURCE: market_landscape_overview.md, Section 3]

| Dimension | Motor | Property |
|-----------|-------|----------|
| **EU GWP** | ~€128-136B | ~€54-61B |
| **US DWP** | ~$359B | $172.7B |
| **EU claims/year** | ~25-35M | ~16-20M |
| **US claims/year** | ~35M | ~4.4-4.5M |
| **Convention system?** | YES (EU only) — IRSA, CARD, CIDE, IDS | **NONE — anywhere** |
| **Core decision** | WHO caused it? (fault %) | WAS it covered? (policy interpretation) |
| **Estimation monopoly** | Audatex/Solera (EU), CCC/Mitchell (US auto) | Xactimate (US, ~80%), fragmented in EU |
| **AI competition for decisions** | Some (Shift, Five Sigma) | **Almost none** (Crawford CoverAI failed, Wamy pre-traction) |
| **Avg claim size** | ~€1,500-3,000 (EU), ~$5,000 (US) | ~€3,000-8,000 (EU), **$17,059 (US — 3.4x auto)** |
| **Dominant peril** | Collision | **Water damage (38-44% EU), wind/hail (US)** |

[SOURCE: market_landscape_overview.md, Section 3 — "Motor vs Home — Side by Side, Same Carriers"]

### Total Carrier/Buyer Universe

| Market | Total Carriers | TPAs | MGAs | **Total Potential Buyers** |
|--------|---------------|------|------|--------------------------|
| **EU** | ~2,141+ undertakings | ~200-300 | 650+ (€18B GWP, 23% CAGR) | **~3,000+** |
| **US** | ~4,116 P&C entities | ~500-800 | ~330-550 | **~5,000-5,500** |
| **Global** | | | | **~8,000+** |

[SOURCE: market_landscape_overview.md, Section 1 — "Total Carrier/Buyer Universe"]

---

## 4.2 EU Market by Country

This section covers all 16 validated EU markets, split into Southern EU (countries with established motor convention systems — the initial wedge) and Northern/Central EU (mixed or no convention systems — expansion markets).

All data sourced from validated regulatory filings and industry bodies: ASF (Portugal), DGSFP/ICEA (Spain), ACPR/France Assureurs (France), IVASS/ANIA (Italy), BaFin (Germany), DNB (Netherlands), FSMA/Assuralia (Belgium), FMA/VVO (Austria), FINMA/SVV (Switzerland), Central Bank of Ireland, FI Sweden/Svensk Forsakring, FSA Denmark, FIN-FSA Finland, Finanstilsynet Norway, KNF/PIU (Poland), CNB/XPRIMM (Czech Republic), EIOPA, NAIC, AM Best. [SOURCE: mysa_product_strategy.md, Part 9a — full regulatory source list]

---

### 4.2.1 Southern EU (Convention System Countries — The Wedge)

These four countries have established motor convention systems that create a technical wedge for Mysa: deterministic fault rules encoded into inter-insurer settlement protocols. Convention expertise is hard to replicate and creates immediate value for carriers struggling with data quality at convention intake.

#### Motor Insurance

| Country | Convention System | Motor GWP | Registered Vehicles | Total Insurers | Motor Writers | Caravela-Tier Carriers (€100-200M) | Small Carriers (€50-100M) | Convention Detail |
|---------|-------------------|-----------|---------------------|----------------|---------------|-------------------------------------|---------------------------|-------------------|
| **Portugal** | IDS/CIMPAS | **€1.8B** (2023) | ~5.8M light (7.3M total) | ~47 active non-life (63 domestic) | ~25-30 | **6-8** | ~8-12 | 1.94 day avg processing, 91% agreement rate |
| **Spain** | CIDE/ASCIDE/CICOS | **€13.2B** (2024, +8.9%) | **34M** | ~176 operating (187 RAEA) | ~80-100 (31 groups in motor) | **8-10** | ~25-35 | 2.5M claims/year processed through convention |
| **France** | IRSA | **€28.1B** (2024, +7.3%) | **45.5M** | **660** ACPR-supervised (246 FFA, 324 mutuelles, 302 insurance code, 34 social security code) | ~100-120 | **30-60** | ~100+ | 13 cases, deterministic rules |
| **Italy** | CARD | **~€14.8B** (2023) | **~40M** | ~85 national (IVASS) | **38** write RC Auto | **10-15** | ~8-12 | Mandatory for 2-vehicle collisions |
| **Southern EU Total** | **All have convention** | **€57.9B** | **~125M** | | | **54-93** | **141-159+** | |

[SOURCE: mysa_product_strategy.md, Part 3c — country-level data; Part 9a — convention details and regulatory sources]

> [WEB SOURCE: Portugal — ECO/ASF rankings, top 10 = 92% of market. Spain — DGSFP sector report, 176 operating entities. France — ACPR data, 660 organizations. ACPR 1st quartile cutoff = €82M. Italy — IVASS, only 38 companies write RC Auto. EIOPA — ~300 of ~2,300 Solvency II entities qualify as SNCU (<€100M GWP, ~13%)]
> [SOURCE: mysa_product_strategy.md, Part 3c]

**Key observations:**

- **France is the largest motor market in the EU** at €28.1B, and has the most mid-market targets (30-60 Caravela-tier carriers, 100+ small carriers). The French mutuelle system creates a deeply fragmented market with hundreds of autonomous, multi-line carriers — many with motor books in the €82-200M range. [SOURCE: mysa_product_strategy.md, Part 3c]
- **Spain is the fastest-growing motor market** at +8.9% YoY. Its convention system (CIDE) processes 2.5M claims per year. [SOURCE: mysa_product_strategy.md, Part 9a]
- **Portugal is the smallest market but the best proving ground** — tightest feedback loop, highest convention agreement rate (91%), and Caravela as design partner. [SOURCE: mysa_product_strategy.md, Part 3c]
- **Italy has the fewest motor writers** (only 38 write RC Auto per IVASS) but mandatory CARD convention for two-vehicle collisions. Italy's pending mandatory nat cat insurance for businesses (effective October 2025) will drive massive property claims growth. [SOURCE: mysa_product_strategy.md, Part 3c; Part 3f]

#### Property Insurance

| Country | Property GWP | Claims/Year | Penetration | Dominant Peril | Catastrophe Scheme |
|---------|-------------|------------|-------------|---------------|-------------------|
| **Portugal** | ~€0.44B (Multirriscos) | ~200-300K est. | ~55% | Wildfires, storms | None |
| **Spain** | **€6.1B** (Hogar, 61.4% of €9.99B multirriesgos) | **~4M+** (UNESPA) | ~74% | **Water damage (38.2%)** | **CCS** (state reinsurer; DANA 2024 = €3.5B) |
| **France** | **€13.8B** (MRH, 2024, +7.5%) | **4.6M** (France Assureurs) | **~96%** (mandatory for tenants) | **Water damage (44%)** | **CCR/Cat-Nat** (surcharge increasing 12% to 20%) |
| **Italy** | ~€3.5-4.0B (Fire + Property) | ~1-2M | ~50% (lowest in Southern EU) | Earthquakes, floods | **Mandatory nat cat for businesses from Oct 2025** |
| **Southern EU Total** | **~€24-28B** | **~10-12M** | | | |

[SOURCE: mysa_product_strategy.md, Part 3f — Southern EU Home/Property Market; market_landscape_overview.md, Section 5]

> [WEB SOURCE: France Assureurs 2024, ICEA 2024, UNESPA, ASF, ANIA/IVASS, DLA Piper Italy nat cat law]
> [SOURCE: mysa_product_strategy.md, Part 3f]

**Key observations:**

- **Water damage is the "fender bender" of property claims** — 38-44% of all home claims in Spain and France. Highly repetitive, highly standardizable, and perfect for AI-assisted decision-making. [SOURCE: mysa_product_strategy.md, Part 3f]
- **Italy is a massive growth story**: mandatory nat cat insurance for all businesses (effective October 2025) will add an estimated €2-3B in new premiums. Residential mandatory coverage is under discussion. 2023 was a record cat year (€6B insured losses). Claims volumes will surge, and carriers will need tech to handle it. [SOURCE: mysa_product_strategy.md, Part 3f]
- **France has near-universal penetration** (~96%) because tenants insurance is mandatory, making it the largest EU property claims market by volume (4.6M claims/year). [SOURCE: mysa_product_strategy.md, Part 3f]

---

### 4.2.2 Northern/Central EU (Mixed Convention Systems — Expansion Markets)

These 12 countries represent a larger premium pool than Southern EU (€70-78B motor vs €57.9B) but with fewer mid-market carriers in the Caravela tier. Convention systems are mixed — some countries have partial or emerging convention-like systems, others have none. The wedge is weaker here, but the market size justifies expansion once Southern EU is proven.

#### Motor Insurance

| Country | Motor GWP | Convention-Like System? | Total Insurers | Caravela-Tier (€100-200M) | Small (€50-100M) |
|---------|----------|------------------------|----------------|--------------------------|-------------------|
| **Germany** | **~€30B** | Teilungsabkommen (bilateral only, not universal) | ~522 BaFin + 534 state-supervised | **15-25** | 20-35 |
| **Netherlands** | **~€5.9-6.2B** | DSA (new, launched 2024) | ~60-70 | **3-5** | 5-8 |
| **Belgium** | **~€4.3-4.5B** | RDR (Convention Reglement Direct) | ~82-90 | **5-8** | 8-12 |
| **Austria** | **~€4.3B** | None formal | ~30-35 | **2-4** | 3-5 |
| **Switzerland** | **~€7.2-8.2B** | None formal | ~117 | **3-5** | 5-8 |
| **Ireland** | **~€1.3B** | None | ~40-50 | **2-4** | 3-5 |
| **Sweden** | **~€2.6-2.9B** | Trafikskadenamden (injury board) | ~50-60 | **3-4** | 4-6 |
| **Denmark** | **~€2.0-2.4B** | None formal | ~40-50 | **2-3** | 3-5 |
| **Finland** | **~€1.2-1.4B** | Traffic Insurance Centre | ~40-49 | **2-3** | 2-3 |
| **Norway** | **~€2.7-2.8B** | None formal | ~30-40 | **2-3** | 3-4 |
| **Poland** | **~€6.5B** | UFG coordination | ~29 | **3-5** | 4-6 |
| **Czech Republic** | **~€2.1-2.3B** | None formal | ~24-30 | **2-3** | 3-4 |
| **Northern/Central EU Total** | **~€70-78B** | **Mixed** | | **~42-72** | **~63-101** |

[SOURCE: mysa_product_strategy.md, Part 9a — Northern/Central EU table; validated via BaFin, DNB, FSMA, FMA, FINMA, FI Sweden, FSA Denmark, FIN-FSA, Finanstilsynet Norway, KNF Poland, CNB Czech Republic]

**Key observations:**

- **Germany (~€30B) is the single largest EU motor market** but more concentrated than Southern EU — fewer mid-market targets proportionally. Still, 15-25 Caravela-tier carriers is the largest Northern segment. [SOURCE: mysa_product_strategy.md, Part 9a]
- **Belgium (RDR convention), Netherlands (DSA — new 2024), and Sweden (Trafikskadenamden)** have convention-like systems, providing a partial wedge opportunity. [SOURCE: mysa_product_strategy.md, Part 3d]
- **Poland (€6.5B)** is a significant market with only ~29 insurers — more concentrated but growing. [SOURCE: mysa_product_strategy.md, Part 9a]
- **Austria, Switzerland, Ireland, Denmark, Norway, Finland, Czech Republic** have no formal convention systems — the sell here is the general decision engine capability, not convention expertise. [SOURCE: mysa_product_strategy.md, Part 3d]

#### Property Insurance

| Country | Property GWP | Penetration | Key Dynamic | Motor/Property Carrier Overlap |
|---------|-------------|-------------|------------|-------------------------------|
| **Germany** | **~€15.5-17B** | ~94% building insurance | Profitable only 4x since 2002. Water damage >€4.5B/yr. €8.2B 2021 floods. | Very high (except HUK-Coburg motor-only) |
| **Netherlands** | ~€4.5-5.5B | ~90%+ | Property is LARGEST non-life line. Flood risk rising; EIOPA new 0.17% flood factor. | Very high |
| **Belgium** | ~€2.4-2.5B | ~95% | Nat cat mandatory in fire policies. 2021 Wallonia floods. | Very high |
| **Austria** | ~€2.0-2.5B | ~80-85% | >€1B weather damages 2023 | Very high |
| **Switzerland** | ~€2.5-3.5B | ~95-100% | **KGV monopoly in 19 cantons limits private market to ~80% of country** | High (limited by KGV) |
| **Ireland** | ~€1.8-2.0B | ~85-90% | Windstorm + flood exposure | Very high |
| **Sweden** | ~€3.5-4.0B | ~95% | Near-universal coverage. Forest fires increasing. | Very high |
| **Denmark** | ~€3.0-3.5B | ~90%+ | Stormradet mandatory storm scheme | Very high |
| **Finland** | ~€1.5-2.0B | ~80-85% | Flood gap >90% (worst Nordic coverage gap) | Very high |
| **Norway** | ~€2.5-3.0B | ~90%+ | **Naturskadepool mandatory; $218M deficit 2023** | Very high |
| **Poland** | ~€1.5-2.0B | **~49%** | **Major growth market — lowest penetration in EU-16** | Very high |
| **Czech Republic** | ~€1.3-1.5B | ~60-70% | Below Western EU average penetration | Very high |
| **Northern/Central EU Total** | **~€30-33B** | | | |

[SOURCE: mysa_product_strategy.md, Part 3f — Northern/Central EU table; market_landscape_overview.md, Section 5]

> [WEB SOURCE: GDV, Verbond van Verzekeraars, FSMA/Assuralia, VVO, VKG/SVV, Central Bank of Ireland, Svensk Forsakring, Finanstilsynet, Finanssiala, Naturskade.no, PIU, XPRIMM/CNB]
> [SOURCE: mysa_product_strategy.md, Part 3f]

**Key observations:**

- **Germany is the EU's largest property market** (~€15.5-17B) but is structurally unprofitable — only profitable 4 times since 2002. Water damage alone costs >€4.5B/year. Carriers here need decision efficiency the most. [SOURCE: mysa_product_strategy.md, Part 3f]
- **Poland (~49% penetration) is the EU's biggest growth market for property** — as penetration catches up to Western EU norms, claims volumes will multiply. [SOURCE: market_landscape_overview.md, Section 5]
- **Motor/property carrier overlap is "very high" in every Northern/Central EU country** — confirming the upsell thesis. [SOURCE: mysa_product_strategy.md, Part 3f]

---

### 4.2.3 EU Grand Totals

| Metric | Southern EU (4 countries) | Northern/Central EU (12 countries) | **All 16 EU Countries** |
|--------|--------------------------|-----------------------------------|------------------------|
| **Motor GWP** | €57.9B | ~€70-78B | **~€128-136B** |
| **Property GWP** | ~€24-28B | ~€30-33B | **~€54-61B** |
| **Combined GWP** | ~€82-86B | ~€100-111B | **~€182-197B** |
| **Caravela-tier carriers (€100-200M)** | 54-93 | 42-72 | **~96-165** |
| **Small carriers (€50-100M)** | 141-159+ | 63-101 | **~204-260+** |
| **Enterprise (>€1B — builds in-house)** | 16-19 | ~20-30 | **~36-49** |
| **Large (€200M-€1B)** | 30-47 | ~30-50 | **~60-97** |
| **Micro (<€50M)** | 243-372+ | 200-400+ | **~443-772+** |
| **Motor claims/year** | — | — | **~25-35M** |
| **Property claims/year** | — | — | **~16-20M** |

[SOURCE: mysa_product_strategy.md, Part 9a — "Full EU Totals" table; market_landscape_overview.md, Sections 4-5]

> The Northern EU market is LARGER in premium terms than Southern EU (€70-78B vs €57.9B) but has FEWER mid-market carriers in the Caravela tier. Germany alone is €30B but concentrated in large players. Southern EU has more fragmented markets = more mid-market targets. Convention systems in Southern EU provide the wedge, but Germany/Benelux/Nordics are the expansion that makes this a real company.
> [SOURCE: mysa_product_strategy.md, Part 9a — CLAUDE ANALYSIS]

---

## 4.3 US Market

The US is the largest single insurance market globally. Its structure differs fundamentally from the EU: no convention systems, a large TPA/MGA ecosystem, and much higher concentration in auto (but less in property). This section maps the US opportunity as an expansion market.

### US Market Structure

| Segment | Count | Premium/Revenue | Concentration |
|---------|-------|----------------|--------------|
| **Total P&C carriers** | ~4,116 entities | $1.06T DWP | Top 10 = 51.4%, Top 100 = ~90% |
| **Auto insurance** | — | **$359B** | **Top 5 = 63.6%** (extremely concentrated) |
| **Homeowners** | — | **$172.7B** (+13.7% YoY, 2024) | Top 25 = 78% (less concentrated) |
| **Commercial multi-peril** | — | $87B | More fragmented |
| **Workers' comp** | — | $65B | Fragmented |

[SOURCE: mysa_product_strategy.md, Part 9a — US Market comparison; validated via NAIC 2024 Market Share, AM Best, Conning, IBIS World]

### US Carrier Distribution by Size

| Tier (DWP) | Carrier Count | Profile | Mysa Fit |
|-----------|--------------|---------|---------|
| **>$5B** (top 25-30 groups) | ~25-30 | Build in-house — State Farm, GEICO, Progressive, Allstate, Liberty Mutual | **NO** |
| **$1B-$5B** | ~50-80 | Mix of build/buy — Cincinnati Financial, Hanover, Erie | Possible — longer cycles |
| **$100M-$500M** (Caravela-comparable) | **~200-350** | **Buy-not-build — can't afford data science teams** | **YES — primary** |
| **$50M-$100M** | ~150-250 | Lean operations, budget-conscious | YES — entry-level |
| **<$50M** | ~3,000+ | Micro carriers, regional, many inactive/run-off | Long-tail only |

[SOURCE: mysa_product_strategy.md, Part 9a — US Carrier Distribution table]

### US Non-Carrier Buyers (Unique to US)

The US has a large ecosystem of non-carrier buyers that does not exist at comparable scale in the EU. These entities process claims on behalf of carriers and represent a significant additional buyer pool.

| Buyer Type | Count (Material Size) | Why They Buy | Market Size |
|-----------|----------------------|-------------|------------|
| **TPAs** (P&C-focused) | ~500-800 | Process claims for carriers. Adjuster shortage + leakage pressure. Need efficiency tools. | ~$115B managed |
| **MGAs with claims authority** | ~330-550 | Fastest-growing segment (16% CAGR). Increasingly handle claims in addition to underwriting. | ~$114B managed premium |
| **Independent adjusting firms** | ~53,000 businesses | Workforce IS their product. Augmentation = survival. | $11.7B market |

[SOURCE: market_landscape_overview.md, Section 2 — US Non-Carrier Buyers; mysa_product_strategy.md, Part 9a]

> "Mid-tier TPAs buy rather than build. They have budget pressure (adjuster shortage, leakage, turnover)."
> [SOURCE: mysa_product_strategy.md, Part 3d — referencing RESEARCH Section 6]

### Total US Addressable Buyers

**~1,030-1,700** entities (carriers in $100M-$500M tier + material-size TPAs + MGAs with claims authority). [SOURCE: mysa_product_strategy.md, Part 9a]

### US Homeowners — Key Metrics

| Metric | Value | Source |
|--------|-------|--------|
| Total DWP | **$172.7B** (2024, +13.7% YoY) | NAIC |
| Claims/year | **~4.4-4.5M** (5.3% frequency on ~84M insured homes) | III/ISO |
| Total carriers writing homeowners | **~496** | IBISWorld |
| $100-500M tier (Caravela-comparable) | **~60-80 carriers** | NAIC/AM Best |
| Top 5 market share | **45.7%** (LESS concentrated than auto = 63.6%) | NAIC |
| Average claim size | **$17,059** (3.4x larger than auto's ~$5,000) | III |
| Xactimate usage | **~80% of property claims** | Verisk |

[SOURCE: mysa_product_strategy.md, Part 3f — US Homeowners Market table; market_landscape_overview.md, Section 5]

### Why Property, Not Auto, in the US

US auto is dangerously concentrated — the top 5 carriers (State Farm, GEICO, Progressive, Allstate, USAA) control 63.6% of the market. Mid-market carriers in auto are being squeezed. US homeowners, by contrast, is less concentrated (top 5 = 45.7%), with more of the market sitting in mid-market and regional carriers. **For Mysa, US entry should target homeowners/property mid-market carriers + TPAs, not US auto.** [SOURCE: mysa_product_strategy.md, Part 9a — CLAUDE ANALYSIS; Part 3d]

### Named US Mid-Market Carriers (Property-Strong)

Erie ($3.3B, tech-forward — invested in AI startups), Cincinnati Financial ($1.6B), Amica ($1.2B, "AI Trailblazer" — partnered with ZestyAI), NJM Insurance, Donegal Insurance Group, Secura, Shelter Insurance, Westfield Insurance, state farm bureaus (KY, NC, TX). Plus insurtechs: Hippo, Kin, SageSure. [SOURCE: mysa_product_strategy.md, Part 3f]

---

## 4.4 Why Bottom-Up: Mid/Small First, Not Enterprise

### The Enterprise Trap

> "For big carriers, it will be 'don't touch this. It's my turf. It's my logic. Build our own.'"
> — Jeremy Blehaut [TRANSCRIPT: Feb 7, 2026]

> "I always think about insurance companies as companies that have a data science team. But I think you are right." — Co-founder, after realizing mid-market carriers don't have dev teams [TRANSCRIPT: Feb 7, 2026]

Enterprise carriers (>€1B GWP / >$5B DWP) — Allianz, AXA, Generali, UnipolSai, Covea, State Farm, GEICO, Progressive — exhibit a consistent pattern:

**They build in-house. Badly.**

- Allianz launched "Insurance Copilot" in Austria in 2024. Key insight: they built it in-house for themselves, not as a product for other insurers. [SOURCE: mysa_product_strategy.md, Part 3a — referencing competitive_landscape_reality_check.md]
- BCP (Portugal's largest bank) has an in-house Copilot. Direct observation from co-founder's girlfriend who works there: "It's very bad." [TRANSCRIPT: Feb 7, 2026]

Even when enterprise builds are bad, the institutional bias is still "my turf, my logic." Selling to enterprise means:

| Enterprise Characteristic | Impact on Mysa |
|--------------------------|---------------|
| 12-month procurement cycles | Burns cash with no revenue during sales cycle |
| Enterprise procurement committees | 8-15 stakeholders instead of 1-2 decision-makers |
| RFP processes | Commoditizes Mysa's unique value into a feature checklist |
| Internal build bias | Carrier believes they can do it themselves (even when they can't) |
| Existing vendor lock-in | Guidewire, Duck Creek, CCC already entrenched — adding another vendor feels risky |
| Customization demands | "We're different" — enterprise expects bespoke, not product |

[SOURCE: mysa_product_strategy.md, Part 3a — enterprise vs mid-market analysis; CLAUDE ANALYSIS]

### Why Mid/Small Works

> "For the mid-market ones like Caravela, they want us."
> — Jeremy Blehaut [TRANSCRIPT: Feb 7, 2026]

Mid-market carriers (€100-200M GWP, ~100-200 employees) are the opposite of enterprise on every dimension that matters for an early-stage company:

| Mid-Market Characteristic | Why It Matters |
|--------------------------|---------------|
| **Can't build it** | No data science team. No AI/ML engineers. 100-200 total employees — they don't have the talent to build claims AI. |
| **Want to buy it** | Growing fast (Caravela grew 10x in 10 years). Need tools to scale without proportional headcount growth. |
| **Fast decisions** | 1-2 decision-makers (VP Claims + CEO/COO). No procurement committee. No 12-month RFP process. |
| **No procurement bureaucracy** | Call, demo, pilot, contract. 3-6 month sales cycle vs 12-18 months for enterprise. |
| **Budget exists** | €50K-200K/year is 0.03-0.2% of GWP — trivial if it improves STP or reserve accuracy. |
| **Pain is acute** | Growing claims volume with flat headcount. Adjusters drowning. Institutional knowledge walking out the door. |
| **Reference customers** | Happy mid-market customers create peer pressure in tight insurance communities. Word of mouth in a market of 300-500 carriers. |

[SOURCE: mysa_product_strategy.md, Part 3a — "Why Caravela tier is the sweet spot"; market_landscape_overview.md, Section 2]

### Bottom-Up Expansion Path

The strategy is not "stay mid-market forever." It is:

1. **Win mid-market** (€100-200M, Caravela tier) — prove product-market fit, build data moat
2. **Expand to small** (€50-100M) — entry-level pricing, same product
3. **Move up to large** (€200M-€1B) — with customer proof points and data, large carriers become "better than what you built internally"
4. **Eventually serve enterprise** — but only from a position of strength, with a proven product and hundreds of mid-market deployments

> Even the large carriers that build in-house are building BAD copilots. The co-founder's direct observation: internal tools are document retrieval, not decision support. Mysa could eventually sell to large carriers as "better than what you built internally" — but that's Phase 3, not Phase 1.
> [SOURCE: mysa_product_strategy.md, Part 3a — CLAUDE ANALYSIS]

---

## 4.5 Caravela Tier Sweet Spot

### The Anchor: Caravela Seguros

| Metric | Value |
|--------|-------|
| GWP (2024) | €188M |
| Employees | 149 |
| Total claims/year | ~57K (42K motor + ~15K property) |
| Ranking | 7th in Portuguese non-life |
| Growth | 10x in 10 years |
| Property growth | +31% (fastest-growing line) |
| Data science team | **None** |

[SOURCE: market_landscape_overview.md, Section 6 — Anchor: Caravela Seguros; WEB: Caravela 2024 Annual Report, ECO rankings, ASF data]

Caravela is the archetype of the target customer: a mid-market carrier with real claims volume (57K/year), rapid growth (10x in a decade), zero in-house AI capability (149 employees, no data science team), and acute operational pressure (growing claims with flat headcount). It is also Mysa's design partner.

### Why €100-200M GWP Is Optimal

1. **Real claims volume** (~30K-60K claims/year) justifies the technology investment. A carrier processing 5K claims/year doesn't need a decision engine. One processing 40K does. [SOURCE: mysa_product_strategy.md, Part 3a]

2. **No data science team** — at 100-200 employees, there is no room for ML engineers, data scientists, or AI specialists. They must buy, not build. [SOURCE: mysa_product_strategy.md, Part 3a]

3. **Growth pressure** — many Caravela-tier carriers are growing fast (Caravela: 10x in 10 years, UNA motor +26%). They need tools to scale without hiring proportionally. [SOURCE: market_landscape_overview.md, Section 6]

4. **Budget exists** — €50K-200K/year is 0.03-0.2% of GWP. Trivial if it improves STP rates or reserve accuracy. Compare to a single adjuster's fully loaded cost (~$110K/year). [SOURCE: mysa_product_strategy.md, Part 3a]

5. **Fast decision-making** — 1-2 decision-makers (not a procurement committee). 3-6 month sales cycle. [SOURCE: mysa_product_strategy.md, Part 3a]

### Named Caravela-Tier Carriers by Market

| Country | Carrier | Estimated GWP | Notes |
|---------|---------|---------------|-------|
| **Portugal** | **Caravela** | €188M (2024) | Design partner. 7th non-life. 42K motor claims. |
| Portugal | CA Seguros | ~€200-210M | 8th, displaced by Caravela |
| Portugal | Mapfre PT | ~€190-210M | 9th, surge with Bankinter partnership |
| Portugal | Aegon Santander | ~€170-190M | 10th, health +37.5% |
| Portugal | Victoria | ~€130-150M | 11th, strong in health |
| Portugal | UNA | ~€120-140M | 12th, health +53%, motor +26% |
| **Spain** | Pelayo | ~€375M (mutua) | 844K auto policies, 2.42% motor share |
| Spain | Admiral/Balumba | ~€100-150M motor | UK-owned direct writer, +13.4% |
| Spain | Patria Hispana | ~€100-130M | Centennial company, +12.9% |
| Spain | Mutua Tinerfena | ~€80-120M | Regional Canary Islands mutual |
| **France** | Thelem Assurances | €453M total (~€150-200M motor) | 1.15M contracts. **Closest French analog to Caravela.** |
| France | L'Olivier Assurance | ~€220-260M | Online auto pure-play. Similar growth profile to Caravela. |
| France | Direct Assurance (AXA sub) | ~€300-400M | Slightly larger than Caravela tier |
| France | ~30-60 small mutuelles | €82-200M each | ACPR 2nd quartile. Many are autonomous, multi-line with motor books. |
| **Italy** | HDI Assicurazioni | €716M non-life, ~€160-200M motor | R.C. Auto = 22.8% of non-life. **Closest Italian analog to Caravela.** |
| Italy | ~10-12 smaller carriers | €50-200M motor | Regional companies, online insurers (Prima, Quixa, Verti, Linear) |

[SOURCE: mysa_product_strategy.md, Part 3c — Caravela-Tier Deep Dive; market_landscape_overview.md, Section 6]

> [WEB SOURCE: Caravela 2024 Annual Report; ASF; ECO Sapo rankings; MAPFRE Economics; France Assureurs; IVASS/ANIA]
> [SOURCE: mysa_product_strategy.md, Part 3c]

---

## 4.6 Mid-Market vs Small: Different Needs

Carriers in the €100-200M range (Caravela tier) and carriers in the €50-100M range (small tier) share the core problem — they can't build AI in-house — but their buying behavior, data maturity, and budget constraints differ meaningfully.

### By Carrier Size

| Dimension | Caravela Tier (€100-200M) | Small Tier (€50-100M) |
|-----------|--------------------------|----------------------|
| **Employees** | ~100-200 | <100 |
| **Claims/year** | ~30K-60K | ~15K-30K |
| **Data infrastructure** | Basic CMS (often legacy or homegrown). Some have Guidewire/Duck Creek. Digital records exist but may be inconsistent. | Minimal. May still use paper-heavy processes. Some have no CMS at all — spreadsheets and email. |
| **Decision-maker** | VP Claims or CCO (dedicated role) | CEO or COO wearing multiple hats. Claims may report to a general operations head. |
| **Budget for claims tech** | €50K-200K/year | €10K-100K/year |
| **Pricing sensitivity** | Moderate — ROI-driven. Will pay if value is demonstrated. | High — tight budgets, every euro scrutinized. Per-claim pricing preferred over platform fees. |
| **Sales cycle** | 3-6 months | 1-3 months (simpler decision, lower stakes) |
| **Onboarding complexity** | Medium — need to ingest SOPs, connect to existing CMS, configure workflows. Historical data may be available. | Low — simpler SOPs (or no formal SOPs), fewer integrations, less historical data. |
| **Strategic value to Mysa** | High — reference customers, meaningful data volume, case studies | Moderate — volume play, proves broad applicability, lower ACV |

[SOURCE: mysa_product_strategy.md, Part 3a — carrier segmentation; Part 3e — pricing model; market_landscape_overview.md, Section 2]

### By Line of Business

| Dimension | Motor | Property |
|-----------|-------|----------|
| **EU mid-market data maturity** | Higher — convention systems create structured data standards (EAS forms, convention codes). Carriers have been digitizing motor for years. | Lower — no convention systems, less standardized data. Property claims often documented in free-text reports, photos, and vendor estimates. |
| **US mid-market data maturity** | Higher — CCC/Mitchell integration widespread. Structured auto claims data. | Mixed — Xactimate used by ~80% for estimation, but coverage determination and causation remain largely unstructured. |
| **Pricing sensitivity (EU)** | Lower — motor is the bread-and-butter line. Carriers understand the ROI of motor claims efficiency. | Higher — property is often a secondary line for motor-primary carriers. Budget may be tighter for property-specific tools. |
| **Pricing sensitivity (US)** | Higher — auto mid-market is being squeezed by top 5 carriers. Less room for new tools. | Lower — property is growing rapidly (+13.7% YoY). Carriers have acute pressure from cat losses and need tech solutions. |

[SOURCE: mysa_product_strategy.md, Part 3f — motor vs property comparison; market_landscape_overview.md, Section 3]

### By Region

| Dimension | EU Mid-Market | US Mid-Market |
|-----------|--------------|--------------|
| **Primary buyer type** | Carriers (direct) | Carriers + TPAs + MGAs (three buyer types) |
| **TPA ecosystem** | Small — most carriers handle claims in-house | Large — ~500-800 material TPAs, many handling claims for multiple carriers |
| **Convention system value** | High — differentiator in Southern EU, partial in Northern EU | None — no convention systems in the US |
| **Regulatory complexity** | Per-country regulation (16 different frameworks), GDPR, EU AI Act | Per-state regulation (50 states + DC), more litigious environment |
| **Sales motion** | Relationship-driven, conference-based, language/cultural barriers per market | More standardized, English-only, larger conference ecosystem (ITC, RIMS) |
| **Competitive density** | Low (90-95% of mid-market has no claims AI) | Moderate (75-85% open, but more competitors active — Five Sigma, Hi Marley) |

[SOURCE: mysa_product_strategy.md, Parts 3a, 3d, 9a — market openness by segment]

---

## 4.7 Motor + Property Overlap

### The Same Buyers

**80-95% of carriers that write motor also write property.** This is validated across all 16 EU countries and the US. [SOURCE: market_landscape_overview.md, Section 3; mysa_product_strategy.md, Part 3f]

Caravela itself illustrates the overlap: €188M total GWP, of which motor is the primary line (42K motor claims) but property is the fastest-growing (+31%), with approximately 15K property claims per year. The same VP Claims manages both lines. The same adjusters often handle both (though specialization increases with carrier size). [SOURCE: market_landscape_overview.md, Section 6]

The Northern/Central EU data confirms this universally:

| Country | Motor/Property Carrier Overlap |
|---------|-------------------------------|
| Germany | Very high (except HUK-Coburg motor-only) |
| Netherlands | Very high |
| Belgium | Very high |
| Austria | Very high |
| Switzerland | High (limited by KGV cantonal monopolies) |
| Ireland | Very high |
| Sweden | Very high |
| Denmark | Very high |
| Finland | Very high |
| Norway | Very high |
| Poland | Very high |
| Czech Republic | Very high |

[SOURCE: mysa_product_strategy.md, Part 3f — Northern/Central EU property table, carrier overlap column]

### The Same Workflow (~80% Identical)

The adjusting process for property is nearly identical to motor — the same 6 decision sub-steps apply:

| Decision Sub-Step | Motor | Property | Overlap |
|-------------------|-------|----------|---------|
| **Coverage verification** | "Is this accident covered under the policy?" | "Is this water damage / fire / storm covered under the policy?" | ~90% identical |
| **Policy check** | Check policy terms, exclusions, deductibles | Check policy terms, exclusions, deductibles, named vs open perils | ~80% identical (property adds causation) |
| **Repair assessment** | Damage assessment via photos, inspection | Damage assessment via photos, inspection, contractor scopes | ~85% identical |
| **Cost analysis** | Audatex/CCC estimates, parts pricing | Xactimate estimates, material pricing, contractor bids | ~70% identical (different estimation tools) |
| **Reserve calculation** | Historical comparison, severity bands | Historical comparison, severity bands, cat exposure | ~85% identical |
| **Fraud detection** | Pattern matching, staged accident indicators | Pattern matching, inflated claims indicators, pre-existing damage | ~80% identical |

[SOURCE: mysa_product_strategy.md, Part 3f — "the adjusting process for property is nearly identical to motor — the same 6 decision sub-steps"]

The key difference is in the **decision itself**: motor asks "WHO caused it?" (fault allocation, often determined by convention systems). Property asks "WAS it covered?" (policy interpretation, causation analysis — sudden vs gradual for water damage, named peril vs open peril). This means the AI modules are different, but the workflow architecture, data model, and user experience are ~80% shared. [SOURCE: market_landscape_overview.md, Section 3]

### Revenue Uplift: +60-70% Per Carrier, Zero New Acquisition

| Scenario | Motor-Only TAM | Motor + Property TAM | Uplift |
|----------|---------------|---------------------|--------|
| EU mid-market only | €50-100M | **€80-170M** | **+60-70%** |
| EU + US mid-market | €100-250M | **€160-425M** | **+60-70%** |
| Full addressable | €200-650M | **€320M-1.1B** | **+60-70%** |

[SOURCE: mysa_product_strategy.md, Part 3f — "Revenue impact of adding property to motor"]

> Adding property doesn't require new buyers — it requires new AI modules (coverage determination, causation analysis) applied to the **same carrier relationships**. The carrier overlap is 80-95% across all 16 EU countries and the US.
> [SOURCE: mysa_product_strategy.md, Part 3f]

Caravela reference: at €188M GWP, 57K total claims/year = 42K motor (74%) + ~15K property (26%). French carriers are closer to 50/50 motor/property. Average across the EU: property claims = ~30-50% of motor per multi-line carrier. [SOURCE: mysa_product_strategy.md, Part 3f]

---

## 4.8 TAM Calculations

All TAM calculations are built bottom-up from validated carrier counts, anchored to Caravela's actual economics (€188M GWP, 57K claims/year, 149 employees). No top-down percentages of "total insurance market." Every number maps to a countable set of carriers.

### EU Carrier Size Distribution (Full Segmentation)

| Size Tier | GWP Range | EU Count (16 countries) | Tech Approach | Mysa Addressable? |
|-----------|----------|------------------------|---------------|-------------------|
| **Enterprise** | >€1B | ~36-49 groups | Build in-house (Allianz, AXA, Generali, UnipolSai, Covea all building own) | NO — Phase 3+ |
| **Large** | €200M-€1B | ~60-97 | Buy best-of-breed or outsource to TPA | YES — longer cycles |
| **Caravela tier** | €100-200M | **~96-165** | **Need it, can't build it. ~100-200 employees.** | **PRIMARY TARGET** |
| **Small** | €50-100M | **~204-260+** | Want tech, tight budget, <100 employees | YES — entry pricing |
| **Micro** | <€50M | ~443-772+ | Manual processes, minimal tech, <50 staff | LONG-TAIL only |

[SOURCE: mysa_product_strategy.md, Part 9a — Full EU Totals; market_landscape_overview.md, Section 2]

### US Carrier Distribution (For Comparison)

| Size Tier | DWP Range | US Count | Mysa Fit |
|-----------|----------|---------|---------|
| **Top 25-30** | >$5B | ~25-30 | NO — build in-house |
| **Large** | $1B-$5B | ~50-80 | Possible — longer cycles |
| **Caravela-comparable** | $100-$500M | **~200-350** | **YES — buy-not-build** |
| **Small** | $50-$100M | ~150-250 | YES — budget-conscious |
| **Micro** | <$50M | ~3,000+ | Mixed — many mono-line or inactive |

[SOURCE: mysa_product_strategy.md, Part 9a — US Carrier Distribution]

### Target Segment Claims Volume

| Segment | Carriers | Motor Claims | Property Claims | **Combined Claims** |
|---------|---------|-------------|----------------|-------------------|
| **Caravela tier (€100-200M) — EU** | 96-165 | 2.9-7.4M | 1.2-4.1M | **4.1-11.5M** |
| **Small tier (€50-100M) — EU** | 204-260 | 2.4-6.5M | 1.0-3.1M | **3.4-9.6M** |
| **US mid-market ($100-500M) + TPAs** | 60-80 carriers + 500-800 TPAs | ~3-5M | ~1-2M | **~4-7M** |
| **TOTAL TARGET** | **360-505 carriers + TPAs** | **~8-19M** | **~3-9M** | **~11-28M claims/year** |

[SOURCE: market_landscape_overview.md, Section 6 — Target Segment Claims Volume; mysa_product_strategy.md, Part 3f]

### Target as Percentage of Total Market

| | Motor | Property | Combined |
|--|-------|----------|---------|
| **Target segment** | ~8-19M | ~3-9M | **~11-28M** |
| **Total market** | ~60-70M | ~20-25M | ~80-95M |
| **Target as %** | ~15-27% | ~15-36% | **~14-29%** |

[SOURCE: market_landscape_overview.md, Section 6 — "Target as % of Total Market"]

This is the right size for a focused startup: **large enough to build a $100M+ ARR business, small enough that enterprise competitors (Shift, CCC, Guidewire) aren't competing for the same buyers.** [SOURCE: mysa_product_strategy.md, Part 3f — CLAUDE ANALYSIS]

### TAM Scenarios — Motor Only (Bottom-Up from Validated Carrier Counts)

| Scenario | EU Carriers | US Buyers | Total Buyers | ACV Range | **Revenue Range** |
|----------|------------|-----------|-------------|-----------|-------------------|
| **Conservative** — Southern EU Caravela tier only | 54-93 | — | 54-93 | €50-200K | **€2.7-€18.6M** |
| **Base** — All EU €50-200M carriers | 300-425 | — | 300-425 | €30-200K | **€25-55M** |
| **EU + large tier** — Add €200M-1B | 360-520 | — | 360-520 | €30-500K | **€50-100M** |
| **EU + US mid-market** — Add US $100-500M carriers + TPAs + MGAs | 360-520 | 1,030-1,700 | 1,530-2,400 | €10K-2M | **€200-650M** |

[SOURCE: mysa_product_strategy.md, Part 9b — Motor TAM table]

### TAM Scenarios — Motor + Property Combined (Same Buyers, +60-70% Revenue)

| Scenario | Motor TAM | + Property TAM | **Combined TAM** |
|----------|----------|---------------|-----------------|
| **Conservative** — Southern EU Caravela tier | €2.7-€18.6M | +€1.6-€13M | **€4.3-€31.6M** |
| **Base** — All EU €50-200M | €25-55M | +€15-38M | **€40-93M** |
| **EU + large** | €50-100M | +€30-70M | **€80-170M** |
| **EU + US mid-market** | €100-250M | +€60-175M | **€160-425M** |
| **Full addressable** | €200-650M | +€120-455M | **€320M-1.1B** |

[SOURCE: mysa_product_strategy.md, Part 9b — Motor + Property TAM table]

### The Honest TAM Narrative

> [TRANSCRIPT — Jeremy]: "It's like 700 mid-market players in Europe. That makes less than 500 million of... insurance, like Caravela style."
> [SOURCE: mysa_product_strategy.md, Part 3c]

The Southern EU motor market alone is **NOT a venture-scale TAM**. At base case (~€15-25M), it is a healthy SaaS business but not a $1B+ outcome. The venture story requires:

1. Expanding to all of EU including Northern markets
2. Expanding to the US
3. Expanding from motor to property
4. Moving up-market over time

EU motor is the **wedge**, not the company. [SOURCE: mysa_product_strategy.md, Part 3c — CLAUDE ANALYSIS]

**But as a wedge, it is perfect:**
- 54-93 carriers in the primary tier = reachable with 2-3 sales reps
- Caravela as design partner proves the product in a live environment
- Convention system expertise creates a defensible moat
- Every carrier added builds the historical data flywheel
- Technology transfers directly to property and US markets

[SOURCE: mysa_product_strategy.md, Part 3c]

### The Fundraising TAM Story

| Stage | TAM | What It Represents |
|-------|-----|-------------------|
| **Wedge TAM** (EU motor, Caravela tier) | €2.7-€18.6M | Proves the product works. Not venture-scale alone. |
| **Year 2-3 TAM** (all EU mid-market motor + property) | €80-170M | Real SaaS business. |
| **Year 3-5 TAM** (EU + US mid-market, both lines) | €160-425M | Venture-scale. |
| **Vision TAM** (full addressable + expansion) | €320M-1.1B | IPO-scale. |

[SOURCE: mysa_product_strategy.md, Part 9b — "The honest TAM story for fundraising"]

> "We start with EU motor — the convention system wedge that nobody else has. Within 6 months, the same carrier pays us for property too (same AI, bigger problem, same buyer). By year 3, we're in the US with the same product. The market is ~11-28M claims/year in our target segment alone, 80-95M globally. And 90%+ of mid-market carriers have ZERO AI claims tools today."
> [SOURCE: mysa_product_strategy.md, Part 9b]

### Market Openness — Why This TAM Is Actually Accessible

| Segment | Total Entities | Using Claims AI | % Open | Mysa Opportunity |
|---------|---------------|----------------|--------|-----------------|
| **All carriers globally (EU + US)** | ~6,300+ | ~400-600 (~7%) | **~93% open** | Massive whitespace |
| **EU mid-market (€50-200M)** | ~300-425 | <30 (Shift = large carriers, Bdeo = visual only) | **~90-95% open** | **Primary target — virtually untouched** |
| **US mid-market ($100-500M)** | ~200-350 | ~30-50 (Five Sigma + Hi Marley customers) | **~75-85% open** | Strong — but competitors more active |
| **TPAs globally** | ~500-800+ | ~50-80 (Shift, ClaimSorted) | **~85-90% open** | Good expansion target |
| **MGAs with claims authority** | ~330-550 | <20 | **~95% open** | Emerging segment, growing fast |

[SOURCE: mysa_product_strategy.md, Part 9a — "Competitor Adoption — How Open Is the Market?"]

> Only 4% of insurers have SCALED AI in claims. Most "adoption" is pilots, POCs, or single-feature tools (Bdeo = photos only, Hi Marley = texting only). Nobody has deployed an AI decision engine at scale. [WEB: McKinsey 2025 insurance survey]
> [SOURCE: mysa_product_strategy.md, Part 9a]

---

## Sources

| Source | Type | Sections Used |
|--------|------|--------------|
| `market_landscape_overview.md` | Primary — validated market data compilation | 4.1, 4.2, 4.3, 4.5, 4.7, 4.8 |
| `mysa_product_strategy.md` Part 3a | Primary — segmentation, enterprise vs mid-market | 4.4, 4.5, 4.6, 4.8 |
| `mysa_product_strategy.md` Part 3b-3c | Primary — total market sizing, country-level data | 4.2, 4.3, 4.8 |
| `mysa_product_strategy.md` Part 3d | Primary — expansion markets, US entry strategy | 4.2, 4.3, 4.6 |
| `mysa_product_strategy.md` Part 3e | Primary — pricing model | 4.6 |
| `mysa_product_strategy.md` Part 3f | Primary — property market, overlap analysis, revenue uplift | 4.2, 4.7, 4.8 |
| `mysa_product_strategy.md` Part 9a | Primary — fundraising narrative, full EU country-by-country, US comparison, market openness | 4.2, 4.3, 4.8 |
| `mysa_product_strategy.md` Part 9b | Primary — revised TAM calculations | 4.8 |
| Feb 7 Granola call — Mid-market strategy | Transcript | 4.4 (enterprise vs mid-market quotes) |
| MODULE_01_POSITIONING.md | Reference — ICP segmentation, carrier table | 4.4, 4.5 (cross-reference) |
| EIOPA, BaFin, ACPR, IVASS, ASF, DGSFP, DNB, FSMA, FMA, FINMA, Central Bank of Ireland, FI Sweden, FSA Denmark, FIN-FSA, Finanstilsynet, KNF, CNB | Regulatory sources (via agent research) | 4.2 |
| NAIC 2024 Market Share, AM Best, Conning, IBIS World | US market sources (via agent research) | 4.3, 4.8 |
| France Assureurs 2024, ICEA 2024, UNESPA, ANIA, GDV | Industry body sources (via agent research) | 4.2 |
| McKinsey 2025 insurance survey | Web source — AI adoption rate | 4.8 |
| Caravela 2024 Annual Report, ECO Sapo rankings | Web sources — anchor carrier data | 4.5 |
