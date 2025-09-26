# Financial Risk Analysis – Financial Health Score Prediction

## Project Overview
This project analyzes financial company data to detect financial indicators that influence financial score.
It simulates an end-to-end Data Analyst / Data Scientist workflow:  
- Data cleaning  
- Exploratory Data Analysis (EDA)  
- Machine Learning modeling

## Project Files
- [notebooks/financial_risk_analysis.ipynb](notebooks/financial_risk_analysis.ipynb) → main notebook with data cleaning, EDA, and ML modeling
- [data/financial_data.csv](data/financial_data.csv) → dataset used for cleaning, EDA, and machine learning models
- [data_dictionary/dictionnaire_data_unite_mesure.xlsx](data_dictionary/dictionnaire_data_unite_mesure.xlsx) → full data dictionary

## Dataset
- Type: Financial indicators (simulated dataset)  
- Variables (33 total):
  - Identity & Context  
  - Financial Health  
  - Liquidity (7 variables)  
  - Profitability  
  - Risks & Commitments  
  - Human & External Factors  
- Size: **42,000 records**

## Methodology
1. **Data Cleaning**: missing values  
2. **EDA**: distributions, correlations 
3. **Feature Engineering**: scaling, encoding, transformations  
4. **Machine Learning Models**: Linear Regression, Ridge Regression, Random Forest, XGBoost, Gradient Boosting  
5. **Evaluation Metrics**:R², RMSE

## Results
- **Key indicators influencing financial score**:
  - Debt-to-equity ratio  
  - Interest coverage ratio  
  - Leverage ratio  
  - Equity
 
- **Model comparison**:
  - Gradient Boosting achieved the best trade-off between performance and efficiency.  
  - Models with extensive hyperparameter tuning (e.g., XGBoost, Ridge) yielded slightly better scores but were significantly more computationally expensive.  

## Tools & Libraries
- Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)  
- Jupyter Notebook

## How to Run
Clone the repo and install dependencies: 

```bash
git clone https://github.com/AudreyTravant/financial-risk-analysis.git
cd financial-risk-analysis
pip install -r requirements.txt
jupyter notebook
