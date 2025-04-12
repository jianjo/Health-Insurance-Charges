# Health-Insurance-Charges

This project explores the factors influencing individual treatment costs and builds predictive models for the charges by health insurance using the R programming environment. The insights derived from this work can help insurance companies and policy planners to set more accurate premiums and design targeted interventions. 

**※** It was conducted collaboratively with my partner, Kelly Lee.  

### Project Objectives

- **Data Exploration:** Analyze a real-world dataset to identify key variables influencing healthcare costs.
- **Model Development:** Utilize regression techniques to predict insurance charges and determine the best fit of various models.
- **Insight Extraction:** Interpret the model results to understand the relative importance of features, finding significant predictors of higher costs.
- **Data Storytelling:** Present the findings through visualizations and clear code snippets to facilitate further exploration and adaptation by others.

## Methodology and Tools

- **Libraries**: lmtest, readr, ggplot2, faraway, lattice, caret, knitr, car, glmnet
- **Computational Language**: R 

## Results

**Simple Linear Regression**

- MSE: 36,680,455.99
- All predictors (age, BMI, smoker status, children) exhibited significant p-values, confirming their impact on insurance charges.

**Ridge Regression**

- MSE: 37,103,807.91
- R-squared of around 0.746 with an optimal lambda of ~953, indicating that regularization helped stabilize coefficient estimates, particularly in the presence of multicollinearity, though it resulted in a slightly higher MSE compared to the simple linear model.

**➡️ Influence of Smoking**: Smoking status remains the most influential variable, markedly increasing insurance charges.

**➡️ Age and BMI**: Both factors demonstrate positive correlations with charges, with older and higher BMI individuals tending to incur higher costs. 

**➡️ Model Sensitivity**: While the simple linear model performed marginally better in terms of MSE, the Ridge model’s robustness to outliers and multicollinearity is advantageous for datasets with high variance. 

⇒ Depending on the analysis needs (simplicity vs. robustness), practitioners can choose between a straightforward linear regression and a regularized approach, Ridge regression. 

## Conclusion

This project not only deepens our understanding of the dynamics behind health insurance costs but also serves as a practical demonstration of applying data science techniques—from data cleaning to model evaluation—in a real-world context. The methodologies and insights presented here are adaptable to insurance companies in policy formulation and pricing strategies while also informing broader healthcare economics strategies.
