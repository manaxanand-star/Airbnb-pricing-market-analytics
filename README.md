# Airbnb Pricing & Market Analytics

A comparative marketing analytics project analysing Airbnb pricing patterns
across Rio de Janeiro, Brazil and Los Angeles County, USA.

## Project Overview

This project investigates which observable listing characteristics are
associated with Airbnb prices and whether these relationships transfer
across two structurally different markets.

The analysis uses cleaned and currency-harmonised Airbnb listings data from
Rio de Janeiro and Los Angeles County.

## Key Questions

- Which market has the higher typical listing price?
- How strongly does room type affect price?
- Does the room-type premium remain after controlling for neighbourhood?
- How does review activity relate to price?
- Does host portfolio scale relate to pricing?
- Which pricing relationships generalise across markets?

## Dataset

After cleaning:

- **Rio de Janeiro:** 35,376 listings
- **Los Angeles County:** 32,736 listings
- **Total:** 68,112 listings

Rio prices were converted from BRL to USD using a rate of 5.15 BRL/USD
to enable a consistent cross-market comparison.

## Methodology

The analysis follows a descriptive-to-inferential approach:

1. Data cleaning and outlier treatment
2. Currency harmonisation
3. Descriptive statistics
4. Room-type ANOVA
5. Correlation analysis
6. Log-price OLS regression
7. Neighbourhood-controlled regression
8. Host portfolio segmentation
9. Pooled cross-market interaction model
10. Managerial recommendation analysis

### Tools

- Python
- Pandas
- NumPy
- SciPy
- Statsmodels
- Matplotlib

## Key Findings

### 1. Los Angeles is the higher-priced market

After converting Rio prices to USD:

- Rio mean price: **~$120**
- Los Angeles County mean price: **~$177**

Los Angeles County is therefore approximately **47% more expensive**
on average.

### 2. Room type is the strongest pricing signal

Entire-home listings showed a substantial premium over private rooms:

| Market | Entire-home premium |
|---|---:|
| Rio de Janeiro | +147.1% |
| Los Angeles County | +145.7% |

The relationship remained strong after controlling for neighbourhood.

### 3. Cross-market pricing patterns

A pooled interaction model was used to distinguish relationships that
genuinely transfer across markets from those that require
market-specific calibration.

The entire-home premium was statistically consistent across the two
markets, while hotel/shared-room and review-related effects differed
across markets.

## Managerial Implications

The analysis suggests that:

- **Room type** should be the primary segmentation variable for
  cross-market benchmarking.
- **Neighbourhood** should be used as a secondary local benchmark.
- Review-based pricing signals should be **market calibrated**.
- Host portfolio scale should be treated primarily as an **operational**
  indicator rather than a direct pricing strategy.

## Project Report

The complete academic report is available in:

`report/Airbnb_Pricing_Market_Analytics_Report.pdf`

## Academic Context

**Course:** MS 491 – Marketing Analytics  
**Institution:** Indian Institute of Technology Gandhinagar  
**Project:** Group 13  
**Submission:** September 2026

## Authors

- Aman Bola
- Manax Anand
- Piyush Jain
- Rhythem Soni
- Rohit Kumar Meena
