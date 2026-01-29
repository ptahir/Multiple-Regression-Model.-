# Multiple-Regression-Model.-
A Python project demonstrating multiple regression modelling. 

This project analyzes how R&D Spend, Administration, Marketing Spend, and State of Operation impact Profit using Multiple Linear Regression. It includes model training, evaluation, visualization, and business insights into which features most influence profit and how well the model predicts outcomes.

The dataset used in this project: 50_Startups.csv

Project Objectives

• Build a Multiple Linear Regression model 


• Evaluate the model using:


– Coefficients → Feature impact indicators

– R² Score → Model explanatory power

– Mean Squared Error (MSE) → Prediction accuracy


• Visualize model performance using scatter plots


• Identify which company is likely to earn the highest profit


• Predict future profit values for hypothetical inputs

Dataset Description

The dataset contains business data for 50 startups, including expenditures in different areas and corresponding company profits. 

Feature	Description

• R&D: Money spent on research and development
• Administration: Administrative expenses
• Marketing: Marketing expenses
• State: U.S. state in which the company operates
• Profit:	Annual profit

Technologies Used


• Python • Pandas • NumPy • Scikit-learn • Matplotlib • Seaborn

Methodology


1. Load and inspect the dataset
2. Handle categorical data (State → dummy variables)
3. Train/test split (80/20)
4. Train a Multiple Linear Regression model
5. Compute coefficients, R² score, and MSE
6. Visualize actual vs. predicted profit
7. Identify which company the model predicts will have the highest profit
8. Predict profit for new example data

Model Results: 

Feature Coefficients

The coefficients show how much expected profit changes with a one-unit increase in each feature, holding other variables constant:

• Positive coefficient → Feature increases predicted profit
• Negative coefficient → Feature decreases predicted profit
• Larger absolute value → Stronger influence

For example (hypothetical values):

R&D Spend → 0.805630 Strong Positive impact

Marketing Spend →  0.029855 Moderate positive impact

Administration → -0.068788 Weak or negative impact

State dummies → Indicates state-specific effects

Interpretation of State Coefficients

• State_Florida (≈ 938.8): Being in Florida is associated with about $939 higher predicted profit compared to California (reference), holding other factors constant.

• State_New York (≈ 7.0): Being in New York is associated with only $7 higher predicted profit versus California, after accounting for other features.

These values show how location affects predicted profit relative to the baseline state.

Interpretation of Intercept

• Intercept (~54,028):
This is the model’s baseline predicted profit when all input features (spending and state) are zero — essentially the starting value before other factors contribute.

📌 Interpretation of Model Performance

• R² Score (~0.90):
The model explains about 90% of the variation in profit — meaning the input features (R&D, Administration, Marketing, State) collectively do a very good job predicting profit.

• Mean Squared Error (~82,010,363):
On average, the squared difference between actual and predicted profits is ~82 million. Although this number seems large due to the scale of profit values, lower MSE still indicates closer predictions to actual values.

Actual vs Predicted Plot 
<p align="center">
  <img src="https://github.com/ptahir/Simple-Linear-Regression.-/blob/main/actualvspredicted.png" width="1000">
</p>
