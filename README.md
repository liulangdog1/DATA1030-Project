# Parkinson's Disease Progression Analysis  

## Overview  
This project predicts Parkinson's disease progression using voice features from the [UCI Parkinson's Telemonitoring Dataset](https://archive.ics.uci.edu/ml/datasets/Parkinsons+Telemonitoring). Models estimate **Motor UPDRS** and **Total UPDRS** scores.

## Project Structure  
- **data/**: Raw and preprocessed data  
- **figures/**: Plots and visualizations  
- **results/**: Predictions, saved models, and performance summary  
- **report/**: Final report (PDF)  
- **src/**: Jupyter Notebooks for analysis  
- **environment.yaml**: Python dependencies  
- **LICENSE**: Project license  
- **README.md**: Project description  

## Workflow  
1. **EDA**: Analyze feature distributions and correlations.  
2. **Preprocessing**: Standardize features and remove multicollinearity.  
3. **Modeling**: Train and evaluate ElasticNet, KNN, Random Forest, XGBoost, and SVR.  
4. **Results**: Compare models using RMSE and analyze feature importance with SHAP.

| Model            | Motor UPDRS RMSE | Total UPDRS RMSE |  
|------------------|------------------|------------------|  
| Baseline         | 9.04             | 11.30            |  
| ElasticNet       | 8.90             | 11.00            |  
| K-Nearest Neighbors (KNN) | 8.80     | 11.10            |  
| Random Forest    | 8.50             | 10.90            |  
| XGBoost          | 8.00             | 11.50            |  
| SVR (Best)       | 7.50             | 10.20            |  

**Insights**:  
- **Age** is the most important feature, followed by **DFA**, **HNR**, and **PPE**.

## How to Run  
1. Clone this repository:  
   ```bash
   git clone https://github.com/YOUR_USERNAME/parkinsons-analysis.git
   cd parkinsons-analysis

##Required library versions:

python=3.10.5
matplotlib=3.5.2
pandas=1.4.2
scikit-learn=1.1.1
numpy=1.22.4
xgboost=1.5.1
shap=0.40.0
jupyter_client=7.3.1
jupyter_core=4.10.0
jupyterlab=3.4.2
jupyter_server=1.17.0
jupytext=1.13.8
rise=5.7.1
plotly=5.8.0
ipywidgets=7.7.0
