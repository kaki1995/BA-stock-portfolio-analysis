# Project: Stock Return Prediction and Portfolio Optimization

**1. Introduction**
   
This project focuses on optimizing stock portfolios of 10 US companies from various industries by applying financial theories and machine learning models. The data is collected from WRDS database including Stock Daily Trading dataset and Financial Ratios dataset from 01-01-2022 to 31-12-2023. It includes sections for data processing, descriptive analysis, predictive analysis using different machine learning models and one time series model, model evaluation and selection for return prediction, rolling windows and optimisation strategies for choosing and adjusting portfolio optimal weights.

This project is important in real world´s situation for managers or investors in making informed short-term trading decisions and developing long-term strategies based on stock market data. The aim is to develop a methodology for calculating and predicting an optimal stock portfolio that maximizes the Sharpe Ratio.

**2. Step-by-step analysis**

To achieve this goal, we carefully planned and carried out the following steps: 
- Pre-select 10 most profitable companies in 2023;
- Choose variables (including daily trading data and monthly financial ratios) according to relevant literature;
- Download and merge the two datasets, and handle missing data;
- Descriptive analysis, including …
- Data preparation before predictive analysis, including transforming categorical variables, creating lagged features, data standardization, and data splitting;
- Evaluate the prediction accuracy of 6 models, including Linear Regression (Ridge and Lasso), Random Forest, Support Vector Regression, Deep Neural Networks, and SARIMAX, and select the fine-tuned Random Forest model as the prediction model;
- Apply the rolling window technique to predict returns and use optimization methods (CVXPY and Gurobi) to allocate weights;
- Create two benchmarks: equal-weighted portfolio and S&P Composite Index;
- Compare the optimized portfolios' annual return, risk and Sharpe Ratio with those of the two benchmarks.

**3. Files**
- Data (taken from WRDS Dataset: https://wrds-www.wharton.upenn.edu/login/?next=/pages/get-data/)
1. Financial Ratios_Top 10 Profitable Companies_2y.csv
2. Stock_Daily_Trading.csv
3. Return on S&P Composite Index-2023.csv
4. Merged_dataset_clean.csv
   
- Python File for analysis: Final Submission Code.ipynb


**4. Tools**

This project requires you to have the following tools installed: Python v3 (https://www.python.org/downloads/)

The following python libraries should be installed:
1. cvxpy (https://www.cvxpy.org/install/)
2. arch (https://pypi.org/project/arch/)
3. matplotlib (https://pypi.org/project/matplotlib/)
4. sklearn (https://pypi.org/project/scikit-learn/)
5. numpy (https://pypi.org/project/numpy/)
6. pandas (https://pypi.org/project/pandas/)
7. statsmodels (https://pypi.org/project/statsmodels/)
8. gurobipy (https://pypi.org/project/gurobipy/)
