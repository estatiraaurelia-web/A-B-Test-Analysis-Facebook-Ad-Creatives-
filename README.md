# A-B-Test-Analysis-Facebook-Ad-Creatives-
Author: Estatira Aurelia
Tools Used: Python (Pandas, NumPy, SciPy), Google Colab
Dataset: 200 rows of campaign performance data across two creative variants (A & B)

Overview
This project analyzes the performance of two ad creative variants (A and B) in a Holiday Jewelry campaign running across the U.S. and Canada.
The goal is to determine which creative drives better results based on:
Impressions
Clicks
Purchases
Revenue
CTR / CPC / CPM
Conversion Rate
CPA
ROAS

We performed:
✔ Data cleaning
✔ Metric calculations
✔ Group-level performance analysis
✔ A statistical t-test on conversion rates
This README summarizes the findings and concludes which variant should be scaled.

Project Structure
ab_test_creatives.csv — Raw dataset
ab_test_analysis.ipynb — Google Colab notebook with analysis code
README.md — Project documentation

Key Metrics Calculated
For each variant, we computed:
Engagement Metrics
CTR = clicks / impressions
CPC = spend / clicks
CPM = spend / (impressions / 1000)
Conversion Metrics
Conversion Rate = purchases / clicks
CPA = spend / purchases
Revenue Metrics
ROAS = revenue / spend

Final Results Table
variant	impressions	clicks	spend	purchases	revenue	CTR	CPC	CPM	conversion_rate	CPA	ROAS
A	878,108	23,510	15,266.67	1,448	99,088.00	2.68%	0.65	17.39	6.16%	10.54	6.49
B	836,972	22,949	14,721.77	1,386	96,805.98	2.74%	0.64	17.59	6.04%	10.62	6.58

Interpretation/Recomendationa
Engagement
Variant B had a slightly higher CTR (2.74% → better at grabbing attention)
CPC & CPM were nearly identical → no significant cost differences
Conversion & Revenue
Variant A had a slightly higher conversion rate (6.16%)
ROAS was nearly tied (A = 6.49, B = 6.58)
Costs
CPAs are virtually the same (A = $10.54 vs B = $10.62)

Statistical Testing
A t-test was performed comparing conversion rates of A vs B:
p-value > 0.05
✔ Result: No statistically significant difference
This means we cannot confidently claim one creative is better — both performed similarly.

Final Recommendation
Both creatives performed nearly identically.

However:
Variant B shows slightly stronger upper-funnel performance (better CTR)
Variant A shows slightly stronger lower-funnel performance (better conversion rate)

Recommended Action:
Continue running both variants, but:
Test new creative concepts to achieve a clearer winner
Consider segment-based testing (mobile vs desktop, US vs CA) for deeper insights
Use this A/B test as the baseline for a new iteration cycle
