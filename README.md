# Actuarial DCF Pricing & Fackler Reserve Engine for 15-Year Endowment Insurance 

## Project Overview
This project simulates an actuarial pricing and reserving engine for a 15-year Education Endowment product tailored for the Vietnam Middle-Income Market. The main objective is to measure the financial impact of the post-2022 Bancassurance crisis (characterized by high upfront agent commissions and massive early lapse rates).

## Tools & Technologies
*   **Core Actuarial Logic:** MS Excel (Cash Flow Projections, Fackler's Retrospective Method)
*   **Automation & Stress Testing:** Python (pandas, matplotlib, seaborn)
*   **Mortality Table:** CSO 1980 (Vietnam Ministry of Finance - Circular 156/2007)

## Key Actuarial Methodologies
1.  **Multiple Decrement Model:** Incorporated dynamic lapse rates alongside standard mortality.
2.  **Model Calibration:** Built a Python DCF engine to calculate the *Exact Net Annual Premium*, eliminating Actuarial Drift (rounding errors) found in Excel commutation functions.
3.  **Fackler's Reserve:** Successfully converged the prospective reserve to exactly 800,000,000 VND at maturity (Year 15).

## Stress Testing & Market Insights
I automated a scenario analysis (Interest Rate × Lapse Rate) and uncovered a critical pricing insight:
> **The "Liability Release" Effect:** In heavily savings-oriented products (like Endowments), early surrenders mathematically offset the high initial acquisition costs (80% Year-1 Commission). 

### Visualizations:
*Reserve Run-off Curve ensuring 800M maturity target:*
![Reserve Runoff](Reserve_Runoff.png)

*Premium impact of Bancassurance Lapse Crisis:*
![Lapse Stress Test](Lapse_StressTest.png)

---
*Created by Trinh Xuan Mai as a personal academic project.*
