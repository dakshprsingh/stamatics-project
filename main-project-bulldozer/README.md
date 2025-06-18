# Bulldozer Price Prediction Project

## Objective
This project aims to build a machine learning model that can accurately predict the sale price of bulldozers and other heavy machinery at auction. The goal is to assist Fast Iron in developing a reliable “Blue Book” pricing guide based on various factors like:

- Usage hours
- Equipment type and configuration
- Sale date and auction-related features

---

## Dataset Overview

- **Train.csv** – Contains historical auction data with known sale prices.
- **Test.csv** – Includes similar equipment data without prices (used for final predictions).
- **Data Dictionary.xlsx** – Explains each feature in detail.

---

## Phase 1: Data Understanding

- Explored structure, types, and distributions.
- Identified missing values and outliers.
- Understood key variables like `Usage`, `YearMade`, `MachineHoursCurrentMeter`, and `ProductGroup`.

---

## Phase 2: Data Cleaning & Preparation

- Handled missing values using imputation or dropping irrelevant columns.
- Converted data types (e.g., `saledate` to datetime).
- Extracted time-based features (e.g., `saleYear`, `saleMonth`).
- Applied label encoding and one-hot encoding for categorical features.

---

## Phase 3: Model Building

- Trained several regression models:
  - Linear Regression
  - Random Forest Regressor
  - XGBoost Regressor

- Evaluated performance using **RMSLE** (Root Mean Squared Logarithmic Error).
- Final model: **Random Forest** (balanced accuracy and interpretability)

---

## Phase 4: Final Predictions

- Applied the final model on the test dataset.
- Saved predictions to `test_predictions.csv` in the required format:

