# FTTH Site Progress Analysis

Python and Pandas analysis of simulated FTTH site data: ATP pass rates, defect types, and build time vs site size.

**Note:** All data is simulated. No real client or employer data is used.

## Problem
Fibre rollout teams need to know where sites fail acceptance testing (ATP) and why, so they can cut rework and delays.

## Data
`sites.csv`: 55 simulated FTTH sites with poles, cable length, team size, dates, ATP result, defect type and optical loss (dB). It includes missing values, duplicates and inconsistent labels to practise cleaning.

## Method
1. Cleaned the data with Pandas (duplicates, missing values, label formats).
2. Calculated days to complete per site.
3. Charted pass rate by area, defect types, build time vs site size, and loss distribution.

## Findings
1. In this simulated dataset, Lekki had the lowest first-time ATP pass rate (50.0%, 8 sites). Yaba had the highest among areas with 5 or more sites (88.9%, 9 sites). The overall pass rate was 70.9%.
2. Cable sag was the most common defect found at ATP.
3. Larger sites took longer to complete (correlation of 0.65 between poles per site and days to complete).

Note: Areas have between 3 and 11 sites each, so area pass rates are indicative only.

## Tools
Python, Pandas, Matplotlib, Google Colab

