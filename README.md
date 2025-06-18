# R-Basketball-Player-Points-with-Regression
Basketball Player Performance: Regression Analysis

Project Title: Predicting NBA Player Points Using Negative Binomial Regression

Course: STAT 4194 - Applied Regression Analysis

Author: Chenchenyi Zhu

Date: February 2025

📌 Overview
This project analyzes basketball player performance (2000-2001 season) using regression modeling to identify key factors influencing points scored (PTS). After testing Poisson and negative binomial approaches, a negative binomial regression model emerged as optimal due to overdispersion in the data.

🔗 Dataset: Basketball Players Stats (Kaggle)

🔍 Key Findings
🏆 Best Model
Model 1 (Negative Binomial):

Predictors: Stage + FGM + FGA + X3PM + FTM + TOV + draft_round

Metrics:

AIC = 4068.454 (lowest among candidates)

BIC = 4106.137

Interpretation: Points are significantly influenced by shooting efficiency (FGM, X3PM), turnovers (TOV), and draft status.

📊 Exploratory Insights
Strong Correlations:

Field goals (FGM, FGA) and 3-pointers (X3PM) show linear relationships with PTS.

Higher draft rounds correlate with lower points (potential undervaluation of late-round picks).

Overdispersion: Poisson models were rejected (dispersion ratios > 38, *p* < 2.2e-16).

🛠️ Methodology
Data Prep: Subset to 2000-2001 season; filtered 20+ predictors.

Visualization:

Scatterplots (PTS vs. FGM, TOV, etc.)
Diagnostic plots (residuals, QQ plots) for model validation.

Model Comparison:

Tested 4 negative binomial models; selected based on AIC/BIC.

🎯 Takeaways
Actionable Insight: Teams should prioritize player efficiency (e.g., FGM, FTM) over draft position.

Statistical Rigor: Negative binomial regression handles count-based, overdispersed data better than Poisson.

🔧 Tools Used
R Packages: glm.nb (negative binomial), ggplot2, AER (dispersion test)

Tags: #SportsAnalytics #Regression #NBA #R
