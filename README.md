# Telecom Customer Churn Prediction

This project forecasts whether a customer will leave Interconnect, a telecom provider, using personal, contract, and service usage data. It was completed as part of a data science bootcamp final sprint.

## 🧠 Goal
Client wants to identify customers who are likely to cancel their service contracts. By forecasting client churn in advance, the company can proactively offer promotional deals or plan adjustments to retain at-risk users. This project aims to build a machine learning model that supports that goal using personal, contract, and service usage data.

## 📊 Dataset
The dataset includes four CSV files joined on customerID:

- contract.csv
- personal.csv
- internet.csv
- phone.csv

These were cleaned, merged, and encoded into a final modeling dataset.


## 📈 Target & Metrics
- **Target**: Customer churn (defined as `EndDate != "No"`)
- **Primary Metric**: ROC-AUC
- **Secondary Metric**: Accuracy

## 📂 Project Structure
- fp_eda_and_analysis.ipynb: EDA, statistical tests, and data cleaning
- fp_churn_modeling.ipynb: Feature scaling, model training, tuning, and evaluation
- datasets/: Original CSVs and final encoded dataset (churn_cleaned.csv)
- report.md: Summary report for team leader
- README.md: Project overview

## 📌 Status📌 Status
✅ Project completed
✅ All models tested and evaluated
✅ Final model selected and recommendations delivered


## 📈 Results Summary
| Model                  | Accuracy | ROC AUC |
|------------------------|----------|---------|
| XGBoost (Tuned)        | 0.8567   | 0.8956  |
| Random Forest (Tuned)  | 0.8322   | 0.8732  |
| Decision Tree (Tuned)  | 0.8134   | 0.8580  |
| Logistic Regression    | 0.8060   | 0.8487  |
| Decision Tree (Untuned)| 0.7981   | 0.7340  |

## ✅ Final Recommendation
We recommend using the tuned XGBoost model, which achieved the highest accuracy and ROC AUC score. It identified contract type, internet service, and tenure as the top churn predictors — patterns that align with business logic and earlier exploratory analysis.

This model would be an effective foundation for powering churn-risk dashboards or retention strategies.

## 🚀 Ideas For Next Steps 
- Deploy model outputs to a dashboard to monitor churn risk by customer
- Export predictions to support outreach lists or promotional campaigns
- Test retention strategies informed by top risk factors (e.g. short tenure, month-to-month plans)
- Retrain the model regularly with fresh data to keep performance high
- Explore customer lifetime value (CLV) modeling to pair with churn predictions for prioritization


