# Raw Positioning Synthesis — Feb 11, 2026

## Sources
- FOS v1 document (fos/MYSA_FOS_v1.md)
- Feb 9: Claims workflow and triage process optimization (Jeremy + Tiago)
- Feb 10: Insurance claims workflow automation with Joaquim (Crisur)
- Feb 11: Insurance workflow platform strategy and product positioning (Jeremy + Tiago)

## What happened across 3 days

### Feb 9 — Product deep dive
- Mapped 11 claim phases, all stakeholders (field adjusters, BI adjusters, SIU, supervisors, appraisers, medical case managers)
- SOPs feed workflows, workflows contain agents
- FNOL intake → triage → investigation → assessment → decision → settlement
- US vs EU differences: calls required in US, electronic in EU (GDPR checkbox)
- White-label FNOL portal identified as killer feature for brokers
- Triage has: classification, severity scoring, coverage checks, fraud detection
- Integration landscape: Guidewire (Policy Center, Claims Center), Duck Creek, CCC, Mitchell
- CCC/Mitchell dominate auto assessment with 50-year data moats
- No equivalent tool for property/home assessment = opportunity
- Forward-deployed model: 2 months onboarding, historical data training
- Product is a "proactive claims orchestrator"

### Feb 10 — Joaquim meeting (Crisur, 8th largest insurer worldwide)
- Uses GIZ as their information system
- Confirmed product makes more sense for INSURERS than brokers
- Simple auto claims (DAA) too basic for the product
- Real value on COMPLEX claims: property, multi-party, contestações
- Offered forward deployment day at Porto office
- Communication automation (back-and-forth) resonated most
- Quote: "The things truly useful are where you need reports, technical assessments, multiple documents"
- Caution: cannot take decisions without consulting hierarchy (England/global)
- He helped develop software at previous insurers, created manuals, knows gaps

### Feb 11 — Positioning debate (Jeremy + Tiago, ~2 hours)
Core tension:
- Tiago: Generic document intelligence company for claims. Parse, extract, create docs. Adjusters are one consumer.
- Jeremy: Adjusters are the moat — most underserved, most complex. But too complex for day 1.

What they agreed on:
- Company = data extraction, data parsing, data upload, data creation
- "Further AI for claims" — Further AI does underwriting, Mysa does claims
- Forward-deployed: 2 months onboarding, reverse-engineer historical claims + SOPs
- Human-in-the-loop: prepare decisions, humans decide
- Not a CMS replacement (not Guidewire, not Duck Creek)
- Not a chatbot ("you don't upload and ask questions")
- Not STP automation (serve the complex 20% that consumes 80% of time)
- Present "decision-ready" claims, not decisions

Architecture = "Lego blocks":
- Building blocks (OCR, email parsing, doc gen, SOP parsing) compose into workflows
- Workflows serve different stages and personas
- Agents operate within workflows with guardrails

Adjuster debate resolution:
- Day 1: generic doc intelligence across claim journey
- Day 2+: deeper adjuster tooling once we have data from forward deployments
- Adjusters need image/voice/field analysis = too complex for day 1
- But the moat IS there — nobody serves them well

Demo feedback:
- Too static, data already exists
- Missing inbox view
- Too crowded
- Customer/Onboarding cards don't belong
- Lead with product, not problem
- Show old vs new comparison
- Show specific use cases (like competitors)

Website feedback:
- Too complex, too generic
- Should be simpler, YC-style
- Hero section fine, title needs to be stronger
- Demo should come right after hero
- Platform section should show specific use cases
- Show motor flavors, generic enough for US

Expansion sequence agreed:
- Motor EU → Property/Home EU → Motor US → Property/Home US
- Brokers = B2B2B exploration, not primary focus
- "Cancer strategy" — expand everywhere from the doc intelligence core

Pitch needs:
- Send something to investors this week
- Mention live with mid-size MGA in Europe
- Building for US readiness
