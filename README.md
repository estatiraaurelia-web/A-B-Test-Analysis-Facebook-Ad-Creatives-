# A-B-Test-Analysis-Facebook-Ad-Creatives-
A/B Test Analysis: Marketing Creative Performance
Author
Estatira Aurelia

Tools Used
Python (Pandas, NumPy, SciPy), Google Colab

Dataset
200 rows of campaign performance data comparing two creative variants (A and B).

Overview
This project analyzes the performance of two ad creative variants (A and B) in a Holiday Jewelry paid media campaign running across the United States and Canada.

The objective is to determine which creative performs better based on:
Impressions
Clicks
Purchases
Revenue
CTR (Click-Through Rate)
CPC (Cost per Click)
CPM (Cost per Mille)
Conversion Rate
CPA (Cost per Acquisition)
ROAS (Return on Ad Spend)

The notebook includes:
Data cleaning
Metric calculations
Group-level performance summary
A statistical t-test on conversion rates
This README summarizes the findings and conclusions.

Project Structure 
ab_test_creatives.csv      # Raw dataset
ab_test_analysis.ipynb     # Google Colab notebook with analysis code
README.md                  # Project documentation

Key Metrics Calculated
Engagement Metrics
CTR = clicks / impressions
CPC = spend / clicks
CPM = spend / (impressions / 1000)
Conversion Metrics
Conversion Rate = purchases / clicks
CPA = spend / purchases
Revenue Metrics
ROAS = revenue / spend

## Final Results Table

| Variant | Impressions | Clicks| Spend    | Purchases | Revenue   | CTR   | CPC  | CPM   | Conversion Rate | CPA   | ROAS |
|--------|-------------|--------|-----------|----------|-----------|-------|------|-------|-----------------|-------|------|
| A      | 878,108     | 23,510 | 15,266.67 | 1,448    | 99,088.00 | 2.68% | 0.65 | 17.39 | 6.16%           | 10.54 | 6.49 |
| B      | 836,972     | 22,949 | 14,721.77 | 1,386    | 96,805.98 | 2.74% | 0.64 | 17.59 | 6.04%           | 10.62 | 6.58 |

Interpretation and Recommendations
Engagement
Variant B showed a slightly higher CTR (2.74%), indicating stronger ability to capture initial attention.
Cost Efficiency
CPC and CPM were nearly identical between A and B, showing no significant cost differences.
CPA values were also nearly equal (A = 10.54 vs B = 10.62).
Conversion and Revenue
Variant A produced a slightly higher conversion rate (6.16%).
ROAS was nearly tied (A = 6.49, B = 6.58).
Overall, both creatives performed very similarly, with no major performance gaps.

Statistical Testing
A two-sample t-test was conducted to compare the conversion rates of Variant A and Variant B.
p-value > 0.05
Conclusion: There is no statistically significant difference between the conversion rates of the two creatives.
This means we cannot confidently declare a single winning creative. Performance differences are minimal and likely due to natural variation rather than true creative superiority.

Statistical Testing
A two-sample t-test was conducted to compare the conversion rates of Variant A and Variant B.
p-value > 0.05
Conclusion: There is no statistically significant difference between the conversion rates of the two creatives.
This means we cannot confidently declare a single winning creative. Performance differences are minimal and likely due to natural variation rather than true creative superiority.
