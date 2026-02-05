# Applied Sampling Mini-Project: EV Adoption Survey

**Course:** Applied Sampling (Honours)  
**Institution:** University of the Witwatersrand  
**Year:** 2025  
**Result:** Top-performing submission

## Project Overview

This mini-project estimates electric vehicle (EV) adoption intentions among urban residents using stratified sampling techniques. The study simulates a survey of 10,000 Green City residents, stratified by age (18-34, 35-54, 55+), to achieve a margin of error ≤ 0.05 with improved efficiency over simple random sampling.

## Key Techniques

- Stratified random sampling with cost-constrained allocation
- Post-stratification adjustment for missing-at-random (MAR) nonresponse
- Bayesian estimation using binomial logit models
- Monte Carlo simulation (200 replications) for performance evaluation
- Power analysis for subgroup difference detection

## Key Findings

- **Design-adjusted estimate:** 0.4024 (SE = 0.0234, 95% CI: 0.3574–0.4490)
- **True population proportion:** 0.3891
- **Relative efficiency:** 1.2375 (23.75% variance reduction over SRS)
- **Precision target:** Achieved (MOE = 0.0453 ≤ 0.05)

## Demographic Insights

EV adoption varies significantly by:
- **Age:** 62.25% (18-34) vs 11.48% (55+)
- **Income:** 28.84% (Very Low) vs 67.78% (Very High)

## Tools Used

- R (sampling, survey, rstanarm packages)
- Quarto/R Markdown for report generation

## Note

This is academic coursework submitted for Wits Honours in Mathematical Statistics. The Green City population is simulated for educational purposes.
