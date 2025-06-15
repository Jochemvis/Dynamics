# Causal Effects of Parental Gifts on Family Relationships
In this project, we examined whether receiving valuable items or money from biological parents influences the quality of family relationships among young adults aged 16–40. Using four waves of panel data from the Dutch LISS dataset (2020–2023), we estimated the Average Causal Effect (ACE) of repeated parental gifting on self-reported relationship satisfaction, measured on a 1–5 scale.

To approximate a causal relationship, we applied Inverse Probability Weighting (IPW), using both logistic regression and random forest models to estimate propensity scores. We cleaned and merged the data across all four time points, restricted the sample to individuals with living biological parents throughout the period, and removed implausible or missing responses.

The analysis showed that those who received gifts in both 2021 and 2022 reported slightly higher family relationship quality in 2023. However, the effect was small (approximately 0.15 points on a 5-point scale) and somewhat sensitive to assumptions. Notably, the positivity assumption was partly violated, and balance (SMD) was not fully achieved across all covariates—though logistic regression outperformed random forest in this regard.

While both methods yielded similar conclusions, the logistic regression-based model was preferred due to better covariate balance and interpretability. Overall, the results suggest a modest but statistically significant positive association between receiving valuable items from parents and the perceived quality of family relationships.

The repository contains code for data cleaning, merging, IPW estimation, model fitting, and diagnostic plots to assess assumptions and balance.
