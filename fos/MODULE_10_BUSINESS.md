# Module 10: Business Model & Unit Economics

**Status:** DRAFT v1.0
**Last updated:** February 9, 2026
**Feeds:** Pitch deck slides 10-12, financial model, investor data room, pricing page, sales proposals

---

## 10.1 Revenue Stream: Decision Engine (Primary)

This is the core product and the core revenue stream. The decision engine -- the 6 expert judgment steps that consume 60-70% of adjuster time -- is what nobody else has built and what carriers will pay the most for.

### Revenue Model: Dual Pricing

Carriers choose between per-claim pricing and platform licensing. Most start per-claim (low barrier, pay-as-you-go) and migrate to platform pricing as they scale.

> "100% we can get from the tiniest 50k a year for this. And for the biggest 1,000,000."
> -- Jeremy Blehaut [TRANSCRIPT: Feb 7, 2026]

[SOURCE: mysa_product_strategy.md, Part 3e -- pricing model; CLAUDE ANALYSIS on per-claim vs platform pricing]

**Per-Claim Pricing:**

| Tier | Per-Claim Price | Typical Annual Volume | Implied Revenue |
|------|----------------|----------------------|----------------|
| Micro (<EUR50M GWP) | EUR5-8/claim | ~5-15K claims/year | EUR25K-120K/year |
| Starter (EUR50-100M GWP) | EUR3-5/claim | ~15-30K claims/year | EUR45K-150K/year |
| Professional / Caravela tier (EUR100-200M GWP) | EUR2-4/claim | ~30-60K claims/year | EUR60K-240K/year |
| Growth (EUR200M-500M GWP) | EUR2-3/claim | ~60-150K claims/year | EUR120K-450K/year |
| Enterprise (EUR500M-1B GWP) | Custom | ~150K+ claims/year | Custom |

[SOURCE: mysa_product_strategy.md, Part 3e -- pricing tiers anchored to Caravela economics]

**Platform Licensing (Annual Contract):**

| Tier | Annual Contract Value | Target Carrier Size |
|------|----------------------|-------------------|
| Micro | EUR10K-30K/year | <EUR50M GWP |
| Starter | EUR30K-100K/year | EUR50-100M GWP |
| Professional | EUR50K-200K/year | EUR100-200M GWP |
| Growth | EUR200K-500K/year | EUR200M-500M GWP |
| Enterprise | EUR500K-2M/year | EUR500M-1B GWP |

[SOURCE: mysa_product_strategy.md, Part 3e]

**Why this works:** At a Caravela-sized carrier (EUR188M GWP, ~57K claims/year), a EUR100K/year platform license equals 0.05% of GWP. At EUR3/claim, that is EUR171K/year or 0.09% of GWP. Both are trivial relative to the potential savings (EUR562K-750K/year from STP improvement alone).

[SOURCE: mysa_product_strategy.md, Part 3e -- Caravela reference economics]

### What the Decision Engine Includes

Per-claim or platform pricing covers access to the full 6-step decision workflow:

| Step | What Mysa Does | Time Impact |
|------|---------------|-------------|
| 1. Coverage verification | AI reads policy, matches claim facts, highlights applicable coverage and exclusions | 15-30 min --> 2 min review |
| 2. Policy report checking | AI validates completeness, flags gaps, identifies contradictions | 10-20 min --> 1 min review |
| 3. Repair assessment | AI compares scope against comparable claims, flags anomalies | 15-25 min --> 3 min review |
| 4. Cost analysis | AI pulls comparable data, identifies outliers, calculates expected range | 10-20 min --> 2 min review |
| 5. Reserve calculation | AI calculates reserve with confidence interval, shows P&L impact | 10-15 min --> 2 min review |
| 6. Fraud detection | AI pattern-matches against fraud signals, scores risk, recommends SIU referral | 5-10 min --> automated flagging |

[SOURCE: mysa_product_strategy.md, Part 1 -- decision sub-steps and time estimates]

**Total decision time:** 65-120 minutes today --> 10-15 minutes with Mysa (4-8x improvement on the decision step).

---

## 10.2 Revenue Stream: Intake & Document Processing (Secondary)

### Why Intake Is a Revenue Stream (Not Just a Feature)

> "I think what is wrong with companies, and I think our value is here, but you cannot start here. Because it's garbage in garbage out. So if you already have a lot of garbage in, you need to start by fixing that."
> -- Tiago Brigido [TRANSCRIPT: Feb 7, 2026]

The decision engine requires clean, structured data. Carriers do not have it. Mysa must fix "garbage in" as a prerequisite to delivering decision value -- and that fix is independently valuable enough to charge for.

[SOURCE: mysa_product_strategy.md, Part 2e -- garbage in garbage out; CLAUDE ANALYSIS on intake as data pipeline]

### Intake Pricing: Two Buyer Types

**A. Carrier Document Processing**

Carriers need incoming claim documents (EAS forms, invoices, photos, police reports, medical records) parsed, structured, and validated before decisions can begin. Current state: manual data entry, 20-30 minutes per document set, error-prone.

| Capability | Current Process | Mysa Process |
|-----------|----------------|-------------|
| EAS form extraction | Manual data entry (20-30 min, error-prone) | OCR extraction (2 min, 81.5% accuracy) |
| Convention matching | Manual lookup after data entry | Instant deterministic matching from structured data |
| Document completeness | Adjuster eyeballs it, misses gaps | AI flags missing fields, auto-generates follow-up requests |
| Data structuring | Typed into CMS by hand | Auto-populated structured data, validated against business rules |

[SOURCE: mysa_product_strategy.md, Part 6c -- EAS process comparison; caravela-ocr.md -- 81.5% accuracy]

**Pricing model:** Bundled into the per-claim or platform pricing above. Document processing is the data pipeline -- it feeds the decision engine. Charging separately risks creating a perception that Mysa is "just another intake tool." Bundling keeps the narrative on decisions.

**B. Broker Intake Flow (Standalone Revenue Opportunity)**

Brokers submit claims on behalf of policyholders. Today this is email-based, unstructured, and creates the "garbage in" problem at source.

| Capability | Description |
|-----------|-------------|
| White-labeled FNOL forms | Carrier-branded intake forms for brokers |
| Email-to-claim creation | Chrome extension / email parser creates structured claims from broker emails |
| AI gap analysis | Flags missing information before submission, reducing back-and-forth |
| Auto-outreach | Draft SMS/email to policyholder requesting missing info |

[SOURCE: mysa_product_strategy.md, Part 1 -- broker FNOL flow; Part 5a -- product flow architecture]

**Pricing model:** Per-submission fee or bundled into carrier platform license. When a carrier licenses Mysa, broker intake is included (it improves the carrier's data quality). Standalone broker tools could be offered as a lighter entry point for carriers not yet ready for the full decision engine.

### Cost to Deliver

LLM processing cost for the full Mysa stack (gap filling, pattern learning, second opinion, email parsing, appeal drafting, clinical suggestions, contract parsing):

**~$6.50/month per 100 claims**

| Use Case | Calls/Month (per 100 claims) | Avg Tokens | Cost |
|----------|------------------------------|-----------|------|
| Gap Filling | 200 | 500 | $0.50 |
| Pattern Learning | 30 | 2,000 | $0.60 |
| Second Opinion | 50 | 1,500 | $3.00 |
| Email Parsing | 100 | 500 | $0.25 |
| Appeal Drafting | 10 | 2,000 | $1.00 |
| Clinical Suggestions | 150 | 500 | $0.38 |
| Contract Parsing | 5 | 3,000 | $0.75 |
| **Total** | | | **~$6.50/month** |

[SOURCE: LLM_ARCHITECTURE.md -- cost estimation table]

**At scale (Caravela: ~57K claims/year = ~4,750 claims/month):**
- LLM cost: ~$309/month = ~$3,700/year
- At EUR100K/year platform pricing: LLM cost is **~3.7% of revenue**
- At EUR3/claim pricing (EUR171K/year): LLM cost is **~2.2% of revenue**

This is an exceptionally high gross margin business. LLM costs are negligible relative to revenue.

---

## 10.3 Unit Economics: Per Adjuster

This is the math the VP Claims runs when deciding whether to buy.

### Current State (Without Mysa)

| Metric | Value | Source |
|--------|-------|--------|
| Fully loaded cost per adjuster | ~$110K/year | mysa_product_strategy.md, Part 2a; TRANSCRIPT |
| Caseload | ~125 open claims at any time | mysa_product_strategy.md, Part 2a |
| Claims closed per year | 300-480 | mysa_product_strategy.md, Part 2a |
| Cost per closed claim | $230-$370 | mysa_product_strategy.md, Part 2a |
| Time on decisions per claim | 65-120 minutes | mysa_product_strategy.md, Part 1 |
| Time on admin / data entry | 30-40% of total time | mysa_product_strategy.md, Part 2c |
| Annual attrition | 20% at carriers, 33% at TPAs | mysa_product_strategy.md, Part 2a |
| Knowledge loss per departure | ~6 years institutional knowledge | mysa_product_strategy.md, Part 2a |

[SOURCE: mysa_product_strategy.md, Part 2a -- adjuster economics]

### With Mysa: 3x Productivity

| Metric | Current | With Mysa | Change |
|--------|---------|-----------|--------|
| Claims closed/year per adjuster | 300-480 | 900-1,440 | **3x** |
| Cost per closed claim | $230-$370 | $75-$125 | **-67%** |
| Decision time per claim | 65-120 min | 10-15 min | **4-8x faster** |
| New hire time to productivity | ~6 years to full expertise | Weeks (SOP-guided workflows) | **Massive** |

[SOURCE: mysa_product_strategy.md, Part 2c -- 3x productivity math]

### Per-Adjuster Savings Calculation

```
Current cost per adjuster:                    $110,000/year
Current claims closed:                        300-480/year
Current cost per claim:                       $230-$370

With Mysa (3x throughput):
  Same adjuster now closes:                   900-1,440 claims/year
  Cost per claim:                             $75-$125
  Savings per claim:                          $155-$245

Total savings per adjuster:                   $45,000-$120,000/year
```

**The pitch:** Every adjuster on Mysa saves the carrier $45K-$120K per year in cost-per-claim efficiency. A 20-adjuster claims team saves $900K-$2.4M/year. Mysa costs EUR50K-200K/year for a Caravela-tier carrier. That is a **4.5-48x ROI on the labor economics alone** -- before reserve accuracy and STP improvements.

[SOURCE: mysa_product_strategy.md, Part 2c -- savings calculation]

### For a Mid-Tier TPA (200 Adjusters)

| Metric | Value |
|--------|-------|
| Current cost (200 adjusters x $110K) | $22M/year |
| Claims processed (200 x 390 avg) | ~78,000/year |
| With Mysa (3x): same team processes | ~234,000 claims/year |
| OR: reduce headcount by 2/3 for same volume | Save ~$14.7M/year |
| Realistic savings (blend of both) | **$9-24M/year** |

[SOURCE: mysa_product_strategy.md, Part 2c -- TPA savings calculation]

---

## 10.4 Unit Economics: Per Carrier

This is the math the CFO runs. Two value drivers: adjuster productivity (Section 10.3 above) and STP improvement.

### STP (Straight-Through Processing) Improvement

STP = claims resolved with minimal human intervention. Convention systems (EU motor) promise 60-70% STP. Actual delivery: ~10%. The gap is data quality at intake.

[SOURCE: mysa_product_strategy.md, Part 2b -- STP gap; MODULE_01_POSITIONING.md, Section 1.2]

**The STP math (Caravela-sized carrier, ~50K motor claims/year):**

```
Current STP rate:                             ~10%
Target STP rate with Mysa:                    40-50%
Delta:                                        30-40 percentage points

Additional claims processed via STP:          15,000-20,000/year
Time saved per STP claim:                     ~45 min
Total hours saved:                            11,250-15,000 hours/year
At EUR50/hour loaded cost:                    EUR562,500-EUR750,000 saved/year

Mysa charges:                                 EUR100K-200K/year
ROI on STP improvement alone:                 3-7x
```

[SOURCE: mysa_product_strategy.md, Part 6c -- STP improvement calculation]

### ACV by Carrier Tier

| Tier | GWP Range | Est. Claims/Year | Target ACV | Per-Claim Equivalent |
|------|----------|-----------------|-----------|---------------------|
| Micro | <EUR50M | ~5-15K | EUR10K-30K | EUR2-6/claim |
| Starter | EUR50-100M | ~15-30K | EUR30K-100K | EUR2-3/claim |
| **Professional (Caravela tier)** | **EUR100-200M** | **~30-60K** | **EUR50K-200K** | **EUR2-3/claim** |
| Growth | EUR200M-500M | ~60-150K | EUR200K-500K | EUR1.3-8/claim |
| Enterprise | EUR500M-1B | ~150K+ | EUR500K-2M | Custom |

[SOURCE: mysa_product_strategy.md, Part 3e]

### Combined ROI: Caravela-Tier Carrier

This is what the CFO sees in the sales proposal.

```
CARRIER PROFILE
  GWP:                                        EUR188M (Caravela reference)
  Motor claims/year:                          ~42,000
  Property claims/year:                       ~15,000
  Total claims:                               ~57,000/year
  Adjusters:                                  ~20-30 (estimated for 149-employee carrier)

MYSA ANNUAL COST
  Platform license:                           EUR100K-200K/year
  As % of GWP:                                0.05-0.11%

SAVINGS: STP IMPROVEMENT (motor only)
  STP rate improvement:                       10% --> 40-50%
  Additional STP claims:                      12,600-16,800/year
  Hours saved:                                9,450-12,600 hours/year
  Value at EUR50/hr:                          EUR472,500-EUR630,000/year

SAVINGS: ADJUSTER PRODUCTIVITY
  Per-adjuster savings:                       $45K-$120K/year
  For 25 adjusters:                           $1.1M-$3.0M/year (~EUR1.0M-EUR2.8M)

SAVINGS: RESERVE ACCURACY
  5% improvement in reserve accuracy:         EUR500K-EUR750K freed capital or avoided losses/year
  (Caravela lost EUR18M in one year from weather + poor reserve management)

TOTAL ANNUAL VALUE TO CARRIER
  STP savings:                                EUR472K-630K
  Productivity savings:                       EUR1.0M-2.8M
  Reserve accuracy:                           EUR500K-750K
  TOTAL:                                      EUR2.0M-4.2M/year

ROI
  Mysa cost:                                  EUR100K-200K/year
  Return:                                     EUR2.0M-4.2M/year
  ROI:                                        10-42x
```

[SOURCE: mysa_product_strategy.md, Parts 2a, 2c, 2d, 6c -- combined from adjuster economics, STP calculation, reserve accuracy; TRANSCRIPT -- Caravela EUR18M loss]

**Note:** The 10-42x ROI range is wide because it combines three value drivers with their own ranges. Even at the conservative end (3-7x ROI on STP alone), the investment is justified. The CFO presentation should lead with STP savings (most concrete, easiest to measure) and layer productivity and reserves as additional upside.

---

## 10.5 Pricing Tiers

### Tier Summary

| Tier | Target Carrier | GWP Range | Annual Contract | Per-Claim Overlay | EU Carrier Count (16 countries) | What They Get |
|------|---------------|----------|----------------|------------------|-------------------------------|--------------|
| **Micro** | Regional mutuals, niche writers | <EUR50M | EUR10K-30K/year | EUR5-8/claim | ~243-372+ | Decision engine (motor only), standard SOP templates, email support |
| **Starter** | Small multi-line carriers | EUR50-100M | EUR30K-100K/year | EUR3-5/claim | ~204-260+ | + Property module, custom SOP encoding, dedicated onboarding |
| **Professional** | Caravela-tier carriers | EUR100-200M | EUR50K-200K/year | EUR2-4/claim | ~96-165 | + Full decision engine (motor + property), convention systems, broker FNOL, priority support |
| **Growth** | Large multi-line carriers | EUR200M-500M | EUR200K-500K/year | EUR2-3/claim | ~30-47 | + Multi-country, API access, custom integrations, dedicated CSM |
| **Enterprise** | Major carriers approaching EUR1B | EUR500M-1B | EUR500K-2M/year | Custom | ~16-19 | + Full customization, on-premise option, SLA guarantees, dedicated team |

[SOURCE: mysa_product_strategy.md, Part 3e -- pricing tiers; market_landscape_overview.md, Section 2 -- carrier counts]

### Design Partner Pricing

| Partner | Terms | Rationale |
|---------|-------|-----------|
| Caravela | Free for 6 months, then EUR50K-100K/year | Design partner builds the product with us. Their data + feedback is worth more than revenue in Phase 1. |

[SOURCE: mysa_product_strategy.md, Part 3e -- design partner row]

### Pricing as % of GWP

A useful sanity check. Insurance technology spend is typically 0.1-0.5% of GWP for mid-market carriers.

| Tier | Low End (% GWP) | High End (% GWP) | Assessment |
|------|-----------------|------------------|-----------|
| Micro (EUR30K on EUR40M GWP) | 0.05% | 0.075% | Well within budget |
| Starter (EUR100K on EUR75M GWP) | 0.04% | 0.13% | Reasonable |
| Professional (EUR200K on EUR150M GWP) | 0.03% | 0.13% | Trivial relative to savings |
| Growth (EUR500K on EUR350M GWP) | 0.06% | 0.14% | Standard enterprise software |
| Enterprise (EUR2M on EUR750M GWP) | 0.07% | 0.27% | Justified by ROI |

All tiers sit comfortably below 0.3% of GWP. Given the 3-42x ROI demonstrated in Section 10.4, pricing has significant room to increase as the product matures and value proof accumulates.

### Per-Claim Pricing: When to Lead With It

Per-claim pricing is better for:
- **Landing new customers** -- low barrier, no large upfront commitment
- **TPAs** -- per-claim is the natural unit (they process claims for others)
- **Pilots and proof-of-concept** -- pay for what you use, prove value before committing
- **Volume-variable carriers** -- seasonal or catastrophe-driven claim volumes

Platform pricing is better for:
- **Revenue predictability** -- for Mysa and for the carrier's budget planning
- **High-volume carriers** -- per-claim gets expensive above ~60K claims/year at EUR3/claim
- **Multi-line carriers** -- bundling motor + property into one license

**Recommendation:** Offer both. Let the carrier choose. Most will start per-claim and migrate to platform as they scale.

[SOURCE: mysa_product_strategy.md, Part 3e -- CLAUDE ANALYSIS on per-claim vs platform pricing]

### Revenue Expansion: Property Upsell

Adding property to an existing motor customer increases revenue by 60-70% per carrier with zero new customer acquisition. 80-95% of carriers writing motor also write property.

[SOURCE: market_landscape_overview.md, Section 3 -- motor vs property; mysa_product_strategy.md, Part 9b]

| Carrier | Motor Revenue | + Property Revenue | Combined |
|---------|-------------|-------------------|---------|
| Micro | EUR10K-30K | +EUR6K-21K | EUR16K-51K |
| Starter | EUR30K-100K | +EUR18K-70K | EUR48K-170K |
| Professional | EUR50K-200K | +EUR30K-140K | EUR80K-340K |
| Growth | EUR200K-500K | +EUR120K-350K | EUR320K-850K |
| Enterprise | EUR500K-2M | +EUR300K-1.4M | EUR800K-3.4M |

---

## 10.6 Financial Projections

### [REQUIRES FOUNDER INPUT]

This section requires founder decisions on the following inputs before projections can be modeled:

**Revenue Projections -- Inputs Needed:**

| Input | Why It Matters | Notes |
|-------|---------------|-------|
| Year 1 revenue target | Sets hiring/spend plan | Design partner (Caravela) is free for 6 months. First paying customer timing drives this. |
| Year 1-3 carrier acquisition pace | 2 carriers/quarter? 5? 10? | Determines sales hiring, onboarding capacity, and infrastructure investment. |
| Average ACV assumption | EUR75K? EUR100K? EUR150K? | Depends on whether early customers are Starter or Professional tier. |
| Property upsell timeline | Month 8-14 per Module roadmap | Accelerates revenue 60-70% per carrier. Critical to model. |
| US market entry timing | Year 2? Year 3? | Changes TAM and required investment significantly. |

**Cost Projections -- Inputs Needed:**

| Input | Why It Matters | Notes |
|-------|---------------|-------|
| Current monthly burn rate | Determines runway from any raise | Pre-revenue burn = founders + infrastructure. |
| Current runway | How long until revenue or next raise needed | Critical for fundraising timeline. |
| Headcount plan (6/12/18 months) | Largest cost line | Engineering, sales, customer success, domain expertise. |
| Infrastructure costs | Cloud, LLM APIs, data storage | LLM costs are ~$6.50/month per 100 claims -- scales linearly. |
| Office / operational costs | If any | Remote-first reduces this significantly. |

**Projection Framework (to be completed with founder inputs):**

| Metric | Year 1 | Year 2 | Year 3 |
|--------|--------|--------|--------|
| Carriers (paying) | [TBD] | [TBD] | [TBD] |
| Average ACV | [TBD] | [TBD] | [TBD] |
| ARR | [TBD] | [TBD] | [TBD] |
| Headcount | [TBD] | [TBD] | [TBD] |
| Monthly burn | [TBD] | [TBD] | [TBD] |
| Gross margin | >90% (LLM costs are <4% of revenue) | >90% | >90% |
| Net burn | [TBD] | [TBD] | [TBD] |

**What we do know:**
- LLM cost per 100 claims: ~$6.50/month (scales linearly)
- At a Caravela-sized carrier (57K claims/year), LLM cost is ~$3,700/year vs EUR100K+ revenue = >96% gross margin on AI infrastructure
- The business is SaaS with recurring revenue -- no physical goods, no hardware
- Customer acquisition is direct sales to 1-2 decision-makers at mid-market carriers (3-6 month cycle)

---

## 10.7 Fundraising Plan

### [REQUIRES FOUNDER INPUT]

**Founder Signals from Calls:**

> "I think we need to raise as much money as ClaimSorted [EUR11.4M]"
> -- Tiago Brigido [TRANSCRIPT]

> "Further AI series A level [$30M]... on seed."
> -- Jeremy Blehaut [TRANSCRIPT]

[SOURCE: mysa_product_strategy.md, Part 9c -- pitch slide 12]

These are aspirational anchors, not decisions. This section requires founder alignment on:

**Decisions Needed:**

| Decision | Options | Considerations |
|----------|---------|---------------|
| Target raise amount | EUR2-5M (seed) vs EUR5-15M (large seed / Series A) | Depends on ambition timeline. Smaller raise = faster close, less dilution. Larger raise = faster hiring, multi-country expansion. |
| Use of funds allocation | Engineering / Sales / Operations / Buffer | Typical seed: 60% engineering, 20% sales, 10% operations, 10% buffer. |
| Timeline to raise | Q2 2026? Q3 2026? | Depends on current runway and Caravela traction milestones. |
| Equity allocation | Founder split, ESOP, investor % | Standard: 15-20% ESOP, 15-25% to seed investors. Must be decided before term sheet. |
| Investor profile | EU insurtech specialists? US generalist VCs? Angels? | EU investors understand the market. US investors validate the TAM story. |
| Valuation expectations | Pre-money based on comparable raises | ClaimSorted: EUR11.4M raised. Five Sigma: ~$20M raised. FurtherAI: $30M raised. Shift: $320M raised. These set the floor for what's possible in the category. |

**What the raise should fund (framework):**

| Priority | Investment | Rationale |
|----------|-----------|-----------|
| 1 | Engineering team (3-5 engineers) | Build the decision engine beyond OCR. SOP workflow engine, multi-country convention systems, property module. |
| 2 | First sales hire | Dedicated to EU mid-market carriers. Co-founders cannot sell and build simultaneously at scale. |
| 3 | Customer success (1 hire) | Onboarding carriers requires deep domain knowledge + technical support. |
| 4 | Infrastructure | Cloud, LLM APIs, data storage, security/compliance tooling. |
| 5 | Runway buffer | 18-24 months minimum to reach meaningful ARR milestone. |

**The TAM story for investors (validated):**

| Stage | TAM | Timeline | Narrative |
|-------|-----|----------|-----------|
| Wedge | EUR2.7-18.6M (Southern EU, Caravela tier, motor only) | Year 1 | Proves the product works |
| Year 2-3 | EUR80-170M (all EU mid-market, motor + property) | Year 2-3 | Real SaaS business |
| Year 3-5 | EUR160-425M (EU + US mid-market, both lines) | Year 3-5 | Venture-scale |
| Vision | EUR320M-1.1B (full addressable + expansion) | Year 5+ | IPO-scale |

[SOURCE: mysa_product_strategy.md, Part 9b -- TAM progression]

**The honest TAM narrative:**

"We start with EU motor -- the convention system wedge that nobody else has. Within 6 months, the same carrier pays us for property too (same AI, bigger problem, same buyer). By year 3, we're in the US with the same product. The market is ~11-28M claims/year in our target segment alone, 80-95M globally. And 90%+ of mid-market carriers have ZERO AI claims tools today."

[SOURCE: mysa_product_strategy.md, Part 9b -- TAM narrative]

---

## Key Numbers Summary (For Pitch Deck)

| Metric | Value | Source |
|--------|-------|--------|
| **Per-claim price** | EUR2-10/claim | Part 3e |
| **Platform price** | EUR50K-2M/year | Part 3e |
| **LLM cost per 100 claims** | ~$6.50/month | LLM_ARCHITECTURE.md |
| **Gross margin** | >96% (on AI infrastructure) | Calculated: $3,700 LLM cost vs EUR100K+ revenue |
| **Adjuster loaded cost** | ~$110K/year | Part 2a |
| **Claims per adjuster (current)** | 300-480/year | Part 2a |
| **Claims per adjuster (with Mysa)** | 900-1,440/year | Part 2c |
| **Cost per claim reduction** | $230-370 --> $75-125 (-67%) | Part 2c |
| **Savings per adjuster** | $45K-120K/year | Part 2c |
| **STP improvement** | 10% --> 40-50% | Part 6c |
| **STP savings (50K claims)** | EUR562K-750K/year | Part 6c |
| **Combined ROI (Caravela-tier)** | 10-42x | Section 10.4 calculation |
| **Addressable carriers (primary)** | 96-165 (EU Caravela tier) | market_landscape_overview.md |
| **Addressable carriers (full)** | 1,530-2,400 (EU + US all tiers) | Part 9b |
| **Target segment claims** | ~11-28M claims/year | market_landscape_overview.md |
| **Property upsell** | +60-70% revenue per carrier | Part 9b |
| **Market openness (EU mid-market)** | 90-95% untouched by AI claims tools | market_landscape_overview.md |

---

## Sources

| Source | Type | Sections Used |
|--------|------|--------------|
| `mysa_product_strategy.md` Part 1 | Primary -- decision sub-steps, time estimates | 10.1, 10.3 |
| `mysa_product_strategy.md` Part 2a-2e | Primary -- adjuster economics, STP gap, reserve accuracy, garbage-in problem | 10.2, 10.3, 10.4 |
| `mysa_product_strategy.md` Part 3e | Primary -- pricing model, tiers, Caravela economics | 10.1, 10.4, 10.5 |
| `mysa_product_strategy.md` Part 6c | Primary -- STP improvement calculation | 10.4 |
| `mysa_product_strategy.md` Part 9b-9c | Primary -- TAM, pitch deck, fundraising signals | 10.4, 10.7 |
| `LLM_ARCHITECTURE.md` | Secondary -- LLM cost per 100 claims | 10.2 |
| `market_landscape_overview.md` | Secondary -- carrier counts, market sizing, competitive landscape | 10.4, 10.5 |
| `MODULE_01_POSITIONING.md` | Cross-reference -- ICP, value proposition, adjuster demographics | 10.3 |
| Feb 7, 2026 Granola call | Transcript -- pricing ("50k to 1M"), Caravela EUR18M loss, mid-market strategy | 10.1, 10.4, 10.7 |
| Feb 8-9, 2026 Granola calls | Transcript -- productivity calculations, SOP workflows, fundraising anchors | 10.3, 10.7 |
