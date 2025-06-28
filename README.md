# Cross-Selling Modeling in Insurance – Predictive Analytics Project (UNED)

This repository contains a complete machine learning pipeline developed for the prediction of customer response to a cross-selling campaign. The project was created for Module 7 – Big Data in the Insurance Sector, as part of the Master's in Big Data and Data Science Applied to Economics and Business at UNED (2024–2025).

## 🎯 Objective

The goal of the project is to predict whether a customer will purchase an additional insurance product, based on demographic and behavioral data. This enables optimized targeting of marketing actions and improved campaign ROI.

## 📊 Dataset Overview

The dataset includes a sample of customers with their:
- Socio-demographic attributes (e.g., age, gender, profession)
- Product subscription data (e.g., product1, product2, ...)
- Response variable: `target` (binary)

The dataset was split into a training and a validation set to ensure unbiased evaluation.

## 🧪 Project Workflow

- **EDA & Data Cleaning**:
  - Data inspection and variable transformation
  - Grouping categorical variables with many levels
  - Addressing class imbalance (explored but not applied)

- **Model Training**:
  - Multiple algorithms trained using `caret`
  - Validation with 5-fold cross-validation (1 repeat)
  - Models evaluated with ROC AUC and PR AUC

- **Model Comparison**:
  - Visualization of model performance
  - Metrics stored for reproducibility
  - Best model: XGBoost (caret), RMSE ≈ 4.6, R² ≈ 0.75

- **Interpretability**:
  - Local and global explanations using DALEX
  - Variable importance, SHAP values, and what-if analysis

- **API Deployment**:
  - Productivization of the model using `plumber`
  - Interactive documentation with Swagger
  - Custom endpoint with parameter validation and enumerated fields

## ⚙️ Tools Used

- R and RStudio  
- caret, DALEX, ggplot2, dplyr, plumber  
- RMarkdown for reproducible reporting  
- GitHub for project versioning

## 📄 Output

The complete cross-selling report is available here:  
📎 `Oscar_Porta_Modulo7_VentaCruzada.html`

## 👨‍💻 Author

Óscar Porta  
Master’s Student in Big Data & Data Science – UNED  
GitHub: [Oscar-Porta](https://github.com/Oscar-Porta)
