# Mysa — Positioning & Product Direction v1
**Date:** Feb 11, 2026
**Status:** Working draft — needs Tiago review

---

## 1. Positioning

### 1.1 What Mysa does (plain English)
When an insurance company gets a claim, people spend hours opening PDFs, reading emails, checking if documents are missing, calling the customer back, and then typing everything into their system. Then they do it again for the next claim. Mysa does the reading, the checking, and the typing. We also chase the customer when something is missing and write the reports at the end. If the company has procedures (SOPs), we turn those into checklists so nobody forgets a step.

### 1.2 One-liners (pick one)

**Option A — action-focused:**
Mysa reads every document in an insurance claim, finds what's missing, and gets it — so people can skip straight to the decision.

**Option B — before/after:**
Claims teams spend 70% of their time reading documents and chasing missing info. Mysa does that part.

**Option C — product-focused:**
Mysa is a claims workflow tool that parses documents, chases missing info, and writes reports — for every person touching a claim.

**Option D — category-creating:**
Mysa is the back-office your claims team doesn't have. We read the docs, do the follow-ups, and prep every claim for decision.

**Option E — YC-style (what + for whom):**
We automate document processing for insurance claims. Motor in Europe today, US next.

**Option F — short and blunt:**
We do the paperwork in insurance claims. Faster and cheaper than people.

### 1.3 For investors

**Version A — 30-second pitch:**
> An insurance claim touches 5-10 people and 20+ documents before anyone decides anything. Most of the time is spent gathering — opening PDFs, checking policies, emailing customers for missing stuff, writing reports. Not deciding.
>
> Mysa automates the gathering. We read every document in a claim, compare it to what's needed, chase whatever is missing, and write the output reports. We do this by turning each insurer's internal procedures into workflows our software follows.
>
> We're live with a mid-size insurer in Europe doing motor claims. Next: property in Europe, then US.

**Version B — with the moat angle:**
> Every insurance company has different procedures for handling claims. Different documents required, different steps, different people involved. Nobody has standardized this because it's too specific per company.
>
> Mysa sits with each insurer for 2 months, learns their procedures, and turns them into automated workflows. Once we're in, we're hard to replace — the workflows are built on their specific processes.
>
> Day one, we automate document extraction and follow-up. Over time, we accumulate enough data on how decisions get made to start preparing decisions, not just documents. Nobody owns that data today.

**Version C — TAM and traction:**
> 80-95 million motor and property claims per year across EU and US. Each one involves hours of manual document processing. The tools that exist (Guidewire, Duck Creek) are systems of record — they store data, they don't process it.
>
> Mysa processes it. We extract, we follow up on gaps, we generate reports. We sell per-claim (EUR 2-8) or as a platform license (EUR 10K-2M/year). At a EUR 100M GWP insurer handling 30K claims/year, a EUR 100K license pays for itself in 3 months through time savings alone.
>
> Live with one MGA in Portugal. Forward deployment scheduled with the 8th largest insurer worldwide. Pipeline in Southern EU and US.

### 1.4 For insurance company buyers

**For the Chief Claims Officer:**
> Your people open the same types of PDFs every day, check the same fields, send the same follow-up emails, and write the same reports. The only part that actually needs a human is the decision at the end.
>
> Mysa handles everything before the decision. We connect to your email. We read every document. We check it against your procedures. We flag what's missing and draft the follow-up. When your team opens a claim, it's ready.
>
> We don't touch your systems. We sit on top of what you already have.

**For the Head of Operations / IT:**
> We integrate with your email (Outlook, Gmail). We can read from your claims system if it has an API (Guidewire, Duck Creek, or anything with JSON access). We don't require migration. We don't replace anything.
>
> Deployment takes ~2 months. We study your historical claims and SOPs, configure workflows specific to your processes, and go live. Your team uses a web app — inbox-style, not a dashboard.

**For a TPA / Assistance company CEO:**
> You process claims on behalf of insurers. Each insurer has different requirements, different documents, different procedures. Your team has to remember all of it — or look it up every time.
>
> Mysa knows the requirements per insurer. When a claim comes in, we parse the documents, check against the right insurer's requirements, and flag the gaps. Your team stops being a human router and starts being a reviewer.

### 1.5 For brokers

**Version A — small broker (< 5,000 claims/year):**
> You get emails with claims. You figure out which insurer to send them to. You check if the documents are complete. You email the client back for what's missing. You wait. You follow up again. Then you submit.
>
> Mysa does steps 2 through 6. You review the result and click send. We also give you a branded portal so your clients can submit claims with all the right documents from the start — no back-and-forth.

**Version B — larger broker with multiple insurers:**
> You work with 10+ insurers, each with different document requirements. Mysa knows what each one needs. When a claim comes in, we auto-match it to the right insurer, check the documents against their requirements, and handle the follow-up. You manage everything from one screen instead of 10 portals.

### 1.6 For adjusters / claim handlers

**Version A — the busy adjuster:**
> You get assigned a claim. Instead of spending 45 minutes reading emails, opening PDFs, and figuring out what happened — you open it and it's all there. Documents parsed. Fields filled. Timeline built. Your SOP steps listed. You start at the decision, not at the reading.

**Version B — the field investigator:**
> You arrive on site and you already have the full claim summary: what happened, what documents exist, what's been said, what's still missing. After your inspection, you type your findings and we generate the report. You don't write it from scratch.

**Version C — the supervisor:**
> You see every claim your team is handling, where each one is stuck, and why. If a claim is blocked because a document is missing, you see it. If an SOP step was skipped, you see it. You don't need to open each claim to know what's going on.

### 1.7 For the website hero (options)

**Option A:** "Stop chasing documents. Start closing claims."
**Option B:** "Every claim, parsed and ready — before you open it."
**Option C:** "Your claims team spends 70% of their time gathering. We do that part."
**Option D:** "We read the documents. You make the decisions."
**Option E:** "Claims automation that works with your systems, not instead of them."
**Option F:** "From email to decision-ready. Automatically."

### 1.8 Competitive framing

**vs. Pace.ai**
They extract data from the first notice of loss. That's one step. We do extraction + gap analysis + follow-up + document generation + SOP workflows across the full claim. They built a funnel. We built the operating system around it.

**vs. Further AI**
Same playbook, different side of insurance. They do underwriting (quotes, submissions, policy binding). We do claims (FNOL, triage, investigation, settlement). No overlap today. If they move into claims, we're already there with workflow depth they'd need to rebuild.

**vs. Five Sigma**
They built a claims management system (CMS) — a Guidewire alternative for smaller carriers. We're not a CMS. We sit on top of whatever CMS you have. We don't store your claims, we process the documents around them. Different sale, different buyer, compatible products.

**vs. Shift Technology**
Fraud detection and claims automation for Tier 1 carriers (AXA, Zurich). They need 100K+ claims/year to train their models. We sell to mid-market carriers with 10K-60K claims/year who can't afford Shift's pricing or implementation. Different segment entirely.

**vs. Guidewire / Duck Creek**
They are the database. We are the document processor. They store the claim record. We read the emails, parse the PDFs, and write back the structured data. We need them (or something like them) to exist. We're not competing — we're adding a capability they don't have.

**vs. CCC / Mitchell / Verisk**
They own auto damage estimation. 50 years of parts pricing data. We will never compete with that. We handle everything that isn't the estimate itself: the document intake, the gap analysis, the follow-up, the report writing, the SOP enforcement. They do the number. We do the paperwork around the number.

**vs. Wami**
They do claim intake with a focus on FNOL creation. Their demo shows a chatbot-style interface. We go deeper: we don't just create the FNOL, we manage the entire document lifecycle of the claim — from first email to settlement letter. We also do SOP-to-workflow, which they don't touch.

**vs. building in-house**
An insurer with 600+ engineers (like Crisur/Ageas) could build this. But they won't, because claims automation is not their core business and internal projects take 2-3 years. We deploy in 2 months. We also bring cross-insurer patterns — we've seen how multiple companies handle the same claim types, so our workflows start better than anything built in isolation.

### 1.9 Category

We are not calling ourselves:
- ~~"AI-powered claims platform"~~ (everyone says this)
- ~~"Claims copilot"~~ (too vague, sounds like a chatbot)
- ~~"Claims decision engine"~~ (we don't make decisions)
- ~~"Insurtech"~~ (says nothing about what we do)

We could call ourselves:
- **"Claims document automation"** — boring but accurate
- **"Claims workflow software"** — what ops buyers search for
- **"Claims operations platform"** — what we used on Feb 9, still works
- **"Document processing for insurance claims"** — most literal

For now, use: **"Claims workflow and document automation"**
Revisit when we have a stronger opinion after 3-5 customers.

### 1.10 Sales blurb (send to insurers / MGAs)

**Version A — email intro (short, direct):**

> Hi [Name],
>
> We're Mysa. We automate the document work in insurance claims — extraction, gap detection, follow-up, and report generation.
>
> Your team reads documents, checks what's missing, emails the customer, waits, then writes a report. We do all of that automatically. Your people review the output and make the decision.
>
> We're already live with a European MGA on motor claims. We configure everything around your specific procedures — no migration, no system replacement.
>
> Would 30 minutes make sense to show you how it works on a real claim?

**Version B — email intro (with numbers):**

> Hi [Name],
>
> A motor claim takes your team 65-120 minutes of document processing before anyone makes a decision. Reading emails, opening PDFs, checking policy coverage, emailing the customer for missing documents, writing the FNOL, drafting reports.
>
> Mysa cuts that to 10-15 minutes. We parse every document automatically, flag what's missing, send the follow-up, and generate the reports. Your team opens the claim and it's ready for a decision.
>
> We're live in Europe for motor. We deploy in ~2 months — we study your historical claims and SOPs and configure workflows specific to how you work.
>
> Worth a quick call?

**Version C — for a warm intro / referral:**

> [Name] — [mutual contact] suggested I reach out.
>
> We built Mysa to solve a specific problem: claims teams spend most of their time on documents, not decisions. We automate the document part — reading, extracting, chasing missing info, generating reports.
>
> We're live with a mid-size MGA in Portugal on motor claims and have a forward deployment underway with [the 8th largest insurer worldwide]. We're expanding in Southern Europe and preparing for the US.
>
> Happy to show you a real demo — not slides, the actual product running on a real claim. 30 min?

**Version D — LinkedIn message (ultra short):**

> We automate document processing for insurance claims — extraction, follow-ups, reports. Live with European MGA on motor. Worth 15 min to show you?

### 1.11 Impact numbers (what we can claim today)

**What we can say with confidence (based on Caravela + Joaquim feedback):**

| Metric | Before Mysa | With Mysa | Source |
|--------|------------|-----------|--------|
| Time per claim (document processing) | 65-120 min | 10-15 min | FOS research + Caravela observation |
| Back-and-forth emails per claim | 3-5 rounds over days | 1 auto-generated, sent same day | Caravela + broker workflows |
| Documents manually opened per claim | 5-15 PDFs across systems | 0 — all parsed automatically | Caravela workflow |
| FNOL creation time | 20-30 min (manual entry) | 2-3 min (auto-filled, human reviews) | Caravela live |
| OCR extraction accuracy | N/A (manual) | 81.5% normalized match (Gemini 3 flash) | Caravela benchmark Feb 8 |
| Follow-up email drafting | 10-15 min per email | Auto-drafted, 1-click review | Built |
| SOP compliance | "Nobody reads the SOPs" — Joaquim | Step-by-step checklist, enforced per claim | Joaquim quote, Feb 10 |

**What we can project (reasonable estimates for sales conversations):**

| Metric | Estimate | How we get there |
|--------|----------|-----------------|
| Claims handled per person per day | 2-3x increase | Remove 70% of document processing time |
| Cost per claim reduction | 40-60% | Fewer hours per claim, fewer follow-up cycles |
| FNOL completeness at submission | 90%+ (vs ~60% today) | Gap analysis catches missing docs before submission |
| Average claim cycle time reduction | 30-50% | Faster document gathering = faster to decision |
| Annual savings for a 30K claims/year insurer | EUR 500K-750K | Based on FOS unit economics (EUR 15-25 saved per claim) |

**Quotes we can use (from real conversations):**

> "The things that are truly useful are where you need reports, technical assessments, multiple documents." — Joaquim, Crisur (8th largest insurer worldwide), Feb 10

> "I have no doubts that AI can be very important in our processes." — Joaquim, Feb 10

> "If you systematize the information and give the claims handler that information, that's fantastic." — Joaquim, Feb 10

> "Nobody reads the SOPs. Nobody knows the workflow. And when there is no SOP, that's fine — we reverse-engineer it from their historical claims." — Jeremy, Feb 11

**Impact framing for different buyers:**

For a **mid-market MGA (30K claims/year, EUR 100-200M GWP):**
> Your claims team processes 30,000 motor claims per year. Each one takes 65-120 minutes of document work. That's 32,500-60,000 person-hours per year on reading, copying, emailing, and writing — not deciding. At EUR 25/hour loaded cost, that's EUR 812K-1.5M/year spent on document processing alone. We cut that by 40-60%. Your EUR 100K/year license pays for itself in the first quarter.

For a **broker (4,000 claims/year, 10+ insurers):**
> Your team handles 4,000 claims across 10+ insurers. Each insurer has different document requirements. Your people memorize them or look them up every time. Mysa knows what each insurer needs. We cut your intake processing time by 60%+ and reduce back-and-forth with customers by 70%. That's 1-2 full-time employees worth of document work — automated.

For a **TPA / assistance company (100K+ claims/year):**
> You process 100K+ claims on behalf of insurers. Each claim starts with an email or call that your team manually reads and enters into a system. Mysa reads it for them. We give you an API: send the document, get structured data back. Your call center agents stop typing and start reviewing. At EUR 2-5 per claim, the math works at scale.

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
