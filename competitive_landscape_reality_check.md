# Competitive Landscape Reality Check — Is This Already Solved?

*Research date: February 7, 2026*

---

## CCC Is Absolutely Moving Here

**CCC acquired EvolutionIQ for $730M** (closed Q1 2025). EvolutionIQ is an AI claims *guidance* platform — it tells adjusters what to do next on injury claims. CCC launched "Medhub for Casualty" in Q3 2025, which synthesizes medical records and gives auto casualty adjusters actionable insights. This is CCC moving from "here's the estimate" to "here's what the adjuster should do."

CCC also has their IX Cloud Platform connecting 35,000+ businesses and their Workflow product that automates routine tasks. They're building the single pane of glass. **But** — still US-only, still physical damage + casualty, no EU convention systems.

Sources:
- https://www.businesswire.com/news/home/20241220225656/en/CCC-Intelligent-Solutions-Announces-the-Acquisition-of-EvolutionIQ-the-Leading-AI-Guidance-Platform-for-Disability-and-Injury-Claims-Management
- https://www.cccis.com/news-and-insights/posts/cccis-expand-third-party-auto-casualty-offering-with-evolutioniq
- https://www.cccis.com/our-technology/ix-cloud-platform
- https://www.cccis.com/our-technology/workflow

---

## Allianz Already Built Their Own

**Allianz launched "Insurance Copilot"** in Austria in 2024 for automotive claims, now expanding to property and scaling to Asia. It uses GenAI to flag critical factors adjusters might miss, automate workflow tasks, and provide decision support. Human-in-the-loop — AI recommends, adjuster decides. They also launched "Project Nemo" — agentic AI that clears simple claims in hours after storms.

**Key insight: Allianz built it in-house for themselves, not as a product for other insurers.** That's the pattern with the big carriers — they build proprietary tools.

Sources:
- https://www.allianz.com/en/mediacenter/news/articles/250205-smarter-claims-management-smoother-settlements.html
- https://www.allianz.com/en/mediacenter/news/articles/251103-when-the-storm-clears-so-should-the-claim-queue.html

---

## The Startup Landscape Is Crowded

| Company | What They Do | Funding | Market |
|---|---|---|---|
| **Five Sigma / Clive** | Multi-agent AI adjuster copilot on top of any CMS | $20M | 70% US, 30% EU |
| **Avallon** | AI agents for calls, emails, doc triage, data entry | $4.6M seed (YC S25) | US (workers comp + auto) |
| **Strada** | Voice AI agents for insurance FNOL + workflows | YC-backed | US |
| **ClaimSorted** | AI-first TPA, 3x faster settlements | $13.3M | US + UK + EU |
| **Shift Technology** | Fraud → full claims automation (Sept 2025) | $320M | 25+ countries |
| **Majesco Copilot** | GenAI copilot embedded in their CMS | Public company | US |

Plus **Microsoft Copilot for Insurance** through Avanade, **EvenUp** (plaintiff-side AI for BI claims), and **DigitalOwl** (acquired by Datavant for medical record analysis).

Sources:
- https://fivesigmalabs.com/clive/
- https://www.businesswire.com/news/home/20251106838494/en/Avallon-Secures-4.6-Million-Scales-AI-Agents-to-Automate-Insurance-Claims-Operations
- https://www.getstrada.com/
- https://www.claimsorted.com/
- https://www.shift-technology.com/products/claims
- https://www.majesco.com/analytics-solutions-insurance-solutions/insurance-data-analytics/copilot-genai/
- https://www.avanade.com/en/services/artificial-intelligence/ai-copilot-hub/insurance-ai-copilot
- https://www.ycombinator.com/companies/strada

---

## So Why Hasn't It Been "Solved"?

It hasn't been solved because **it's genuinely hard**, not because nobody is trying:

1. **Legacy system integration is brutal.** 74% of insurers still run some legacy tech. Guidewire, Duck Creek, Sapiens, mainframe — each integration is a 6-12 month project. CCC's own integration with Guidewire took years. Every insurer is different.

2. **Regulatory fragmentation.** 50 US states with different settlement timing rules. EU has country-by-country conventions (IRSA, CARD, CIDE, IDS) plus GDPR. No one has built the "universal" layer because the rules differ everywhere.

3. **The incumbents defend their turf.** CCC sued Tractable for 5 years over anti-competitive behavior. Guidewire partners selectively. These aren't open ecosystems — they're walled gardens.

4. **Adjusters resist change.** The research says "enterprise-wide adoption is not plug-and-play — it requires thoughtful process redesign, adjuster upskilling, and robust change management." Tools that adjusters don't adopt are worthless.

5. **The TAM is real but fragmented.** Claims management market: $5.15B (2024) → $13.95B by 2032. AI in claims processing growing at 28.4% CAGR. But buyers are scattered across carriers, TPAs, and MGAs of all sizes.

Sources:
- https://www.fortunebusinessinsights.com/claims-management-market-110629
- https://uk.finance.yahoo.com/news/ai-insurance-claims-processing-market-080700546.html
- https://www.sas.com/en_us/news/press-releases/2025/december/insurance-ai-operating-system.html

---

## The Honest Assessment

**The "adjuster operating system" is being built — by multiple players, from multiple angles.** CCC is coming from estimating. Five Sigma from CMS. Shift from fraud. Allianz from inside. Avallon and Strada from voice/workflow. Microsoft from the platform layer.

What's *genuinely* not being done by anyone:

- **EU convention systems natively** (IRSA, CARD, IDS, CIDE) — nobody, confirmed across all competitors
- **US + EU in a single product** — everyone is either US-centric or EU-centric
- **Decision ground truth capture** — everyone automates the workflow, nobody captures *why* the adjuster decided what they decided (which is the training data moat)
- **The EAS data quality problem** — the 50-point STP gap that the research identified is genuinely unaddressed

But you should be clear-eyed: **this is a crowded, competitive space where well-funded players are converging.** The question isn't "is the opportunity real?" — it clearly is, given $730M acquisitions and $320M funding rounds. The question is whether Mysa's specific angle (EU conventions + decision ground truth + US/EU in one product) is differentiated enough to win against players with 100x more data and capital.

That's the real co-founder conversation.
