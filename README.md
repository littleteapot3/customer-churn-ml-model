# Telecom Customer Churn Prediction

This project forecasts whether a customer will leave Interconnect, a telecom provider, using personal, contract, and service usage data. It was completed as part of a data science bootcamp final sprint.

## 🗂️ Project Structure
- `notebook.ipynb`: Contains all EDA, preprocessing, and modeling steps
- `datasets/`: Folder containing the four original CSV files
- `report.md`: Summary report prepared for the team leader
- `README.md`: Project overview

## 🧠 Goal
Client wants to identify customers who are likely to cancel their service contracts. By forecasting client churn in advance, the company can proactively offer promotional deals or plan adjustments to retain at-risk users. This project aims to build a machine learning model that supports that goal using personal, contract, and service usage data.

## 📊 Dataset
The dataset includes four CSV files:
- `contract.csv`
- `personal.csv`
- `internet.csv`
- `phone.csv`

Each file uses `customerID` as a common identifier.

## 📈 Target & Metrics
- **Target**: Customer churn (defined as `EndDate != "No"`)
- **Primary Metric**: AUC-ROC
- **Secondary Metric**: Accuracy

## 🚧 Work Plan
1. Exploratory Data Analysis
2. Data Cleaning & Merging
3. Feature Engineering
4. Model Training & Tuning
5. Final Evaluation & Report

## 📌 Status
In progress 🚧
