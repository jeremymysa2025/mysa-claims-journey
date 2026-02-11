# Mysa

## What we do
We automate the document work in insurance claims. When a claim comes in, people spend hours reading PDFs, checking policies, emailing customers for missing documents, and writing reports. We do all of that. The human just makes the decision at the end.

## The problem
A single insurance claim touches 5-10 people and 20+ documents. Before anyone decides anything, someone has to:
- Open every PDF and email, find the relevant fields
- Check if all required documents are there (they usually aren't)
- Email the customer back, wait days, follow up again
- Cross-reference the policy to check coverage
- Write the FNOL report, the investigation summary, the settlement letter

This takes 65-120 minutes per claim. 70% of it is gathering and typing, not thinking. Multiply that by 30,000 claims a year for a mid-market insurer — that's 50,000+ person-hours of document processing annually.

The existing software (Guidewire, Duck Creek) stores the data. Nobody processes it.

## What Mysa does — specifically
1. **Reads every document** — PDFs, emails, photos, handwritten forms. Extracts the fields into structured data.
2. **Checks what's missing** — Compares extracted data against what the workflow requires. Returns a list of gaps.
3. **Sends the follow-up** — Drafts the email to the customer requesting missing documents. Human reviews, clicks send (or auto-sends).
4. **Writes the reports** — Generates the FNOL, the investigation summary, the contestation letter — from data already extracted.
5. **Enforces procedures** — Turns each insurer's SOPs into step-by-step checklists. Every person touching a claim sees what to do next and gets notified when it's their turn.

65-120 minutes → 10-15 minutes per claim.

## How we deploy
We don't sell software and walk away. We sit with the insurer for 2 months. We study their historical claims. We read their SOPs. We configure workflows specific to their processes. Then we go live.

This is hard to replicate. Every insurer has different procedures. Once we've encoded them, switching costs are high.

## Who buys it
**Primary:** Mid-market insurers and MGAs in Europe (EUR 100-200M GWP, 10K-60K claims/year). Big enough to have real volume, small enough that they don't have in-house AI teams.

**Secondary:** Insurance brokers managing claims across multiple insurers. They need to know what each insurer requires and chase documents accordingly.

**Later:** TPAs and assistance companies processing high-volume claims on behalf of insurers (100K+ claims/year). They buy the document parsing as an API.

## Where we are
- **Live** with a mid-size MGA in Portugal for motor claims (Caravela)
- **Forward deployment scheduled** with the 8th largest insurer worldwide (Crisur/Ageas) — they invited us to spend a day at their Porto office to configure the product around their workflows
- **Broker pipeline** in Southern Europe
- **Building for US** — motor first, then property

## Market
80-95 million motor and property claims per year across EU and US. ~$1.5 trillion in combined premiums.

Mid-market carriers (our target segment) handle 30-60K claims/year each. There are hundreds of them in Europe alone.

## Business model
- **Per-claim:** EUR 2-8/claim (entry pricing for brokers and TPAs)
- **Platform license:** EUR 10K-2M/year (for insurers, scaled to volume)
- At a 30K claims/year insurer, a EUR 100K/year license saves EUR 500-750K in document processing costs. Payback in one quarter.

## Competition
Nobody does what we do across the full claim.

| Company | What they do | Where they stop |
|---------|-------------|-----------------|
| Pace.ai | FNOL extraction | Just intake. No workflows, no follow-up, no reports. |
| Further AI | Underwriting doc processing | Different part of insurance. We do claims. |
| Five Sigma / Shift | Claims automation for Tier 1 | Need 100K+ claims. We sell to mid-market. |
| Guidewire / Duck Creek | Claims database (CRM) | Stores data. Doesn't process documents. |
| CCC / Mitchell | Auto damage estimation | 50-year data moat on parts pricing. We do everything around the estimate. |

## Why now
- OCR and document parsing hit production-grade accuracy in 2025 (we run at 81.5% normalized match on claims documents)
- 25% of adjusters in the US retire within 5 years — the workforce is shrinking
- Mid-market insurers are being squeezed: rising claim volumes, fewer people, same manual processes
- The big vendors (Guidewire, CCC) don't serve the mid-market well — too expensive, too slow to deploy

## The team
Jeremy Blehaut and Tiago Brigido. Insurance domain + AI product experience. Based in Europe, building for global.

## What we're raising for
- Engineering: document parsing depth (images, voice, multi-language), CMS connectors (Guidewire API integration), phone/call recording for US market
- Go-to-market: forward deployments with 3-5 insurers in Southern Europe, first US conversations
- First US hire (sales/partnerships)

---

*Live in Europe. Building for the US. Automating the 70% of claims work that isn't decisions.*
