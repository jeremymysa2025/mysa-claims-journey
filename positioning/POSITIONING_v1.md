# Mysa — Positioning & Product Direction v1
**Date:** Feb 11, 2026
**Status:** Working draft — needs Tiago review

---

## 1. Positioning

### 1.1 What Mysa does (plain English)
When an insurance company receives a claim, people spend hours reading documents, checking policies, emailing customers for missing info, and writing reports. Mysa reads all the documents for them, tells them what's missing, sends the follow-ups, and writes the reports. We also turn their internal procedures (SOPs) into step-by-step workflows so nobody has to memorize how things work.

### 1.2 One-liner
**Mysa automates the document work in insurance claims — extraction, follow-up, and report generation — so people spend time deciding, not gathering.**

### 1.3 For investors
> Insurance claims involve 5-10 people, 20+ documents, and weeks of back-and-forth before anyone makes a decision. 70% of that time is document processing, not thinking. Mysa automates the document work: we extract data from every document in a claim, flag what's missing, send automated follow-ups, and generate the reports adjusters need. We turn each insurer's SOPs into AI-guided workflows.
>
> We're live with a mid-size MGA in Europe for motor claims. We're building for the US. We start with document processing — which gets us into every stage of the claim — and use that data to eventually own the decision-preparation step, which nobody does today.

### 1.4 For insurance company buyers (Chief Claims Officer, Head of Operations)
> Your team opens 5-7 systems per claim, spends an hour gathering documents, and another hour writing reports. Mysa connects to your email and your existing tools. We parse every document that comes in, check it against what your workflow requires, and flag gaps immediately. If something's missing, we draft the follow-up. When it's time to write a report, we generate it from the data we already have.
>
> You keep your systems. You keep your people. They just stop doing the manual part.

### 1.5 For brokers
> You get an email from a client with a claim. You need to figure out what insurer to send it to, what documents that insurer requires, and chase the client for whatever's missing. Mysa does that automatically. We know what Fidelidade needs vs what AXA needs. We parse the email, check the gaps, and draft the follow-up. Your team reviews and clicks send.

### 1.6 For adjusters / claim handlers
> When you open a claim, everything is already there: documents parsed, fields extracted, SOP steps laid out. You don't search through emails or PDFs. You ask a question, you get the answer from the data we already have. When you need to write a report, we draft it.

### 1.7 Competitive framing
- **vs. Pace.ai** — They do claim intake (FNOL extraction). They stop there. We go further: SOP workflows, document generation, follow-up automation across the whole claim.
- **vs. Further AI** — They do underwriting. We do claims. Same approach (document processing + workflows), different part of the insurance chain.
- **vs. Five Sigma / Shift** — They sell to large carriers with existing platforms. We sell to mid-market (EUR 100-200M GWP) that can't afford custom AI teams.
- **vs. Guidewire / Duck Creek** — They are the system of record (CRM). We sit on top. We don't replace them, we read from them and write back.
- **vs. CCC / Mitchell** — They own auto damage estimation with 50-year data moats. We don't compete there. We handle everything around the estimation: the documents, the comms, the workflows.

---

## 2. Building Blocks

The product is made of components that compose into workflows. Each component does one thing.

| # | Block | What it does | Status |
|---|-------|-------------|--------|
| 1 | **Document Parser (OCR)** | Reads PDFs, images, emails. Extracts structured fields. Handles handwritten content (DAA parte B). | Live — used in Caravela |
| 2 | **Gap Analysis** | Compares extracted data against workflow requirements. Returns list of what's missing. | Built |
| 3 | **Email Drafting + Sending** | Generates follow-up emails to request missing documents. Human reviews before send (or auto-send). | Built |
| 4 | **SOP Parser** | Reads SOP documents, extracts steps, generates workflow definitions. | Partial |
| 5 | **Knowledge Base (Vault)** | Stores policies, SOPs, historical claims. Chat interface to ask questions across all sources. | Partial |
| 6 | **Workflow Engine** | Executes step-by-step processes. Routes tasks to right person. Sends notifications. Tracks status. | Built |
| 7 | **Document Generator** | Creates FNOL reports, contestações, investigation summaries, settlement letters from extracted data. | Partial |
| 8 | **White-label FNOL Portal** | Branded form for end-customers to submit claims directly. Includes GDPR consent. Optional call booking. | Not built |
| 9 | **Phone/Call Integration** | Record calls, transcribe, extract fields from conversation. Required for US market. | Not built |
| 10 | **CMS Connectors** | Pull/push data from Guidewire, Duck Creek, GIZ, or any JSON-based system. | Not built |

### 2.5 Blocks that sell standalone to enterprise

Some blocks are useful even without buying the full platform. These are entry points for large accounts that already have systems but need specific capabilities.

| Block | Standalone product | Who buys it | Example use case |
|-------|-------------------|-------------|-----------------|
| **Document Parser** | "Claims Document API" — send us any claims document, get structured JSON back | Any company processing claims docs. TPAs, assistance companies, insurtechs. | Europ Assistance Portugal receives 100k+ claims/year. Their call center manually reads every email and PDF to enter data into their system. We give them an API: send the doc, get the fields. They plug it into their existing workflow. |
| **SOP Parser + Workflow Generator** | "SOP-to-Workflow" — upload your procedures, get executable workflows | Mid-market carriers doing digital transformation. Compliance teams. | An insurer has 200 pages of procedures that nobody reads. We scan them, generate step-by-step workflows with triggers and notifications. They can edit and deploy. |
| **Knowledge Base / Vault** | "Claims Knowledge Search" — unified search across all your policies, SOPs, and historical claims | Any claims team drowning in documents | An adjuster handling a water leak claim needs to check: is this covered? What's the policy limit? What happened last time on this address? One search, all answers. |
| **Gap Analysis + Follow-up** | "Claims Completeness Checker" — check if a submission has everything needed, auto-draft the follow-up | Brokers, TPAs, assistance companies | A broker receives a property claim email. Our tool checks it against what Fidelidade requires, identifies 3 missing documents, drafts the email to the client. 2 minutes instead of 30. |
| **White-label FNOL Portal** | "Digital Claims Intake" — branded portal for end-customers to submit claims | Brokers and small MGAs without digital intake | A broker with 4,000 claims/year and no portal. We give them a branded page where their clients submit claims with all required documents. Reduces back-and-forth by 60%+. |

**Go-to-market for standalone blocks:**
- Lead with the Document Parser API for assistance companies (Europ Assistance call is the proof point)
- SOP-to-Workflow sells to compliance/ops teams during insurer onboarding
- Knowledge Base is the upsell once they're on the platform
- FNOL Portal is the broker acquisition tool

---

## 3. Website Changes (meetmysa.com)

### Current problems
- Too generic. Reads like "we do AI for insurance" — could be anyone.
- Problem statement is vague ("70% of time on process"). Doesn't say what process.
- Demo is buried. Should be front and center.
- No specific use cases. Just abstract feature descriptions.
- Missing "old vs new" comparison that shows the actual pain.

### Proposed structure

**Hero section** (keep, but tighten the title)
- Current title is weak. Needs to be specific.
- Suggested: "Stop chasing documents. Start closing claims." or "Every document in your claim, parsed and ready — before you open it."
- Keep the CTA: "Book a demo" + "See it in action"
- Add: "Live with insurers in Europe. Building for the US."

**Section 2: Demo embed** (move UP from bottom)
- Put an interactive demo or video right after the hero.
- This is what you and Tiago agreed: "catches your attention right away."
- Short product walkthrough: email arrives → parsed → gaps flagged → follow-up sent → FNOL ready.

**Section 3: Three things we do well** (replace the current generic platform section)

Card 1: **Document extraction & follow-up**
- "An email arrives with a claim. We parse every attachment — PDFs, photos, handwritten forms. If documents are missing, we draft the follow-up. Your team reviews and clicks send."
- Show: before (manual email reading, 45 min) → after (auto-parsed, 2 min)

Card 2: **Search across everything**
- "Ask a question about any claim, policy, or procedure. Get the answer from all your documents instantly. No more Ctrl+F across 100 files."
- Show: adjuster asking "what's the coverage limit for water damage on this policy?" → instant answer with source.

Card 3: **SOP workflows & notifications**
- "Upload your procedures. We turn them into step-by-step workflows. Every person touching a claim knows exactly what to do next. Notifications go out automatically."
- Show: SOP document → generated workflow → notification sent to adjuster

**Section 4: Use cases** (new — specific, not generic)
- Motor claims (EU): DAA parsing, FNOL generation, insurer submission
- Property claims: Multi-document intake, contestação drafting, investigation support
- Broker operations: Multi-insurer management, white-label intake, proactive follow-up

**Section 5: How we work with you** (the forward-deployed pitch)
- "We spend 2 months with every new customer. We study your historical claims, learn your SOPs, and configure workflows specific to your processes. Then we go live."
- This is different from everyone else. Call it out.

**Section 6: Who we are**
- Keep brief. Founded in 2025. European-native. Building for global.

**Footer**
- Book a demo (Calendly)
- Social links

### What to remove
- Generic "AI-powered claims platform" language
- Any mention of "dashboard" or "analytics"
- The "Full-service claims operations or AI-powered automation" tagline (too vague)

---

## 4. Demo Changes

### Current demo (5 cards)
1. Customer Experience — **Remove.** Not our buyer.
2. Insurance Portal — **Rework.** Too static. Needs inbox + workflow.
3. Insurer Onboarding — **Remove.** Internal concern, not a sales demo.
4. Adjuster Workspace — **Keep + rework.** Needs inbox view, less clutter.
5. Broker View — **Keep.** Joaquim validated this resonates.

### Proposed demo (3 flows)

**Flow 1: Claim Intake (for insurers and brokers)**
What happens:
1. Email arrives in inbox view (not a pre-filled dashboard)
2. System parses all attachments automatically
3. Gap analysis runs: "Missing: repair estimate, photos of damage"
4. Draft follow-up email appears: "Dear [customer], we need the following..."
5. Human clicks send (or auto-sends based on config)
6. Customer submits missing docs via white-label portal link
7. FNOL is generated, ready for submission

Why this works: It shows the PROCESS, not the result. Something arrives, you handle it.

**Flow 2: Claims Workspace (for claim handlers / adjusters)**
What happens:
1. Inbox view: 12 claims assigned, sorted by urgency
2. Open a claim: all context pre-loaded (parsed docs, extracted fields, timeline)
3. SOP checklist on the left: "Step 1: Verify coverage ✓ | Step 2: Request repair estimate ⏳"
4. Knowledge base on the right (collapsed by default, chat-style): ask "is water damage covered under this policy?" → answer with source
5. Generate investigation report: one click, pre-filled from extracted data
6. Assign next step to someone, notification sent automatically

Why this works: It's an inbox + workflow, not a dashboard. The adjuster opens it every day.

**Flow 3: Broker Claims Management**
What happens:
1. Multi-insurer view: claims grouped by insurer
2. Workflow per insurer: "Fidelidade requires X, AXA requires Y"
3. Contestação drafting: AI writes the argument based on policy + claim data
4. White-label portal: show the branded intake form
5. Notifications: "Claim #1234 has been waiting 5 days for repair estimate"

Why this works: Brokers deal with multiple insurers. Nobody gives them a unified tool.

### Design principles for all flows
- **Inbox-first**: something arrives, you process it
- **Collapse complexity**: show steps one at a time, not everything
- **AI assistant as side chat**: not a full panel, just a collapsed chat
- **Before/after**: each flow starts with "here's how it works today" vs "here's how it works with Mysa"

---

## 5. Launch Sequence

### Phase 1: NOW (Feb-Mar 2026) — Motor EU, document processing
**What we sell:** Claim intake automation + document follow-up for motor claims in Southern Europe.
**Who we sell to:** Mid-market MGAs and brokers (Caravela tier: EUR 100-200M GWP).
**What we need to build:** Tighten what exists. Inbox view. Gap analysis polish. Email auto-draft.
**Proof points:** Caravela (live). Joaquim/Crisur (forward deployment scheduled). Broker meeting (Jorge).
**Website:** Simplified. Three use cases. Demo front and center.
**Demo:** Three flows as described above. Not five cards.

### Phase 2: Q2 2026 — Property/Home EU
**What changes:** New SOP templates for property. New document types (repair estimates, technical reports, photos). Contestação workflow (this is where Joaquim said the real value is — the 70m wall case).
**What we reuse:** Same blocks. Same inbox. Same workflow engine. Just different configs.
**Why now:** Joaquim's team handles property. Same customer, new use case. Smallest step.

### Phase 3: Q3-Q4 2026 — Motor US prep
**What changes:** Call recording + transcription (mandatory in US). Different FNOL templates. State-specific compliance (California law). Integration with Guidewire Claims Center.
**What we need to build:** Phone/call block (#9). CMS connectors (#10). US-specific SOP templates.
**Why this order:** Motor is same vertical (reuse domain knowledge), US is new market (need relationships). Don't enter US with a new vertical AND new market simultaneously.

### Phase 4: 2027 — Property/Home US + broker B2B2B
**What changes:** Property/home in US is close to EU (same block types). Broker model is B2B2B — sell through brokers to reach multiple insurers.
**What we need:** Scale. Sales team in US. Partnerships.
**Why last:** Home assessment has no dominant tool (unlike CCC for auto). This is the opportunity, but it requires volume and local data to build estimation capabilities.

### Standalone block sales (parallel track)
- Document Parser API: pitch to Europ Assistance and similar assistance companies NOW
- White-label FNOL Portal: pitch to brokers without portals NOW
- SOP-to-Workflow: pitch during forward deployments with insurers

---

## Open Questions
1. **Triage**: We don't know enough about how to help with triage beyond document completeness. Park for now. Revisit after Joaquim forward deployment.
2. **Adjuster deep tooling**: Image analysis, voice analysis, field investigation support. This is the moat but requires capabilities we don't have. Revisit after accumulating data from Phase 1-2.
3. **CMS integration priority**: Guidewire vs Duck Creek vs GIZ. Depends on customer pipeline. Don't build speculatively.
4. **Pricing**: Per-claim (EUR 2-8) vs platform license (EUR 10K-2M/year). Need to test both with Joaquim and next customers.
5. **Europ Assistance call**: Can we sell Document Parser as standalone API? Need to scope the call.
