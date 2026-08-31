---
name: fund-finance
description: Analyze fund finance, NAV, private credit back leverage, and asset-based lending transactions. Use for underwriting, borrowing-base analysis, collateral eligibility, leverage and coverage calculations, covenant review, cash sweeps, waterfalls, credit agreement terms, portfolio stress tests, and lender-focused credit analysis.
---

# Fund Finance / ABL

## Purpose

Act as a lender-side underwriting and structuring skill for fund finance and asset-based credit.

Primary coverage:
- NAV facilities
- Subscription facilities
- Private credit back leverage
- BDC leverage and financing
- Asset-based lending
- Hybrid and umbrella facilities
- Portfolio-level collateral analysis

Focus on repayment, collateral value, structural protections, liquidity, downside behavior, and lender recovery.

## Core Rules

1. Preserve exact borrower, sponsor, lender, creditor, fund, portfolio company, covenant, ratio, and facility names when provided.
2. Preserve exact numerical figures extracted from source material. Do not silently round or substitute values.
3. Separate facts from assumptions and derived calculations.
4. Never invent missing credit agreement terms, collateral values, eligibility criteria, advance rates, concentration limits, cure rights, or covenant thresholds.
5. State the period and valuation date for every material financial or portfolio figure when known.
6. Trace repayment to the actual cash source, not merely to accounting value.
7. Analyze both asset-level and structure-level risk.
8. When documents conflict, identify the conflict and prioritize executed transaction documents over summaries or marketing materials.
9. For public repositories, do not add confidential, MNPI, proprietary, or unredacted borrower materials.

## Underwriting Workflow

### 1. Identify the transaction

Determine:
- Borrower and guarantors
- Sponsor / manager
- Facility type
- Commitment and funded amount
- Currency
- Tenor and maturity
- Pricing and fees
- Collateral package
- Recourse structure
- Purpose / use of proceeds
- Primary and secondary repayment sources

### 2. Map the legal and structural chain

Build the ownership and cash-flow path:

`Investors -> Fund / Borrower -> HoldCo / SPV -> Portfolio Assets -> Cash Proceeds -> Controlled Account -> Lender`

Identify:
- Pledged equity
- Pledged bank or securities accounts
- Distribution accounts
- Security interests
- Control agreements
- Intercreditor arrangements
- Structural seniority / subordination
- Restricted subsidiaries or excluded entities
- Leakage paths

### 3. Build the collateral base

For each asset, capture when available:
- Asset / company / fund name
- Strategy / sector
- Investment type
- Cost
- Fair value / NAV
- Eligible NAV
- Concentration-adjusted NAV
- Eligibility status and reason
- Ownership percentage
- Look-through debt
- EBITDA or relevant cash-flow metric
- Leverage
- Governance / control rights
- Distribution history
- Maturity
- Sponsor valuation marks
- Third-party valuation support
- Pledge / consent status

### 4. Calculate core credit metrics

Use the definitions in the governing documents first. If no contractual definition is available, label the calculation as analytical.

Common calculations:

`LTV = Debt / Eligible NAV`

`Net LTV = Net Debt / Eligible NAV`

`Advance Rate = Borrowing Base Credit / Eligible Collateral Value`

`Availability = Borrowing Base - Loans Outstanding - applicable reserves / deductions`

`DSCR = Eligible Cash Flow / Debt Service`

`Interest Coverage = Eligible Earnings or Cash Flow / Cash Interest`

`Asset Coverage = Total Assets / Debt`, subject to the applicable statutory or contractual definition.

For ABL:

`Borrowing Base = Eligible A/R x A/R Advance Rate + Eligible Inventory x Inventory Advance Rate + other eligible collateral - Reserves`

`Excess Availability = Borrowing Base - Revolver Usage - Letters of Credit - other applicable usage`

If calculating a weighted-average advance rate:

`WAAR = Sum(Eligible Collateral Value x Advance Rate) / Sum(Eligible Collateral Value)`

### 5. Review eligibility and concentrations

Test:
- Single-name limits
- Top-N limits
- Industry limits
- Geography limits
- Sponsor / manager limits
- Asset type limits
- Non-performing or impaired asset exclusions
- Delinquency / default exclusions
- Minimum equity value
- Minimum ownership
- Minimum reporting / valuation requirements
- Currency limits
- Unfunded commitment treatment
- Look-through leverage caps

Show gross NAV, eligible NAV, and concentration-adjusted NAV separately.

### 6. Review covenants and triggers

Extract exact:
- Maximum LTV
- Minimum NAV
- Minimum liquidity
- Minimum DSCR / FCCR / interest coverage
- Asset coverage tests
- Borrowing-base deficiency mechanics
- Cash sweep triggers
- Cash dominion
- Distribution blockers
- Mandatory prepayments
- Cure rights and cure periods
- Margin step-ups
- Events of default
- Key-person / manager events
- Valuation dispute rights
- Lender consent rights

For every trigger, explain what happens operationally when it is breached.

### 7. Stress the collateral

At minimum consider:
- Uniform NAV decline
- Top asset loss
- Top 3 / top 5 asset decline
- Concentration-limit compression
- Ineligibility of major assets
- Distribution slowdown
- Higher interest expense
- Delayed exits
- Lower recovery values
- FX moves where relevant
- Portfolio company leverage increase

Show the path from stress -> eligible collateral -> borrowing base / covenant -> liquidity requirement -> lender repayment or recovery.

### 8. Evaluate liquidity and cash control

Determine:
- Where cash is generated
- Whether distributions are required to enter controlled accounts
- Whether cash can be diverted before reaching lender-controlled accounts
- Sweep percentage
- Release conditions
- Distribution permissions
- Waterfall priority
- Required reserves
- Ability to redraw after prepayment

Do not treat a cash sweep and cash dominion as interchangeable. Describe the actual mechanics in the documents.

## Credit Agreement Review

When reviewing transaction documents, organize findings as:

| Topic | Exact Term | Credit Impact |
|---|---|---|
| Commitment |  |  |
| Maturity |  |  |
| Pricing |  |  |
| Collateral |  |  |
| Eligibility |  |  |
| Advance Rate |  |  |
| Concentration Limits |  |  |
| LTV / Coverage |  |  |
| Cash Sweep |  |  |
| Cash Dominion |  |  |
| Mandatory Prepayment |  |  |
| Cure Rights |  |  |
| Distribution Restrictions |  |  |
| Events of Default |  |  |

Quote only the minimum text required to preserve legal meaning, then explain it in plain English.

## Credit Output

For a full underwriting response, prioritize:

1. Transaction snapshot
2. Sources of repayment
3. Collateral and borrowing base
4. Leverage / coverage
5. Portfolio concentrations
6. Structural protections
7. Liquidity and cash control
8. Covenants / triggers
9. Stress cases
10. Key risks and mitigants
11. Missing diligence
12. Credit conclusion

Keep the analysis lender-focused. Do not confuse strong asset quality with strong lender protection if the collateral cannot be reached, controlled, or monetized.

## References, Scripts, and Assets

- `references/`: public or redacted underwriting guides, definitions, market references, and deal-document excerpts.
- `scripts/`: deterministic calculations, extraction utilities, stress tests, and borrowing-base tools.
- `assets/`: reusable templates, diagrams, blank models, schemas, and presentation assets.

Read relevant files from these directories before performing specialized work when they exist.
