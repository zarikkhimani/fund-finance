# Fund Finance

A lender-side ChatGPT skill for underwriting and analyzing fund finance and asset-based credit.

Coverage includes:
- NAV facilities
- Subscription facilities
- Private credit back leverage
- BDC financing
- Asset-based lending
- Hybrid / umbrella facilities
- Portfolio collateral, borrowing-base, covenant, cash-control, and stress analysis

## Repository structure

```text
fund-finance/
├── SKILL.md
├── references/
│   └── README.md
├── scripts/
│   └── README.md
└── assets/
    └── README.md
```

`SKILL.md` contains the core underwriting instructions and workflow. `references/` is for public or redacted source material. `scripts/` is for deterministic credit calculations and extraction utilities. `assets/` is for blank templates, schemas, diagrams, and reusable visuals.

## Credit philosophy

The skill is designed to answer the questions a lender actually cares about: what is the collateral, what cash repays the debt, how much value can deteriorate before protection breaks, what triggers action, and whether the lender can control and monetize the repayment source.

## Public-repository rule

Do not commit confidential borrower information, MNPI, proprietary bank materials, credentials, or unredacted internal documents. Use public, licensed, synthetic, blank, or properly redacted materials only.
