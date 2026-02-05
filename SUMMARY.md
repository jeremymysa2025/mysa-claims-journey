# Mysa Claims Journey Discovery — Summary for Co-founders

### What We Did
Deep product discovery mapping the complete insurance claims journey for **Motor** and **Home/Property** insurance. Not surface-level — we went phase by phase, researching how things actually work, challenging assumptions, and identifying where automation opportunities exist.

**Output:**
- 2000+ line discovery document with detailed journey mapping
- Interactive service blueprint visualization (React app)
- 46 tracked assumptions
- 20 strategic insights
- GitHub repo: https://github.com/tiago-brigido/mysa-claims-journey

---

## Key Discovery #1: The STP Reality Gap (Motor)

**The conventional wisdom is wrong.**

Everyone says EU convention systems (IRSA, CIMPAS, CID) auto-resolve 60-70% of motor claims. We dug deeper:

- **Theoretical STP:** 60-70% of claims *could* auto-resolve
- **Actual STP:** Only ~10% achieve straight-through processing
- **The gap:** 50+ percentage points

**Why?** The convention lookup is trivial — it's just a database query matching checkboxes to fault percentages. **The bottleneck is data quality:**
- ~50% of EAS forms are still paper
- Filled out by stressed people with shaking hands
- Messy diagrams, unclear checkboxes, missing fields

**The opportunity:** Whoever fixes data quality upstream unlocks the 50+ point STP gap. The convention system isn't the problem — garbage data going IN is the problem.

---

## Key Discovery #2: EU vs US Are Fundamentally Different

| | **EU** | **US** |
|---|---|---|
| **Documentation** | EAS — single agreed document signed by both | Competing narratives, no joint document |
| **Fault determination** | Convention lookup tables | Human investigation every time |
| **FNOL** | "Here's my EAS" (verification) | "Let me tell you what happened" (data collection) |
| **Adjuster involvement** | Often NO for clean claims | Almost ALWAYS — even for fender benders |

**Implication:** Different automation opportunities. EU = fix data quality to unlock STP. US = reduce adjuster time on the 4 recorded statements per claim.

---

## Key Discovery #3: Home Claims Are Structurally Different

| | **Motor** | **Home** |
|---|---|---|
| Counterparty? | YES | Usually NO |
| Agreed document? | EAS | NONE |
| Question to answer | WHO caused it? | WAS it covered? |
| STP possible? | ~10% (EU) | Very rare |
| Adjuster? | Often skipped (EU) | Almost always needed |

**Unlike motor, EU has no structural advantage for home claims.** No EAS, no convention system.

**The opportunity is different:** Not "unlock STP" but "make adjusters 3x more productive."
- Field adjusters spend ~25-30% of time on travel alone
- Virtual inspection is growing (40% now, trending to 60%)
- TPAs (Crawford, Sedgwick, Engle Martin) employ 25-35% of adjusters — massive buyer segment

---

## Key Discovery #4: AI Replacing Adjusters Is Overhyped (For Home)

**What AI can do:** Detect visible damage, measure from photos, process documents, flag fraud patterns

**What AI cannot do:**
- See hidden damage (water behind walls, mold, structural)
- Determine causation ("sudden burst" vs "gradual leak" — coverage depends on this)
- Handle complex coverage interpretation
- Current accuracy ~70%, needs >95% for high-risk automation

**The fraud problem:** AI is making fraud EASIER — fake photos, fabricated receipts, AI-generated documents. Adversarial dynamic matters.

**Realistic opportunity:** Augment adjusters (3x productivity), not replace them.

---

## Strategic Implications for Mysa

1. **The STP gap is the motor opportunity** — Fix data quality upstream (better EAS capture, structured intake) and you unlock massive value

2. **Broker-to-insurer submission is a wedge** — All paths (portal, email, phone) have friction. Data normalization layer that works for both sides.

3. **Home = different product** — Not about STP, about adjuster productivity. TPAs are the buyer.

4. **EU-first makes sense for motor** — Structural data advantage (EAS). But for home, EU has no advantage.

5. **Don't over-index on "AI replaces humans"** — For motor maybe (data quality problem). For home, hidden damage and fraud risk mean humans stay in the loop.

---

## What's Mapped

**Motor (phases 0-6 complete):**
- Incident → Scene Management → Documentation → Reconciliation → First Contact → FNOL → Triage
- 6 decision forks with branching logic
- EU vs US differences at every phase

**Home:**
- FNOL process
- Adjuster workflow (desk vs field)
- TPA landscape
- 3x productivity opportunity

**Not yet mapped:**
- Motor phases 7-11 (Investigation → Settlement → Close)
- Repair networks, subrogation, fraud workflows

---

## Next Steps

1. Continue mapping motor phases 7-11 (where investigation and assessment happen)
2. Go deeper on repair networks / direct repair programs
3. Validate STP assumptions with actual insurer data
4. Decide: upstream data quality or downstream adjuster tools? Or sequence them?

---

*Full details in the GitHub repo. The README has instructions for continuing the research.*
