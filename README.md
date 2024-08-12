# 🏬 Walmart USA Retail Dataset: 2010-2012

Source of Dataset: https://www.kaggle.com/datasets/yasserh/walmart-dataset

## Context:

Leveraging the dataset discovered on Kaggle, a Data Science modelling and machine learning approach was taken, to solve a regression problem.
This dataset contained the following information:
* Store number
* Date
* Weekly_Sales
* Holiday Flag
* Temperature
* Fuel Price
* CPI in the USA at that time
* Unemployment rate

The following approach was taken:
* Preliminary data investigation
* Exploratory data analysis and assessment of data quality (i.e. clean, free from spelling errors)
* Preliminary univariate and bivariate analysis
* Feature engineering, primarily from datetime components, such as time lags and rolling averages
* Machine Learning from 5 common models - Linear Regression, KNN Regressor, Gradient Boosting Regressor, Support Vector Machine, etc. + Model Evaluation (adjusted R2, cross-val, RMSE)
* Hyperparameter tuning was also applied, and after some attempts, Gradient Boosting Regressor was selected with the highest adjusted R2 and non-sensitivity to multicolinearity across variables.
* Insights from feature importance for store performances & recommmendations for improvement for the future analysis
* ARIMA & SARIMA (WIP - will return to this component later).


Conclusions:
The findings point to the importance of more information, as the model's residual analysis points to potentially missing data that could reinforce the relationships uncovered in the model.
For example, pulling in more information about product data (most popular categories), more on location data of each store, and other macro-economic factors to reinforce this model.
Some important findings were the importance of rolling 3-day averages (which may be from colinearity), as well as Fuel Price as potentially one indicator of increasing sales at a Walmart store.
