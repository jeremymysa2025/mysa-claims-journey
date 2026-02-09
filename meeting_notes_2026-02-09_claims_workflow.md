# Claims Workflow and Triage Process Optimization for Insurance Adjusters

*Meeting date: February 9, 2026*
*Source: [Granola recording](https://notes.granola.ai/t/bd0328cb-0d78-4c40-807e-27e27022db96-009c2hma)*

---

## Product Positioning & Market Focus

- Adjuster copilot and orchestrator that's proactive at every step
- Not just removing manual work — empowering decision making process
- Focus on Portugal initially, then expand (small market but specific opportunity)
- Target both insurance companies and brokers with different value propositions

## Claims Workflow Architecture

- Complete end-to-end process from intake to settlement
  - First contact → Triage → Investigation → Assessment → Decision → Settlement → Closure
- Each stage requires different workflows based on claim type (home vs auto vs property)
- SOPs (Standard Operating Procedures) feed into automated workflows
  - Insurance companies must share SOPs for TPA integration
  - SOPs become basis for AI agent decision trees
- Three workflow types needed:
  1. Always-deployed standard workflows
  2. Customized workflows from client SOPs
  3. New workflows clients want to setup

## First Contact & Intake Optimization

- Email-based claim creation with Chrome extension (like Superhuman)
- AI gap analysis cross-checks required fields against insurance requirements
- White-labeled FNOL (First Notice of Loss) forms for brokers
  - Reduces back-and-forth with customers
  - GDPR compliant with booking links for calls when needed
- Human must select email content parts — no fully automated parsing to avoid garbage data

## Triage Decision Logic & Automation

- **Standard thresholds:** 70-80% of car value triggers total loss flag, stops STP
- **Decision tree structure:**
  1. Catastrophe check → Route to CAT team
  2. Injury/fatality → High priority BI specialist
  3. Cost threshold → Manual review vs automated
  4. Fraud score → SIU investigation vs approval
- Coverage validation critical at this stage
  - Policy active status, insured item verification
  - Authority limits (approval thresholds per adjuster)
  - Reserve of rights letters protect insurers legally

## Technical Integration Requirements

- **Core systems:** Guidewire Policy Center, Duck Creek Policy, Salesforce
- **Assessment tools:** Colossus (BI evaluation), CCC (auto parts), local solutions (property)
- **Data sources:** Historical snapshots needed for policy validation at accident time
- **EU vs US differences:**
  - EU pays first then recovers, US denies then defends
  - Different legal frameworks require separate logic trees

## Competitive Landscape & Market Gaps

- **Major players:** Colossus (70% market share, 50+ years data), Shift Technology, Five Sigma
- **Opportunity areas:**
  - Property claims (no standardized assessment tools)
  - Small/medium insurers without enterprise systems
  - European market less penetrated than US
- **Data moat challenge:** Cannot compete with Colossus dataset, need different approach

## Knowledge Base & Agent Architecture

- Vault system containing all client data: SOPs, policies, state regulations, coverage details
- Chat interface for adjusters to query knowledge base contextually
- Agents operate within workflows with specific guardrails
- Performance tracking per agent type (fraud detection, document extraction, etc.)
- Pre-configured best practices built from historical client data
