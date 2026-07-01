# Actuarial Pricing & Reserving Engine — Endowment Insurance

## Overview
A Python + Excel actuarial model for pricing and reserving 
a 15-year Education Endowment insurance product for the 
Vietnamese market.

## Methodology
- **Pricing:** Discounted Cash Flow (DCF) with CSO 1980 
  mortality table (BTC Circular 156/2007)
- **Decrement:** Multiple decrement model — mortality + 
  lapse (25% yr-1 bancassurance) + 80% agent commission
- **Reserving:** Fackler's Retrospective Method — reserve 
  converges to exactly 800M VND at maturity
- **Validation:** Excel calibrated against Python DCF to 
  eliminate Actuarial Drift

## Key Findings
- Upfront 80% commission is primary profitability risk
- "Liability Release" effect: early surrenders partially 
  offset acquisition costs in savings products
- 200bp interest rate drop increases premium by ~18-22%

## Files
| File | Description |
|------|-------------|
| `Actuarial_Pricing_MaiTrinh.ipynb` | Python DCF engine + stress testing |
| `Actuarial_Pricing_MaiTrinh.xlsx` | Excel model + reserve projection |

## Data Source
CSO 1980 Mortality Table — Bộ Tài chính, 
Thông tư 156/2007/TT-BTC
