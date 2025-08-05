# Corporate Bankruptcy Prediction

## Overview
This project predicts corporate bankruptcy using financial ratios from a dataset of 6,819 companies with 96 features. The objective is to identify firms at risk of bankruptcy using machine learning models, enabling better credit risk management, informed investment decisions, and stronger financial oversight. Models developed include Logistic Regression (baseline), Random Forest (ensemble), and XGBoost (gradient boosting), with class imbalance addressed using SMOTE.

---

## Motivation
Corporate bankruptcies can cause significant losses for banks, investors, and regulators, and traditional financial analysis often fails to capture early warning signals of financial distress. Leveraging machine learning enables the detection of complex patterns in financial ratios, allowing for proactive and evidence-based decision-making.

---

## Problem Statement
Financial institutions and stakeholders need a reliable system to:
1. Predict bankruptcy accurately despite class imbalance.
2. Identify key financial indicators driving corporate distress.
3. Provide actionable insights for risk management and policy planning.

---

## Objectives
- Preprocess and standardize financial data.
- Address class imbalance using SMOTE.
- Train and evaluate Logistic Regression, Random Forest, and XGBoost models.
- Perform feature importance analysis to identify key drivers of bankruptcy.
- Provide insights on business impact for banks, investors, corporates, and regulators.

---

## Methodology
1. **Data Preprocessing**:
   - Standardization of features.
   - Handling class imbalance using SMOTE.
2. **Model Development**:
   - Logistic Regression as the baseline.
   - Random Forest to capture non-linear patterns.
   - XGBoost for advanced gradient boosting.
3. **Evaluation Metrics**:
   - Accuracy, Precision, Recall, F1-Score, and AUC-ROC.
   - Feature importance analysis for key ratios.

---

## Observations
- **Logistic Regression**: Provided interpretable coefficients but had lower recall, making it less effective at detecting bankrupt firms.
- **Random Forest**: Captured non-linear relationships, achieved higher recall and AUC-ROC, with liquidity and leverage ratios as dominant predictors.
- **XGBoost**: Delivered the best overall performance, balancing predictive power and generalization, making it the most suitable for deployment.
- **General Findings**: SMOTE improved recall significantly, and liquidity, leverage, and profitability ratios consistently emerged as key drivers of bankruptcy.

---

## Business Impact
The project provides significant value across stakeholders:
- **Banks**: Improved credit risk management, proactive monitoring, and better capital allocation.
- **Investors**: Informed investment decisions, enhanced valuation analysis, and risk-adjusted returns.
- **Corporates & Regulators**: Early warning systems, stronger regulatory oversight, and improved policy planning.
- **Overall Impact**: Promotes data-driven decision-making, reduces financial losses, and enhances market stability.

---

## Key Results
- **XGBoost** achieved the highest recall and AUC-ROC, minimizing false negatives.
- Feature importance analysis highlighted **liquidity, leverage, and profitability ratios** as critical indicators of financial health.
- Ensemble models outperformed linear models, confirming that financial distress is driven by non-linear interactions.

---

## Repository Structure
corporate-bankruptcy-prediction/
│── data/ # Dataset (or link to source)
│── notebooks/ # Jupyter notebooks for EDA & modeling
│── scripts/ # Python scripts for preprocessing & training
│── results/ # ROC curves, feature importance plots, metrics
│── report/ # Final PDF and presentation
│── requirements.txt # Python dependencies
│── README.md # Project overview


---

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/<your-username>/corporate-bankruptcy-prediction.git

## Install dependencies:

pip install -r requirements.txt

## Run model training:

python scripts/train_models.py

Author
Anushka Churi
MBA (Finance) | Electronics & Telecommunication Engineering with Honours in Data Science
