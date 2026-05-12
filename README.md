# Pstat100_final_project

## Dataset and Source
We will use two publicly available sources: Sean Lahman’s Baseball Database (lahman-baseball.com) for MLB career statistics, and Baseball Reference (baseball-reference.com) for NCAA Division I college stats and draft data. Records will be merged by player name and draft year. Data will be accessed via Sports Reference’s export tools or a pre-compiled Kaggle dataset. This is an observational dataset; conclusions apply to NCAA Division I drafted players only.

## Topic and Methodology
Can college baseball statistics predict a player’s MLB career performance? As a secondary angle, we will examine which franchises show the greatest draft efficiency.
Type of modeling: Supervised learning — regression and classification.
- Regression (primary): Predict career WAR/OPS+/ERA+ using multiple linear regression as a baseline, extended with Ridge and Lasso regularization to handle multicollinearity.
- Classification (secondary): Predict whether a player reaches the MLB at all using logistic regression, KNN, or a decision tree classifier.
- Model comparison: Cross-validated RMSE (regression) and AUC-ROC (classification).

## Required Steps
- Data problems: Merging across sources (name inconsistencies), structurally missing MLB stats for players who never reached the majors, duplicate multi-season college records, type correction, and restructuring to one row per player.
- Feature engineering: K:BB ratio, isolated power (ISO), WHIP.
- EDA: Distribution plots, correlation heatmap of college predictors vs. MLB outcomes, draft round scatter plots, team-level aggregations.

