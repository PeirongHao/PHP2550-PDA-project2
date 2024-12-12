# PHP 2550 PDA Project2: Smoking Cessation Study in MDD Patients

## Summary
This project investigated the effectiveness of combined pharmacotherapy and psychotherapy interventions for smoking cessation among adults with Major Depressive Disorder (MDD). Data were analyzed from a 2×2 factorial randomized clinical trial involving 300 participants who received either varenicline or placebo in combination with either behavioral activation for smoking cessation (BASC) or standard behavioral treatment (ST). 

<div align="center">
  <img width="400" alt="logistic_model" src="https://github.com/user-attachments/assets/62c87cc4-c1c8-4b41-be78-f2ac3e47c1b1" />
</div>

The analysis revealed that the Fagerstrom Test for Nicotine Dependence (FTCD) score was negatively associated with smoking abstinence, as higher scores predicted lower odds of quitting. A strong positive interaction was observed between varenicline and nicotine metabolism ratio, indicating that varenicline was particularly effective for individuals with higher nicotine metabolic rates. Additionally, the interaction between varenicline and early morning smoking behavior showed a modest positive effect on abstinence. Behavioral activation therapy appeared less effective for individuals with current MDD compared to those with past MDD only, highlighting the importance of tailoring behavioral interventions to depressive status.

<div align="center">
  <img width="400" alt="auc" src="https://github.com/user-attachments/assets/c1e06a26-bcfc-46b1-8c74-a5a8915a5a55" />
</div>

To identify key predictors and control for overfitting, L0 and L1 regularization techniques were employed. The final model demonstrated moderate predictive performance, achieving an AUC of 0.764 for the derivation data and 0.712 for the validation data. In the derivation set, the model achieved a sensitivity of 83.6% and specificity of 63.2%, with an overall accuracy of 67.4%, while accuracy in the validation set reached 59.7%.

<div align="center">
  <img width="400" alt="calibration" src="https://github.com/user-attachments/assets/b31e14aa-cc39-4140-9edd-927e97cfc1df" />
</div>

These findings emphasize the effectiveness of pharmacotherapy with varenicline for smoking cessation in individuals with MDD and highlight the role of individual characteristics, such as nicotine metabolism and depressive status, in influencing treatment outcomes. While the predictive model performed moderately well, its results suggest that additional factors may contribute to smoking cessation success in this population. Future research could focus on identifying these factors and exploring further interaction effects to refine personalized smoking cessation strategies.

## Files
`project2.qmd`: This file includes R code and text explanations for both the Exploratory Data Analysis and Statistical Analysis.

`project2.pdf`: A PDF version of the report, including the Code Appendix at the end.

## Dependencies
I used the following packages for this analysis: tidyverse, knitr, tidyr, dplyr, kableExtra, readr, visdat, gridExtra, corrplot, fields, glue, mice, gtsummary, naniar, gt, L0Learn, and pROC.
