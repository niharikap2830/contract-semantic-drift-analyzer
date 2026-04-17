# Contract Semantic Drift Analyzer (CSDA)

**A novel legal analytics framework for detecting hidden rights erosion in contract revisions.**

> Invented by Niharika Pandey — First conceived and documented: April 16, 2026.  
> © 2026 Niharika Pandey. All rights reserved.

---

## The Problem Nobody Was Measuring

When contracts get redrafted across negotiation rounds, lawyers review each change individually. A single word swap — "shall" to "may", "thirty days" to "reasonable time", "entitled to" to "eligible for consideration" — looks minor in isolation.

But cumulatively? Those changes can silently strip a party of every meaningful protection in the agreement. No single change triggers an alarm. The damage is invisible until it's too late.

**No existing tool measured this. Until now.**

---

## What This Is

The Contract Semantic Drift Analyzer (CSDA) is an interactive legal analytics tool that accepts two versions of a contract clause and quantifies exactly how much legal protection has been lost between them — using a novel scoring method called **Clause Semantic Entropy Scoring (CSES)**.

It produces:

- A **CSES composite score** from 0–100 (0 = no drift, 100 = complete rights erosion)
- A **severity classification** (Critical / High / Medium / Low)
- **Six dimension scores** measuring distinct axes of semantic erosion
- **Individual findings** with specific language changes and their legal consequences
- **Drift token pairs** — word-level changes mapped to their legal impact
- A **Power-Shift Directional Metric** showing which party gained from the changes
- A **radar chart** visualizing all six dimensions simultaneously

---

## The Core Innovation: Clause Semantic Entropy Scoring (CSES)

CSES is the original measurement framework at the heart of this invention. It defines six independent dimensions of legal language erosion and aggregates them into a single composite score.

### The Six Dimensions

**1. Obligation Weakening**  
Measures erosion of mandatory language into discretionary language.  
*Examples: "shall" → "may", "must" → "should", "is required to" → "is encouraged to"*  
Each substitution converts an enforceable obligation into a non-binding preference.

**2. Temporal Precision Erosion**  
Measures replacement of specific timeframes with vague standards.  
*Examples: "thirty (30) days" → "reasonable time", "within 48 hours" → "promptly"*  
Specific timeframes create clear breach thresholds. Vague standards make breach nearly impossible to prove.

**3. Quantifier Drift**  
Measures substitution of precise numerical commitments with qualitative hedges.  
*Examples: "three (3) months salary" → "reasonable severance consideration", "100% of costs" → "a portion of applicable costs"*  
Directly reduces the measurable value of contractual entitlements.

**4. Discretion Transfer**  
Measures the shift of decision-making authority toward the counterparty.  
*Examples: "as mutually agreed" → "as determined by the Company", "subject to arbitration" → "subject to Company policy"*  
Captures power imbalance quietly introduced through language changes.

**5. Remedy Dilution**  
Measures weakening or removal of enforcement mechanisms and legal remedies.  
*Examples: removal of injunctive relief provisions, "entitled to" → "may seek", attorney's fee-shifting language removed*  
Makes rights practically unenforceable even when they nominally remain.

**6. Scope Narrowing**  
Measures reduction in the breadth of coverage or applicability of protective clauses.  
*Examples: narrowing of defined terms, addition of carve-outs, reduction of covered persons*  
Can eliminate protection entirely while appearing superficially minor.

---

## The Power-Shift Directional Metric

A signed integer from **-100 to +100** that answers: *in whose favor did these changes operate?*

- **Positive score** → power shifted toward the counterparty (Company, Licensor, Client)
- **Negative score** → power shifted toward the protected party
- **Zero** → neutral or balanced drift

This metric is novel because it introduces **directionality** into semantic drift analysis. Existing text comparison tools measure difference — they do not identify which party benefits from each change, nor aggregate those benefits into a single directional score.

---

## Why This Is Novel

To the best of the inventor's knowledge as of April 16, 2026, no prior system, method, tool, or publication has:

- (a) Defined and applied these six specific dimensions as a unified framework for measuring legal rights erosion in contract revisions
- (b) Produced a composite CSES score from 0–100 representing total protection loss
- (c) Applied a Power-Shift Directional Metric to identify which contracting party benefits from cumulative language changes
- (d) Identified and classified individual "drift tokens" — paired word/phrase substitutions mapped to specific legal impact
- (e) Combined all of the above into a single automated analysis system for legal clause comparison

Existing tools (Microsoft Word Track Changes, DocuSign CLM, Ironclad, Kira, Luminance) detect **textual differences** but do not interpret their legal significance, quantify rights erosion, measure directional power shift, or produce a composite semantic entropy score.

---

## Supported Clause Types

- Employment contracts
- NDA / Confidentiality agreements
- Services agreements
- IP / Licensing agreements
- Indemnification clauses
- Limitation of liability clauses
- General commercial contracts

---

## How It Works

1. User pastes Version A (original clause) and Version B (revised clause)
2. User selects the clause type
3. The CSES engine analyzes the text across all six dimensions
4. Results are returned with composite score, dimension breakdown, findings, drift tokens, and power-shift metric
5. User can export results or generate a negotiation strategy to restore eroded protections

---

## Use Cases

- **In-house legal teams** reviewing vendor contract redlines for cumulative erosion
- **Employment lawyers** protecting employees through repeated offer letter negotiations
- **M&A due diligence** scanning stacks of contracts for systematic rights erosion patterns
- **Contract managers** establishing a baseline score and tracking drift across versions over time
- **Individuals** reviewing any contract before signing

---

## Intellectual Property Notice

The Contract Semantic Drift Analyzer, the Clause Semantic Entropy Scoring (CSES) method, the six-dimension erosion framework, the Power-Shift Directional Metric, and the drift token identification methodology are original inventions conceived by **Niharika Pandey** on April 16, 2026.

This repository is published as a **defensive publication** to establish prior art and prevent any third party from obtaining patent rights over this method or any substantially similar method.

© 2026 Niharika Pandey. All rights reserved. This software and methodology may not be reproduced, distributed, or used as the basis of a commercial product without explicit written permission from the inventor.

---

## Contact

**Inventor:** Niharika Pandey  
**Email:** niharikap.jbp@gmail.com  
**GitHub:** [niharikap2830](https://github.com/niharikap2830)  
**Date of first publication:** April 16, 2026

---

*This README constitutes a public disclosure of the invention for the purposes of establishing prior art under 35 U.S.C. § 102 and equivalent statutes internationally. Publication date: April 16, 2026.*
